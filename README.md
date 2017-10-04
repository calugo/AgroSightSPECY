#  AgroSightSPECY - SPECY IMPLEMENTATION using 2 STS spectrometers.


This is an extension of [SPECY](https://github.com/wemperor/SPECY)  originally developed by
[wemperor](https://github.com/wemperor).
  This version implements two STS spectrometers using a microcontroller such as an Arduino Mega to capture data   using UAVs or ground and lab setups.

The connections (plus an additional SD-logger ethernet shield) are as follows:

<p align="center">
  <img src="https://github.com/calugo/AgroSightSPECY/blob/master/setup.png?raw=true" alt="SPECY2"/>  
</p>

In order to have adequate time stamps it is necessary to set the RTC unit in case of battery replacement or first use. The sketch __rtcset.ino__ can be used for such a task.

The firmware is located in the folder __ATSpecy_Firmware_V1_1__ and contains the protocols for each spectrometer, RTC related functions, and data logging. On its present form the execution of the code calibrates the intergration times, computes the spectra and serially prints the spectra and temperatures, so the data is made available to a data stream.

<p align="center">
  <img src="https://github.com/calugo/AgroSightSPECY/blob/master/pics/IMG-20171003-WA0019.jpg?raw=true" alt="SPECY2"/>  
</p>


To monitor the performance of the devices a jupyter notebook is also included although the arduino serial port monitor can be used as well. A snapshot can be seen [here](https://nbviewer.jupyter.org/github/calugo/AgroSightSPECY/blob/master/SPECYtest.ipynb)


An early implementation of the system is shown below:

<p align="center">
  <img src="https://github.com/calugo/AgroSightSPECY/blob/master/pics/IMG-20171003-WA0010.jpg?raw=true" alt="SPECY2"/>  
</p>

<p align="center">
  <img src="https://github.com/calugo/AgroSightSPECY/blob/master/pics/IMG-20171003-WA0016.jpg?raw=true" alt="SPECY2"/>  
</p>
