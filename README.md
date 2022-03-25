# Arduino_Tutorial

This tutorial aims to guide through Arduino's usage alongside of testing with OPT3001.

###step1:
OPT3001, as an ambient light sensor, have a look at its data sheet to know:  
its `INT`, `SDA`, `SCL`, `GND`, 'VDD' attach to which part on the Arduino Hardware Board.
Then use Flexible Flat Cable （FFC）to attach the ports on the places on the board, in this case, `SQL' none, `GND` -> 接地, `VDD` -> 5V, `SDA` -> A4, `INT` -> A5, 

###step2: 
connect the Arduino Hardware with the Arduino Software. 
In the software, load [sketch_scan_address] (found on the CSDN), click `Verify` -> `Upload`, and then `Tools` -> `Serial Monitor` to see if any ERRORs occuring. Then, you will get the address of the sensor.

###step3:
load [opt3001demo], click `Sketch` -> `Include Library` -> `Add .ZIP Library', browse the file `src`, and then click on the `Include Library` the new-added library, `src`.
clicl `Verify`-> `Upload`, and then `Tools` -> `Serial Monitor` to check if there is any ERROR, click `Serial Plotter` to observe the sensed graphs. 
