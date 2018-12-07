# LEGO_Kibble_Balance
Software for LEGO Kibble Balance. Utilises the example code provided by LabJack U6 and Phidgets. 

## LabJack U6
The LabJack U6 is a multifunction DAQ device. For the LEGO Kibble Balance, only two of the Analogue Input ports are used which are AIN0 and AIN1. There are examples methods which are implemented in 'LEGO_Kibble_Balance.py' which can be found at <https://github.com/labjack/LabJackPython>.

## Phidget Analogue 4-Output
The Phidget Analogue is a +-10V DAC. For the LEGO Kibble Balance, the Phidget uses output 0 and 1, the use of which is demonstrated in LEGO_Kibble_Balance.py

## Required installs 

* wxPython - This is a module that allows python to build the Graphic User Interface (GUI) for the Kibble Balance. 
Currently LabJack U6 is only compatible with Python 2.7 and as such the latest version of wxPython will not
work. Older versions of wxPython can be found here <https://sourceforge.net/projects/wxpython/files/wxPython/>.
wxPython 3.0.2.0 is compatible with Python 2.7. 

* LabJack U6 - In order to communicate with LabJack U6, follow the set of instructions in 
<https://labjack.com/support/software/examples/ud/labjackpython>. Further more, download the .zip file
at the bottom of the page. Extract its contents and run ``` python setup.py install ```.  

* Phidget - To install the phidget API, download "Phidget Python module" from <https://www.phidgets.com/docs/Language_-_Python#Quick_Downloads>. Run 
`
	python setup.py install
`
within the downloaded folder

* matplotlib.pyplot - After making the measurements, the program uses matplotlib.pyplot to plot the mass measurements.
This needs to be installed using the following 2 cmd commands
```python -m pip install -U pip```, ```python -m pip install -U matplotlib```

* Phidget Control Panel - The link required to install the control panel for using the Phidget device can be found
in <https://www.phidgets.com/docs/OS_-_Windows#Getting_started_with_Windows>.