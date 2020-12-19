void setup() {
  pinMode(A5,INPUT_PULLUP);
  pinMode(12,INPUT);
  pinMode(13,OUTPUT);
}

void loop() {
  
  boolean button1 = !digitalRead(A5); //  ! - инвертирует сигнал полученный с кнопки
  
  if (buttom1 == 1) digitalWrite(13,1);
  else digitalWrite(13,0);

}   // включает 13ый пин ()встроенный светодиод при нажатии кнопки подключенной к пину А5 (кнопк gnd + А5)   https://youtu.be/3UwgMAdV4xQ







boolean bf = 0;
boolean bb;
boolean lf = 0;

unsigned long last_pressed;

void setup() {
  pinMode(3, INPUT_PULLUP);
  pinMode(13,OUTPUT);

}

void loop() {
  bb = !digitalRead(3); 
  if (bb == 1 && bf == 0 && millis() - last_pressed > 50 ) {
    bf = 1;
    
    lf = !lf;
    digitalWrite(13,lf);
    last_pressed = millis();
  }
  if (bb == 0 && bf == 1) {
    bf = 0;
  }
}  // оставляет включенным/выключенным после нажатия кнопки
