# ติดตั้ง Ubuntu Server 20.04.1 LTS

REFER =>  https://github.com/wachira90/python-unifi

## 1. Download Ubuntu Server 20.04.1 LTS

````
ดาวน์โหลดได้ที่ https://www.ubuntu.com/download/server
````

## 2. ติดตั้ง Ubuntu Server 20.04.1 LTS ตามกระบวนการปกติ



# ติดตั้ง Unifi Controller 

##  1. ติดตั้ง mongodb

````
sudo apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv 0C49F3730359A14518585931BC711F9BA15703C6
````

## 2. Unifi List Key

````
sudo apt-key adv --keyserver keyserver.ubuntu.com --recv 06E85760C0A52C50
````

## 3.MongoDB List File
````
echo "deb [ arch=amd64,arm64 ] http://repo.mongodb.org/apt/ubuntu xenial/mongodb-org/3.4 multiverse" | sudo tee /etc/apt/sources.list.d/mongodb-org-3.4.list
````

## 4. Unifi List File

````
echo 'deb http://www.ubnt.com/downloads/unifi/debian stable ubiquiti' | sudo tee /etc/apt/sources.list.d/100-ubnt-unifi.list
````

## 5. Update the local package database:

````
sudo apt-get update
````

## 6. Install MongoDB 3.4.x

````
sudo apt-get install mongodb-org
````

## 7. ติดตั้ง Unifi controller

````
sudo apt-get install unifi
````

## 8. เข้าใช้งาน
````
https://localhost:8443
````
