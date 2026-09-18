# 2026-programacion-TP3
Ejercicios prácticos de Python sobre funciones, parámetros y el alcance de las variables globales.

# TP3 - Programación

Ejercicios de predicción de código sobre un tema que en la teoría suele pasar 
desapercibido: cómo funciona el alcance (scope) de las variables cuando el código 
está separado en varios archivos .py.

## De qué se trata

La mayoría de estos ejercicios parecen simples a primera vista (funciones, parámetros, 
variables globales), pero comparten una trampa en común: **una función solo puede 
acceder a las variables globales del módulo (archivo) donde fue definida, nunca a las 
de otro módulo**, aunque se importen con `from archivo import *`.

Cada ejercicio aborda esa idea desde un ángulo distinto, y en algunos casos el código 
directamente falla con `NameError` porque intenta acceder a una variable que existe, 
pero en otro archivo.

## Qué vas a encontrar

| Archivo | De qué trata |
|---|---|
| `ejercicio1301.txt` | Una función que intenta leer variables globales de otro módulo y falla. |
| `ejercicio1302.txt` | El mismo caso, pero pasando las variables como parámetro: acá sí funciona. |
| `ejercicio1303.txt` | Validación de un DNI contando dígitos, con una función que trabaja únicamente con lo que recibe por parámetro. |
| `ejercicio1304.txt` | Tres formas de calcular un promedio, comparando cuándo falla por depender de variables globales de otro módulo y cuándo funciona correctamente. |

Cada archivo tiene el código comentado línea por línea y, al final, una explicación 
paso a paso de cómo lo ejecuta el intérprete.

## Cómo clonarlo

Es necesario tener [Git](https://git-scm.com/) instalado. Desde una terminal:

\`\`\`bash
git clone https://github.com/kenyaC17/2026-programacion-TP3.git
\`\`\`

Esto crea una carpeta con todos los archivos en la computadora. No hace falta ejecutar 
nada, son archivos de texto con el análisis de cada ejercicio.