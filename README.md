# In order to use 96BoardsGPIO on DragonBoard 410c, follow the follopwing procedure.

$ sudo apt-get install libsoc-dev
$ sudo apt-get install automake libtool
$ git clone https://github.com/96boards/96BoardsGPIO.git
$ cd 96BoardsGPIO
$ ./autogen.sh && ./configure
$ make && sudo make install
$ sudo ldconfig

# Clone this repo to download libsoc_gpio.conf file and copy it to /etc.

$ git clone https://github.com/nuchida/libsoc_gpio
$ cd libsoc_gpio
$ sudo cp libsoc_gpio.conf /etc
