# Smart Parking System using Arduino & RFID Sensor

> Second Year Mini-Project for subject ADE

### Description :

Smart Parking System enables you a secure process for parking owner's vehicles without any intrusion of an unknown vehicle using an RFID sensor.
RFID sensors can sense only those RFID tags that are registered and reject the rest.
When a tag/card is accepted, the barrier attached using a Servo motor will lift up and the vehicle will be allowed to enter the parking area.
LCD screen is used to display the remaining Parking slots.
A person is allowed only if the remaining parking slots are greater than 0.
IR sensors are attached to each Parking slot to track the count of parking slots.


### Components Used :

| Component               | Quantity     |   
| -------------            | ------------ | 
|  RFID Sensor RC522    | ` X 1 `      | 
|  RFID Tags             | ` X 2 `      | 
|  IR Ssensors             | ` X 3 / 4 `  | 
|  16x2 LCD Display       | ` X 1 `      | 
|  Servo motor       | ` X 1 `      | 
|  Active Buzzer         | ` X 1 `      | 
|  Arduino UNO          | ` X 1 `      | 
|  Arduino USB cable     | ` X 1 `      | 
|  Potentiometer         | ` X 1 `      |
|  Jumper wires         | ` X 1 `      | 


### How to implement: 

1. Read the Unique ID from RFID tags using [DumpInfo](https://github.com/Vipsy-123/Smart-Parking-System-using-Arduino-RFID/blob/main/DumpInfo/DumpInfo.ino) code one by one.
2. Copy these values into the main code. 
3. RFID will detect only those cards whose UID is stored.
4. Run the main code

### Note :

* As there were no Digital pins remaining due to LCD and RFID sensor pins, Analog pins were used to give signals to IR 
  sensors and active buzzers.
* The values for Analogwrite for the IR sensor were fed in the code.
* There is a Unique ID for each RFID tag.
* Please use the recommended GitHub library to get the RFID ID for your tag and add it to your Arduino code.
