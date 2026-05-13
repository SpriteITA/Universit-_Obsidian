Sostanzialmente per conoscere il concetto di applicazione lineare bisogna avere la conoscenza pregressa di sapere:

1. Cos'è uno spazio vettoriale ?  
   1 Uno spazio vettoriale (indicato con )
   
3. Cos'è un vettore e quali operazioni si possono fare ?
4. Come si definisce formalmente un vettore di R^x componenti ? (combinazione lineare e base canonica)
5. Applicazione tra spazi vettoriali --> funzione che prende in input un vettore e ne restituisce un'altro  `f:R3→R4`
6. Quali proprietà deve rispettare un'applicazione `f` per essere lineare ? (1° Somma e 2° Prodotto per scalare)
7. 
   






   ![[1.png]]
   
   
   Sostanzialmente per fare l'esercizio mi giovano queste due regole:
   
   ![[Pasted image 20260504154210.png]]
   
   ![[Pasted image 20260504154247.png]]
   
   E si arriva poi allo svolgimento di questo esercizio:
   ![[Pasted image 20260504154403.png]]

![[Pasted image 20260504161850.png]]


==N.B.== Questi f($e_n$ ) si chiamano  ==Immagini dei vettori della base canonica==

![[Pasted image 20260509222808.png]]

==N.B.== Ricordati ==matrice Associata==

![[Pasted image 20260509225716.png]]


ADESSO CHE SI E' COSTRUITA LA MATRICE ASSOCIATA SI VUOLE TROVARE:

1. RANGO DELLA MATRICE
2. RISOLVERE SISTEMI
3. TROVARE KERNEL
4. STUDIARE INDIPENDENZA LINEARE
5. LA DIMENSIONE DELL'IMMAGINE
6. NUCLE0
   
PER TROVARLI SU USANO DIVERSI ALGORITMI...COME LA RISOLUZIONE DI GAUSS !


------------------------------

==ALGORITMO DI GAUSS SULLA RIDUZIONE DI UNA MATRICE:==

1. Il Primo step è quello di conoscere il significato di ==PIVOT== (che corrispondono alla diagonale principale)
![[Excalidraw/Drawing 2026-05-09 22.53.04.excalidraw]]



2. Conoscendo questo adesso è possibile ==DEFINIRE LE REGOLE==:
   
   2.1 SCAMBIO DI RIGHE:   R$_i$ <-> R$_i$	![[Pasted image 20260509231242.png]]
    2.2 MOLTIPLICARE UNA RIGA PER UNO SCALARE: R$_i$ <- ƛR$_i$
    
    ![[Pasted image 20260509231604.png]] 
    2.3 Sommare a una riga un multiplo di un’altra R$_i$ <- R$_i$ + ƛR$_i$
    
    ![[Pasted image 20260511161356.png]]
    
    ==ALGORITMO DI GAUSS  STEP BY STEP==
    
    ![[Pasted image 20260511161539.png]]
    
    



-----------------------------------------------




==RANGO DELLA MATRICE + DIMENSIONE IMMAGINE==

![[Pasted image 20260511191841.png]]


==EQUAZIONI CARTESIANE== 

![[Pasted image 20260511193926.png]]


![[Pasted image 20260511195001.png]]