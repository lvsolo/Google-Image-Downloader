# Google Image Downloader

## 1. Introdoction

Crawl and download images using Selenium + PhantomJS
Using python3 and PyQt4

## 2. Key features
+ Search Engine: Google, Bing, Baidu
+ Keywords input from keyboard, or input from line seperated keywords list file for batch process.
+ Download image using customizable number of threads.
+ Fully supported conditional search (eg. filetype:, site:).
+ Switch for Google safe mode.
+ Proxy configuration (socks, http).
+ CMD and GUI ways of using are provided.
+ **Windows prebuilt executable release from [release page](https://github.com/sczhengyabin/Google-Image-Downloader/releases).**

## 3. Solve dependencies
### 3.1 Windows
#### 3.1.1 Download and install Python3.4
Download Latest version of Python3.4 installer from [here](https://www.python.org/ftp/python/3.4.4/python-3.4.4.msi)
#### 3.1.2 Download and install PyQt4
Download latest version of PyQt4 install from [here](https://sourceforge.net/projects/pyqt/files/PyQt4/PyQt-4.11.4/PyQt4-4.11.4-gpl-Py3.4-Qt4.8.7-x32.exe/download)
#### 3.1.3 Download and setup phantomjs
Official phantomjs prebuilt executable can be downloaded from [here](https://bitbucket.org/ariya/phantomjs/downloads)

Then copy phantomjs.exe to ${project_directory}/bin/
#### 3.1.4 Install python packages
```
pip3.exe install -r requirements.txt
```
### 3.2 Linux
#### 3.2.1 Install dependent packages
```
apt-get install python3-pip python3-pyqt4 pyqt4-dev-tools
```
#### 3.2.2 Download and setup phantomjs
+ **For PC users**

Official phantomjs prebuilt executable can be downloaded from [here](https://bitbucket.org/ariya/phantomjs/downloads)
+ **For Raspberry Pi Users**

Unofficial phantomjs prebuilt executable or .deb for raspberry pi can be downloaded from [here](https://github.com/fg2it/phantomjs-on-raspberry/releases)

Add the path of phantomjs executable to $PATH, or simply copy it to /usr/local/bin/.
### 3.2.3 Install python packages
```
pip3 install -r requirements.txt
```
## 4. Usage
### 4.1 GUI
![](http://p1.bqimg.com/567571/2d72755a4d3fc319.png)
### 4.2 CMD
```
usage: image_downloader.py [-h] [--engine {Google,Bing,Baidu}]
                           [--max-number MAX_NUMBER]
                           [--num-threads NUM_THREADS] [--timeout TIMEOUT]
                           [--output OUTPUT] [--safe-mode] [--face-only]
                           [--proxy_http PROXY_HTTP]
                           [--proxy_socks5 PROXY_SOCKS5]
                           keywords
```
