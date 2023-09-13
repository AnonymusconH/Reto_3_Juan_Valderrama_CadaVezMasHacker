# Reto_3_Juan_Valderrama_CadaVezMasHacker

## Diagrama de flujo para saber si un número tiene raiz exacta o no:

```mermaid

graph TD

 AA[Número natural n] --> A(Lista del 0 a n-1) ---B
 B[b = número natural b sumado b-1 veces = a] --- 

  C{¿Diferencia de n-a=0?} 

    C-- SI --> E[La raiz de n es b] --- FIN
    C-- NO --> F{La diferencia de n-a < 0?} 


 F{¿Diferencia de n-a=0?}
 F-- SI --> H[n NO tiene raiz exacta] --- FIN
F-- NO --> J[Entonces b= b+1] --->B

FIN

```

## Ahora, su pseudocódigo quedaria de la siguiente forma.

```

n: Número natural
b: Número natural
a: Número natural

  Escribir ("Ingrese su primer número)
    Leer n

b: Suma de b-1 veces
a: Suma de b-1 veces

  Escribir ("Ingrese su segundo número)
    Leer a

Inicio
Si modulo (n-a = 0) entonces
  Escribir ("La raiz de n es b")

Sino
  si modulo (n-a < 0) entonces
    Escribir (" n NO tiene raiz exacta)

Sino
  b= b+1
    Fin mientras
FIN

```



## Diagrama de flujo para saber si un número es primo o no:

```mermaid
graph TD

 AA[Número natural n] -->B
 AA[Número natural n] -->C
  


AA ---D
 B{¿Su número es un 1?}

 B ---|SI| BA[Entonces su número no es primo]
 
 C{¿Su número es un 2?}

  ---|SI| BB[Entonces su número  es primo]

D[Número natural: X : X menos igual a n ] --- E{¿El residuo de n dividio X es 0?}
E ---|SI|F{n es igual a X?}---|SI| G{n o X son pares?} ---|SI| H[n NO es un número primo]

      
G ---|NO| I{El residuo de n dividio X sigue siendo 0} --- |SI| J[n es un numero primo] 
I{El residuo de n dividio X sigue siendo 0} --- |NO| H

E --- |NO|K[n NO es un número primo]

```

## Y con su respectivo Pseudocódigo quedaria asi:

```

n: Número natural
X: Número natural
X: X</n

Inicio

Inserte n
 leer n

Si
 n: 1 Entonces
  Escrbir("1 No es un número primo)
    Fin mientras
 n:2 Entonces
  Escribir ("2 No es un número primo)
fin mientras

Sino
 si modulo ( n & X = 0)
  mientras n = X and pertenezcan al conjunto de los pares (2n) entonces
   Escribir ("n No es un número primo)
fin mientras

Sino
 si modulo ( n % X = 0) Entonces
  Escribir ("n es un número primo)
fin mientras

Fin

```

## Gracias tkm
 



