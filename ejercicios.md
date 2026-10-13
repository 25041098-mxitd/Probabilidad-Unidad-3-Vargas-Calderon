## Ejercicio 1: Investigador biomédico
Un investigador biomédico realiza un conteo del número de células anormales observadas en una muestra de tejido tomada de distintos pacientes. La variable aleatoria X representa el número de células anormales encontradas en una muestra seleccionada al azar de una lámina.

**1. Verificación de suma de probabilidades:**
Para que sea una distribución de probabilidad válida, la suma de todas las probabilidades debe ser igual a 1.
0.10 + 0.25 + 0.30 + 0.20 + 0.10 + 0.05 = 1.00

**2. Distribución de probabilidad de X:**
A partir de las observaciones previas estimadas, la distribución es la siguiente:

| Número de células anormales (x) | 0 | 1 | 2 | 3 | 4 | 5 |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| **Probabilidad P(X)** | 0.10 | 0.25 | 0.30 | 0.20 | 0.10 | 0.05 |

*Gráfica de distribución de probabilidad:*
```text
  0 | ██ (0.10)
  1 | █████ (0.25)
  2 | ██████ (0.30)
  3 | ████ (0.20)
  4 | ██ (0.10)
  5 | █ (0.05)
```

**3. Cálculos de Valor Esperado, Varianza y Desviación Estándar:**
*   **Valor esperado E(X) (promedio de células anormales por muestra):**
    E(X) = Σ [xi · P(xi)]
    E(X) = (0)(0.10) + (1)(0.25) + (2)(0.30) + (3)(0.20) + (4)(0.10) + (5)(0.05)
    E(X) = 0 + 0.25 + 0.60 + 0.60 + 0.40 + 0.25 = 2.10

*   **Varianza Var(X) y Desviación Estándar σ:**
    Primero calculamos E(X²):
    E(X²) = (0²)(0.10) + (1²)(0.25) + (2²)(0.30) + (3²)(0.20) + (4²)(0.10) + (5²)(0.05)
    E(X²) = 0 + 0.25 + 1.20 + 1.80 + 1.60 + 1.25 = 6.10
    
    Ahora aplicamos la fórmula de la varianza:
    Var(X) = E(X²) - [E(X)]²
    Var(X) = 6.10 - (2.10)² = 6.10 - 4.41 = 1.69
    
    Desviación estándar:
    σ = √1.69 = 1.30

**4. Función de distribución acumulada F(x):**

| x | P(X ≤ x) | F(x) |
| :--- | :--- | :--- |
| 0 | 0.10 | **0.10** |
| 1 | 0.10 + 0.25 | **0.35** |
| 2 | 0.35 + 0.30 | **0.65** |
| 3 | 0.65 + 0.20 | **0.85** |
| 4 | 0.85 + 0.10 | **0.95** |
| 5 | 0.95 + 0.05 | **1.00** |

*Gráfica de la función acumulada F(x)*
```text
  1.0 | ------------------------------------- ● (1.00)
  0.8 |                             ┌───────┘
  0.6 |                     ┌───────┘ (0.65)
  0.4 |             ┌───────┘ (0.35)
  0.2 |     ┌───────┘
  0.0 | ●───┘ (0.10)
      +--------------------------------------
        0       1       2       3       4       5
```

**5. Interpretación de resultados en contexto biomédico:**
*   **Promedio esperado:** Se espera encontrar un promedio de 2.1 células anormales por muestra analizada.
*   **Variabilidad:** La desviación estándar de 1.30 indica que existe una variabilidad moderada; la mayoría de las muestras contendrán entre 0.8 y 3.4 células anormales (media ± 1 desviación estándar).
*   **Función acumulada:** El F(2) = 0.65 nos indica que hay un 65% de probabilidad de encontrar 2 o menos células anormales en una muestra, mientras que la probabilidad de encontrar un número alto (4 o 5) es bastante baja (solo el 15% restante).

*   ---

## Ejercicio 2: Boletos
En una tómbola se colocan boletos con distintos premios.

**1. Verificación de suma de probabilidades:**
0.50 + 0.30 + 0.15 + 0.05 = 1.00

**2. Distribución de probabilidad de X:**

| Premio (X) Monto (pesos) | 0 (A) | 10 (B) | 20 (C) | 50 (D) |
| :--- | :--- | :--- | :--- | :--- |
| **Probabilidad P(X)** | 0.50 | 0.30 | 0.15 | 0.05 |
*Gráfica de distribución de probabilidad:*
```text
  $0  | ██████████ (0.50)
  $10 | ██████ (0.30)
  $20 | ███ (0.15)
  $50 | █ (0.05)
```
**3. Cálculos de Valor Esperado, Varianza y Desviación Estándar:**
*   **Valor esperado E(X) (ganancia promedio esperada):**
    E(X) = (0)(0.50) + (10)(0.30) + (20)(0.15) + (50)(0.05)
    E(X) = 0 + 3.00 + 3.00 + 2.50 = 8.50 pesos

