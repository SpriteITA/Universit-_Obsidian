```/*

La classe setup serve per:

1. inizializzare i pin mediante la funzione "pinmode([N.pin],[input/output])"

  
  

*/

  
  

void setup()

{

pinMode(13,OUTPUT);

}

  

//---------------------------------

  

/*

La classe loop è il corpo del programma ed uso funzioni come:

  

1. digitalWrite([numeroPin],[high/low]) --> questra istruzione mi permette di mandare un segnale in output. La funzione prende come riferimento un pin (dove mandare il segnale) seguito dal tipo di segnale

2. delay() --> questa funzione ritarda il program counter

  
  

*/

  
  

void loop()

{

digitalWrite(13,HIGH);

delay(1000); //1.000 ms --> 1 s

digitalWrite(13,LOW); //Non mandare più al pin

delay(1000);

}

  

//--------------------------------------
```