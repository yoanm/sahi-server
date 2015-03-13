# sahi-server
Sahi server for behat, configured with a phantomjs proxy

#Require 
__PhantomJs working installation__ ([Ubuntu help there](https://gist.github.com/yoanm/7777b571acffe9491ad7))

On Ubuntu : 
```shell
# from https://gist.github.com/julionc/7476620
#Instal depedencies
cd ~
sudo apt-get update
sudo apt-get install build-essential chrpath libssl-dev libxft-dev
sudo apt-get install libfreetype6 libfreetype6-dev
sudo apt-get install libfontconfig1 libfontconfig1-dev

#Download and extract PhantomJs package
export PHANTOM_JS="phantomjs-1.9.8-linux-x86_64"
wget https://bitbucket.org/ariya/phantomjs/downloads/$PHANTOM_JS.tar.bz2
sudo mv $PHANTOM_JS.tar.bz2 /usr/local/share/
cd /usr/local/share/
sudo tar xvjf $PHANTOM_JS.tar.bz2

#create links
sudo ln -sf /usr/local/share/$PHANTOM_JS/bin/phantomjs /usr/local/share/phantomjs
sudo ln -sf /usr/local/share/$PHANTOM_JS/bin/phantomjs /usr/local/bin/phantomjs
sudo ln -sf /usr/local/share/$PHANTOM_JS/bin/phantomjs /usr/bin/phantomjs

#then see https://github.com/Gizra/KnowledgeBase/wiki/Behat-phantomJs-install
```
#How to use
 + Clone repository on your machine.
 + If your PhantomJs executable path is not `/usr/local/bin/phantomjs`, edit this file [`userdata/config/browser_types.xml`](https://github.com/yoanm/sahi-server/blob/master/userdata/config/browser_types.xml) and update the [`path node`](https://github.com/yoanm/sahi-server/blob/master/userdata/config/browser_types.xml#L6)
 + From repository folder, go to `bin` directory and start Sahi server by typing : 
```shell
  ./sahi.sh
```
