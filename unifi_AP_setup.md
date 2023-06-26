// default credentials ubnt/ubnt
ssh -v -oHostKeyAlgorithms=+ssh-rsa ubnt@{AP-IP-ADDRESS}

//reset AP to factory 
sudo syswrapper.sh restore-default

// send request to your controller
set-inform http://{controller-ip}:8080/inform
