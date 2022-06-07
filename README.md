# a
REGADO ARDUINO

void setup() {
  // usamos el pin 13 como salida, para activar y desactivar el rel
  pinMode(LED_BUILTIN, OUTPUT);
}


void loop() {
  digitalWrite(LED_BUILTIN, HIGH);   // encendemos la bomba.      Se puede dar más tiempo dependiendo las pruebas
  delay(5000);                       // esperamos 5 segundo.
  digitalWrite(LED_BUILTIN, LOW);    // apagamos la bomba.  
  delay(60000);                       // esperamos un minuto y empieza el loop de nuevo.
