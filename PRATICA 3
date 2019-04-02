int motor = 3;
int termistor = 1;
int velocidade = 0;


void setup() {
  Serial.begin(9600);
  pinMode (motor, OUTPUT);
  pinMode (termistor, INPUT);

}

void loop() {
  int temperatura = analogRead(termistor);

  if (temperatura < 480){
  vel = 0;
  }

  else if (temperatura > 550){
  vel = 255;
  }

  else{

    vel = map(temperatura, 480, 550, 0, 255);
    Serial.print (temperatura);
    delay(100);

  }

  analogWrite (motor, vel);
  delay(100);

  
     
}
