# sahi-server
Sahi server for behat, configured with a phantomjs proxy

#Require 
__PhantomJs working installation__ ([Help there](https://gist.github.com/yoanm/7777b571acffe9491ad7))

#How to use
 + Clone repository on your machine.
 + If your PhantomJs executable path is not `/usr/local/bin/phantomjs`, edit this file [`userdata/config/browser_types.xml`](https://github.com/yoanm/sahi-server/blob/master/userdata/config/browser_types.xml) and update the [`path node`](https://github.com/yoanm/sahi-server/blob/master/userdata/config/browser_types.xml#L6)
 + From repository folder, go to `bin` directory and start Sahi server by typing : 
```shell
  ./sahi.sh
```
