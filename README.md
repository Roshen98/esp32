# esp32

Create a program on your personal computer that will communicate with your ESP32 over WiFi. 
The user should be able to press 1 or 2 to turn on or off respectively a corresponding LED light connected to the ESP32.  
Additionally, the program running from the terminal should also update the status of the LED light. Indicating if it is “ON” or “OFF” 
To communicate with the ESP32 you will use an MQTT broker. This is a program that will run on your laptop/desktop that will relay messages sent by publishers to subscribers. https://mosquitto.org/download/

After completing the program above to introduce yourself to the microcontroller you are free to create another program of your choosing with the following caveats:
It must utilize MQTT.
It must be automated using a script that will call and effectively send commands and be able adapt to messages sent back from the ESP32.
I suggest challenging yourself as your program difficulty will be factored into your final score.

SETUP:
Download and install Ardunio for your O.S.: https://www.arduino.cc/en/Guide
Ardunio is essentially a C program with two functions. 
setup() and loop()
Essentially, it is run as follows in a C program

//This is essentially how setup() and loop() are being called
void main(){
    
    setup();    //Setup() will be run one time at the beginning. 
                //Good time to setup and initialize.
    
    while(1)
        loop(); //Loop() will be run in an infinite loop. 
                //Microcontrollers are designed to be run forever.
    
}
