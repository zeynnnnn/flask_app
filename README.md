Flask app for cloud models of drivision

Download vehicle detection checkpoint from: https://drive.google.com/file/d/0B5WIzrIVeL0WS3N2VklTVmstelE/view and put it to the models/vehicle_detection/weights folder
## HOW TO RUN (WITH DOCKER)
sudo docker-compose up --build 


## HOW TO RUN (WITHOUT DOCKER)

reference: https://www.alexkras.com/how-to-use-virtualenv-in-python-to-install-packages-locally/


* pip install virtualenv
* cd drivision-models
* virtualenv venv
* source venv/bin/activate (bu virtual env'i aktive ediyor, virtualenv i kapatmak icin deactivate yaziyoruz)
* pip install -r requirements.txt

bunlari yaptiktan sonra ben pycharm kullandigim icin yapmaniz gerekenler pycharm'a gore anlatildi

file -> other settings -> preferences for new projects -> project interpreter

burada secili bir interpreter yoksa, sag taraftaki + ya basarak interpreter ekleyin. interpreterin gosterdigi konum "drivision-models/venv/bin/python" olmali. (bunu yapmadan da calisabilir aslinda ama garanti olsun diye ekledim)

apply ve ok deyin.

sonra sol ustte edit configurations -> + -> python'a basin.

sonra script path'te predict.py i secin.
 
sonra interpreter kisminda project default yazani secin. (konum drivision-models/venv/bin/python olacak)

sonra working directory drivision-models olacak ondan emin olun.

apply -> ok.

sonra runlayabilirsiniz.


