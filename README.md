# Reto Nro. 3
En este repo se encontrarán los diagramas de flujo y pseudocódigos asociados a cada problema planteado
## Numeros primos hasta n
### Diagrama de flujo 
```mermaid
graph TD
  A(Inicio)
  B[Número n]
  C[Lista i de 2 hasta n]
  D[Lista j de 2 hasta i^0.5+1]
  E{i % j es cero?}
  G[No es primo]
  H{Hay más números en j?}
  J[Es primo]
  K[Añadir a la lista]

  A --> B
  B --> C
  C --> D
  D -->|Sí| E
  E -->|Sí| G
  E -->|No| H
  H -->|Sí| E
  H -->|No| J
  J --> K
```
### Pseudocódigo 
```pseudocode
  Inicio

Leer n
Para i desde 2 hasta n hacer
    EncontrarDivisor = Verdadero
    Para j desde 2 hasta raíz cuadrada de i + 1 hacer
        Si el residuo de i dividido por j es igual a 0 entonces
            EncontrarDivisor = Falso
            Salir del bucle interno
        Fin Si
    Fin Para

    Si EncontrarDivisor es Verdadero entonces
        Añadir i a la lista de números primos
    Fin Si
Fin Para

Fin
```
## Procedimiento matemático para hallar raíces cuadradad
### Diagrama de flujo 
```mermaid

```
### Pseudocódigo
```pseudocode

```


