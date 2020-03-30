# Guía rápida de Arduino

## 1. Estructura básuca de un programa
Tiene 2 funciones principales: **`setup()`** y **`setup()`**.
```c
int ledPin = 13; // declaraciones

/* inicializaciones */
void setup() {
  pinMode(ledPin, OUTPUT);    
}

/* Bucle principal del programa */
void loop() {
  digitalWrite(ledPin, HIGH); 
  delay(1000);                
  digitalWrite(ledPin, LOW);  
  delay(1000);                
}
```
## 2. Funciones
* **`pinMode(pin, modo)`**
Configura un pin para que sea de entrada o de salida.
Donde:

    * `pin`: es el número de pin
    * `modo`: indica si lo ponemos de **entrada** (`INPUT`), de **salida** (`OUTPUT`) o `INPUT_PULLUP`.


* **`digitalWrite(pin, valor)`**
Configura un pin para que sea de entrada o de salida.
Donde:

    * `pin`: es el número de pin
    * `valor`: valor que ponemos. Puede ser `HIGH`, o `LOW`.

* **`delay(ms)`**
Pausa el programa durante `ms` milisegundos.
Donde:

    * `ms`: número de milisegundos a esperar.