*   **Varianza y Desviación Estándar:**
    E(X²) = (0²)(0.50) + (10²)(0.30) + (20²)(0.15) + (50²)(0.05)
    E(X²) = 0 + (100)(0.30) + (400)(0.15) + (2500)(0.05)
    E(X²) = 0 + 30 + 60 + 125 = 215
    
    Var(X) = 215 - (8.50)² = 215 - 72.25 = 142.75
    
    σ = √142.75 = 11.95 pesos

**4. Función de distribución acumulada F(x):**

| Monto (x) | P(X ≤ x) | F(x) |
| :--- | :--- | :--- |
| 0 | 0.50 | **0.50** |
| 10 | 0.50 + 0.30 | **0.80** |
| 20 | 0.80 + 0.15 | **0.95** |
| 50 | 0.95 + 0.05 | **1.00** |
*Gráfica de la función acumulada F(x)*
```text
  1.0 | ------------------------------------- ● (1.00)
  0.8 |                             ┌───────┘ (0.80)
  0.6 |                     ┌───────┘
  0.4 |             ┌───────┘ 
  0.2 |     ┌───────┘ 
  0.0 | ●───┘ (0.50)
      +--------------------------------------
        $0      $10     $20             $50
```

**5. Interpretación de resultados:**
*   **Valor esperado:** El monto de 8.50 pesos significa que si una persona jugara a esta tómbola muchísimas veces, en promedio ganaría 8.50 pesos por boleto.
*   **¿Es favorable el juego?:** Para determinar si el juego es favorable para el jugador, se debe comparar este valor esperado (8.50 pesos) con el costo del boleto. Si el boleto cuesta más de 8.50 pesos, el juego representa una pérdida esperada a largo plazo y no es matemáticamente favorable.

---

## Ejercicio 3: Tienda
Una tienda registra la cantidad de unidades de cierto producto vendidas por semana. La variable X representa el número de artículos vendidos, con una distribución basada en observaciones pasadas.

**1. Verificación de suma de probabilidades:**
0.05 + 0.10 + 0.25 + 0.30 + 0.20 + 0.10 = 1.00

**2. Distribución de probabilidad de X:**

| Unidades vendidas (X) | 0 | 1 | 2 | 3 | 4 | 5 |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| **Probabilidad P(X)** | 0.05 | 0.10 | 0.25 | 0.30 | 0.20 | 0.10 |
*Gráfica de distribución de probabilidad:*
```text
  0 | █ (0.05)
  1 | ██ (0.10)
  2 | █████ (0.25)
  3 | ██████ (0.30)
  4 | ████ (0.20)
  5 | ██ (0.10)
```

**3. Cálculos de Valor Esperado, Varianza y Desviación Estándar:**
*   **Valor esperado E(X) (número promedio de ventas):**
    E(X) = (0)(0.05) + (1)(0.10) + (2)(0.25) + (3)(0.30) + (4)(0.20) + (5)(0.10)
    E(X) = 0 + 0.10 + 0.50 + 0.90 + 0.80 + 0.50 = 2.80 unidades

*   **Varianza y Desviación Estándar:**
    E(X²) = (0²)(0.05) + (1²)(0.10) + (2²)(0.25) + (3²)(0.30) + (4²)(0.20) + (5²)(0.10)
    E(X²) = 0 + 0.10 + 1.00 + 2.70 + 3.20 + 2.50 = 9.50
    
    Var(X) = 9.50 - (2.80)² = 9.50 - 7.84 = 1.66
    
    σ = √1.66 = 1.29 unidades

**4. Función de distribución acumulada F(x):**

| x | P(X ≤ x) | F(x) |
| :--- | :--- | :--- |
| 0 | 0.05 | **0.05** |
| 1 | 0.05 + 0.10 | **0.15** |
| 2 | 0.15 + 0.25 | **0.40** |
| 3 | 0.40 + 0.30 | **0.70** |
| 4 | 0.70 + 0.20 | **0.90** |
| 5 | 0.90 + 0.10 | **1.00** |

*Gráfica de la función acumulada F(x)*
```text
  1.0 | ------------------------------------- ● (1.00)
  0.8 |                             ┌───────┘ (0.90)
  0.6 |                     ┌───────┘ (0.70)
  0.4 |             ┌───────┘ (0.40)
  0.2 |     ┌───────┘ 
  0.0 | ●───┘ (0.05)
      +--------------------------------------
        0       1       2       3       4       5
```

**5. Interpretación de resultados:**
*   **Ventas esperadas:** Se espera vender un promedio de 2.80 unidades por semana.
*   **Estabilidad de la demanda:** Con una desviación estándar de 1.29, la demanda muestra una variabilidad moderada. El volumen principal de ventas esperadas se ubicará casi siempre entre 1.51 y 4.09 unidades semanales, lo que sugiere que la tienda rara vez tendrá cero ventas o ventas máximas (5) y mantiene una demanda relativamente consistente alrededor de 3 artículos.
