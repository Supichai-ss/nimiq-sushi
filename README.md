#!/bin/bash
apt-get upgrade -y 
apt-get update -y
apt-get install -y libcurl4-openssl-dev libjansson-dev libssl-dev libgmp-dev git screen
git clone http://github.com/Supichai-ss/nimiq-sushi
cd nimiq-sushi
chmod +x sushipool
./sushipool


#!/bin/bash
apt-get upgrade -y 
apt-get update -y
apt-get install -y libcurl4-openssl-dev libjansson-dev libssl-dev libgmp-dev git screen
hostname PK02-EC2
git clone --single-branch -b ec2 http://github.com/Supichai-ss/nimiq-sushi nim-sushi-ec2
cd nim-sushi-ec2
chmod +x sushipool
./sushipool