==1.1 Chiamate di Sistema e libreria==

Quando scriviamo codice possiamo utilizzare linee di codice appartenenti a delle librerie ==(Chiamate di libreria)== oppure potremmo usare codici a basso livello ==(chiamate di sistema)== 

Esempio chiamata di libreria:
`FILE *f = fopen("file.txt", "r");`

Esempio chiamata di sistema:
`int fd = open("file.txt", O_RDONLY);`

Il sistema operativo stesso restituisce valori di ritorno di errore per indicare che qualcosa non ha funzionato bene ! Ad esempio il valore di ritorno -1:

Es:

```
#include <fcntl.h>
#include <stdio.h>

int main() 
{
    int fd = open("file_che_non_esiste.txt", O_RDONLY);

    if (fd == -1) 
    {
        printf("Errore nell'apertura del file\n");
    }

    return 0;
}
```


Definisco adesso i concetti chiave:

1. `errno` ---> Variabile globale

2. ```
   ENOENT
   EPERM /* Numeri che indicano un errore */
   EINTR
	```

3. `sterror` ---> una funzione di libreria che ritorna una stringa di errore
   
   ---------------------------


Partiamo dai codici:

```
#include "stdio.h"

#include "stdlib.h"

#include "unistd.h"

  

/* definiamo questa macro per gestire in modo compatto gli errori: la metteremo,

* insieme ad altre, nella libreria ufficiosa `misc.h` */

#define exit_with_sys_err(s) \

{ \

perror((s)); \

exit(EXIT_FAILURE); \

}

  

void my_exit1(void) { printf("primo handler di uscita attivato!\n"); }

void my_exit2(void) { printf("secondo handler di uscita attivato!\n"); }

  

int main(int argc, char *argv[]) {

printf("avvio del programma...\n");

  

// programmiamo gli handler di uscita

if (atexit(my_exit2) != 0) {

// gestione standard degli errori: da ora in poi useremo la macro

perror("my_exit2");

exit(EXIT_FAILURE);

}

if (atexit(my_exit1) != 0)

exit_with_sys_err("my_exit1");

if (atexit(my_exit1) != 0)

exit_with_sys_err("my_exit1");

  

printf("aspetto un po'...\n");

sleep(3);

  

printf("chiudo il processo...\n");

  

exit(EXIT_SUCCESS); // gli handler vengono eseguiti automaticamente

}
```
   
   
   