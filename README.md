int sensor1Value = 0;
void setup()
{
  // declare the ledPins as an OUTPUT:
  pinMode(13, OUTPUT);
  
}

void loop() {
  // read the value from the sensor:
  sensor1Value = analogRead(A0);
{
  if(sensor1Value <200)     // check the value of sensor 
 {                          //if the value is less than 200 then turn the leds on
 digitalWrite(13, HIGH);
  delay(500);
 }
 else                      // if the value is greater than or equal to 200 then turn leds off
 {
  digitalWrite(13, LOW);
  delay(500);
}
