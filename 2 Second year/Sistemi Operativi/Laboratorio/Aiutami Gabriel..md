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

3. `sterror` ---> una funzione di libreria che re
   