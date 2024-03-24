Laboratory Work report "Bluetooth Device Security Assessment"
Amiruldayev Emil SIS-2121



Purpose:
The purpose of this laboratory work was to evaluate the security of Bluetooth-enabled devices by conducting their detection and identification using Python.

Tools and libraries used:
To do the work, the Python programming language was used, as well as the PyBluez library for working with Bluetooth devices.

Progress of work:

Preparing the environment: Before starting work, make sure that the PyBluez library is installed on the computer. In case of its absence, it was installed using pip.
Program development: We wrote a Python program that detects nearby Bluetooth devices and outputs information about each detected device, including its name, MAC address, device class and supported services.
We tested the program: We launched the program and made sure that it works correctly, detecting and displaying information about available Bluetooth devices.


Let's analyze each function from the program in steps:
 ![image](https://github.com/amiruldayev/Bluetooth-Device-Security-Assessment/assets/114305101/200b3158-518c-4e31-b696-cc51190d04d4)

This feature uses the bluetooth library to detect nearby Bluetooth devices.
Inside the function, the bluetooth.discover_devices() method is called, which returns a list of detected devices.
The parameters lookup_names=True and lookup_class=True indicate that the function should also get the names and classes of the detected devices.


![image](https://github.com/amiruldayev/Bluetooth-Device-Security-Assessment/assets/114305101/2fa62d9e-fc55-4e91-8f43-2a2b73f3572d)


 
This function accepts information about each detected device in the form of a device_info tuple containing the MAC address, name and class of the device.
It displays information about each device, including its name, MAC address, and device class.
It also calls the bluetooth.find_service() method to find the services available on this device.


 ![image](https://github.com/amiruldayev/Bluetooth-Device-Security-Assessment/assets/114305101/0c74b306-c933-41d1-a230-151a32fb14b2)

This is the main function of the program that controls the execution of the entire script.
At the beginning, it displays a message about the start of the search for nearby Bluetooth devices.
Then calls the discover_devices() function to discover the devices.
After receiving the list of devices, it displays the number of devices found.
Next, for each detected device, the print_device_info() function is called, which outputs information about each device.

 ![image](https://github.com/amiruldayev/Bluetooth-Device-Security-Assessment/assets/114305101/246abd64-d14d-4a9c-afc3-f2049906341c)


This construct checks whether a given script is run directly and not imported into another script.
If the script is run directly (that is, if its name is "main"), then the main() function will be called automatically.

Result:
 ![image](https://github.com/amiruldayev/Bluetooth-Device-Security-Assessment/assets/114305101/40834cd5-a941-4a64-b6ef-9f1205f27076)



Conclusions:
As a result of the laboratory work, a Python program was developed that allows you to detect Bluetooth devices in the environment and output information about them. This allows you to conduct an initial security assessment of Bluetooth devices and identify potential vulnerabilities. However, additional analysis tools and techniques should be used for a full-fledged safety assessment.
