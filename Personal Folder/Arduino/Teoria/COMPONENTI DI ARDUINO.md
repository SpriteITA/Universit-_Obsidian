
==1 BreadBoard==

![[Pasted image 20260501142441.png]]


![[BreadoBoard.excalidraw]]

![[Pasted image 20260501145653.png]]


-------------------------------------------------------------------


==2. Resistenza==

![[Pasted image 20260501151547.png]]

La resistenza serve per ridurre la corrente così da evitare di bruciare i componenti. In queste diapositive userò come unità di misura Ω. La corrente che ne si ricava è il risultato di un rapporto:

`I = V/R`

Dove:

`1. I --> Corrente`     Ampere, A   --> ciò che arriva al componente   
`2. V --> Tensione`     Volt, V          --> che passa dal 5V di Arduino
`3. R --> Resistenza` Ohm, Ω        --> che metto nella BreadBoard



==CONCETTO MATEMATICO DELLE FORMULE FISICHE CHE SEGUONO LA STRUTTURA:==

`Qualcosa = effetto / ostacolo`

Mi son sempre chiesto del perché si usasse un rapporto per trovare una Grandezza.
Il motivo nasce per 3 fattori principali: (come due grandezze si influenzano)

1. Una differenza si fa SOLO su grandezze dello stesso tipo e si vuole vedere quanto uno dall'altra differiscono (lo da il risultato)
   
2. Un rapporto tra due grandezze invece nasce dal fatto che queste due nella realtà si influenzano...infatti 
	   2.1 La corrente è inversamente proporzionale alla resistenza (più la resistenza è importante e meno corrente passera)
	   2.2 La corrente è proporzionale alla tensione (più è grande la tensione maggiore sarà la resistenza)



Il valore di una resistenza si calcola così:
Es immagine --> [GIALLO], [VIOLA], [ROSSO], [ORO]
 -->  ((4.     x.    7.)      x.  100)    x.   5%.   -->  2.800 * 5% = +- 140 -->  ==2800 Ω ± 140 Ω==
![[Tabella colori resistenze.jpeg]]


N.B. LA TENSIONE SI DIVIDE TRA I COMPONENTI (perché OGNI componente consuma una sua tensione)

Che sostituendo alla formula diventa (mettendo un led):
B (BreadBoard)  = 5V
L (LED                 = necessita' di 2V
R (resistenza).   = 2800 

1. BreadBoard = 5V
2. LED --> B = B - L --> 3V sulla breadBoard
3. I = 3 / 2800 --> ≈ 0.00107 A ≈ ==1.07 mA==
   
==N.B. La resistenza permette di collegare due righe perché riesce a trasportare la tensione (ovviamente opponendone resistenza)==

==N.B. La resistenza deve avere entrambi i pin nella riga alimentata con la tensione==

-------------------------------------------------------------------

==3. LED==

![[led.excalidraw]]
==N.B.  Se io collego la breadBoard direttamente al 5V e al GND la breadBoard rimarrà sempre accesa perché Arduino non la controlla MA la sta solo alimentando==

---------------------------------------------------------------------