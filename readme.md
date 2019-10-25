# Set up SoapySDR fro SDRPlay and rtl_433 on Mac OSX

From...

https://www.sdrplay.com/mac-soapy-source/

Run...

Build SoapySDRPlay…

cd ~/Dev

sudo rm -rf SoapySDRPlay

git clone https://github.com/pothosware/SoapySDRPlay.git

cd SoapySDRPlay

mkdir build
cd build

cmake ..

sudo make install

sudo ldconfig

To check the SoapySDR installation, type the following into a terminal window:

SoapySDRUtil -info

and also

SoapySDRUtil --probe=sdrplay

(run twice if the RSP is not found the first time)

Then install rtl_433...

https://github.com/merbanan/rtl_433/blob/master/docs/BUILDING.md

rtl_433 -d ""



I previosuly did this...

https://github.com/pothosware/homebrew-pothos/wiki

https://github.com/pothosware/SoapyRTLSDR/wiki

But maybe the above removes need
