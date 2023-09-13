# Reto_3_Juan_Valderrama_CadaVezMasHacker

## Diagrama de flujo para saber si un número tiene raiz exacta o no:

```mermaid
graph TD

 AA[Número natural n] --> A(Lista del 0 a n-1) ---B
 B[b = número natural b sumado b-1 veces = a] --- 

  C{Diferencia de n-a=0?} 

    C-- SI --> E[La raiz de n es b] --- FIN
    C-- NO --> F{La diferencia de n-a < 0?} 


 F{Diferencia de n-a=0?}
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

