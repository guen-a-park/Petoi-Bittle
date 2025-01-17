# Change Log


## Aug 31, 2021
* Moved the device's model info (Nybble/Bittle) to the top of booting printouts.
* Added a shorter encoding for the IR remote to save flash by about 178 Bytes.

## Aug 25, 2021
* Added an 'M' token to move multiple indexed joints to angles (ASCII format entered in the serial monitor) simultaneously;
* Re-arranged the IR key map for the new customized IR panel.

## Jun 29, 2021
* OpenCat.ino will print out the model name (Bittle/Nybble) at booting up.
* Moved #define I2C_EEPROM to the begining OpenCat.h.

## Jun 7, 2021

* Adjusted the threshold voltage so that Bittle will keep beeping when the battery goes under 6.5V, a few moments before the battery power shuts off;
* Adjusted the gaits so that the elbow won't hit the body in the accelerated phase. 
* The trot on key "1" is tuned to be faster.
* Removed the running gait on the IR remote key "2" and replaced it with "check around" behavior previously on key "3";
* Assigned a "play dead" trick to IR remote key "3". Bittle will fall on its back then roll back (if the gyro is activated);
* Removed the behavior when the robot is tilted at a large angle to avoid an occasional bug. Will put the behavior back if the bug can be fixed; 
* Added an auto detection code for a new sound&light sensor connected to the analog Grove pin. Some new automated behaviors are being developed. The code block won't be active if the sensor is not connected to the Analog Grove socket;


