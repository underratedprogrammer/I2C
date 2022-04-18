/// Scannig program I2C Devices
#include <Wire.h>
int address;
int error;
void setup(
  ){
    Serial.begin(9600);
    Serial.print("I2C scanner program is starting ....");
    }
void loop(){
  for(address = 0; address<127; address++){
     Wire.beginTransmission(address);
     error= Wire.endTransmission();
    if(error == 0){
      Serial.print(" I2C Device Found AT ADDRESS 0X");
      if(address < 16){
        Serial.print("0"); };       }
      Serial.print(address,HEX);
      }
    
  }
