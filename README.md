# mhdgc-docker
docker setup for local development of mhdgc.org website

## project setup
1. create a project directory somewhere on your local machine:  
`mkdir ~you/Documents/mhdgc`  
`cd ~you/Documents/mhdgc`
2. clone this repo into `docker` directory within the project directory:  
`git clone git@github.com:yamanote1138/mhdgc-docker.git docker`
3. clone the mhdgc-www repo into a directory named `www` in your project directory:  
`git clone git@github.com:yamanote1138/mhdgc-www.git www`
4. create a `data` directory:  
`mkdir data`
5. add dev subdomain to your host config:  
`sudo echo '127.0.0.1 dev.www.mhdgc.org' >> /etc/hosts`

## database migration
(ideal process and documentation tbd)

## to start
`cd ~you/Documents/mhdgc/docker`  
`docker-compose up -d` (starts Docker containers in detached mode)

## viewing the site
in your browser of choice -> [http://dev.www.mhdgc.org](http://dev.www.mhdgc.org)

## to stop
`cd ~you/Documents/mhdgc/docker`  
`docker-compose down` (stops and removes running Docker containers)
