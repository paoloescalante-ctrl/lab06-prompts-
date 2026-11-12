# Tarea: Mi prompt profesional

## Funcionalidad elegida

Calculo de notas: un programa que recibe las notas de un estudiante y calcula su promedio final.

## Version 1: prompt basico
Le dije a la IA que crear un programa que calcule notas en java.
## Version 1: prompt basico

```text
Hazme un programa para calcular notas.
```

| Aspecto | Descripcion |
|---------|-------------|
| Que cambie | Nada al ser el punto de partida. Escribi el pedido de la forma mas simple posible. |
| Por que | Para ver como responde la IA cuando tiene que adivinar todo. |
| Que paso en la respuesta | La IA por su cuenta asumio 3 notas con el mismo peso. Invento una nota minima aprobatoria de 11 y no valido que las notas esten entre 0 y 20. Dejo todo el codigo en un solo metodo main. Agrego un ejemplo de ejecucion, una lista de conceptos y una oferta final que no pedi, asi que el formato fue impredecible. |

## Version 2
Ahora le pedi algo mas estructurado:

Actua como desarrollador Java. Crea un programa de consola en Java para calcular el promedio final de un estudiante universitario. El estudiante tiene tres notas: practicas (30%), examen parcial (30%) y examen final (40%). La escala es de 0 a 20 y la nota minima aprobatoria es 11. El programa debe validar que cada nota este entre 0 y 20, y mostrar el promedio final y si el estudiante aprobo o desaprobo.

| Aspecto | Descripcion |
|---------|-------------|
| Que cambie | Agregue un rol, el contexto de las tres notas con sus porcentajes, escala de 0 a 20 y nota minima de 11, e instrucciones mas especificas  |
| Por que | En la v1 la IA tuvo que adivinar el lenguaje, los pesos, la escala y la nota minima. Ahora esos datos se los doy yo. |
| Que mejoro en la respuesta | Uso los pesos correctos (30%, 30% y 40%), respeto la escala y la nota minima de 11, y valido que las notas esten entre 0 y 20. Ya no invento datos. Sin embargo, dejo todo el codigo en un solo main, no volvio a pedir la nota cuando era invalida y agrego secciones que no pedi (explicacion, formula, ejemplo, condiciones y recomendacion), por lo que el formato seguia sin controlarlo yo. 

## Version 3: prompt final

Ahora fui mucho mas exacto con lo que queria y como lo queria:

Actua como desarrollador Java con experiencia en ensenanza universitaria. Crea un programa de consola en Java que calcule el promedio final de un estudiante.

Contexto: el estudiante tiene tres notas: practicas (30%), examen parcial (30%) y examen final (40%). La escala es de 0 a 20 y la nota minima aprobatoria es 11. Si una nota esta fuera del rango de 0 a 20, el programa debe volver a pedirla.

Organiza el codigo en metodos separados, con este estilo: leerNota(String nombre) y calcularPromedio(double practicas, double parcial, double examenFinal).

Ejemplo de salida esperada con practicas 15, parcial 12 y final 16:
Promedio final: 14.50
Estado: APROBADO

Formato: primero explica la estructura del programa en maximo 3 lineas y luego presenta el codigo completo en un solo bloque. No agregues nada mas.


| Aspecto | Descripcion |
|---------|-------------|
| Que cambie | Complete el rol (agregue experiencia en ensenanza universitaria), agregue en el contexto que se vuelva a pedir la nota si es invalida, pedi metodos separados con nombres concretos, incluí un ejemplo de salida y defini el formato de la respuesta (explicacion de maximo 3 lineas y un solo bloque de codigo). |
| Por que | En la v2 el codigo quedo en un solo main, no volvia a pedir la nota invalida y la IA agrego secciones que no pedi. Con el ejemplo y el formato reduzco lo que la IA tiene que decidir sola. |
| Que mejoro en la respuesta | Separo el codigo en leerNota, calcularPromedio y main con los nombres pedidos. La nota invalida se vuelve a pedir con un ciclo do-while. La explicacion fue breve y el codigo vino en un solo bloque, sin ejemplos ni listas extra. La salida final tiene el formato del ejemplo (Promedio final y Estado). |

## Componentes del prompt final

| Componente | Texto de mi prompt |
|------------|--------------------|
| Rol | Actua como desarrollador Java con experiencia en ensenanza universitaria. |
| Instruccion | Crea un programa de consola en Java que calcule el promedio final de un estudiante. |
| Contexto | El estudiante tiene tres notas: practicas (30%), examen parcial (30%) y examen final (40%). La escala es de 0 a 20 y la nota minima aprobatoria es 11. Si una nota esta fuera del rango de 0 a 20, el programa debe volver a pedirla. |
| Ejemplo | Organiza el codigo en metodos separados, con este estilo: leerNota(String nombre) y calcularPromedio(double practicas, double parcial, double examenFinal). Ejemplo de salida esperada con practicas 15, parcial 12 y final 16: Promedio final: 14.50 / Estado: APROBADO |
| Formato | Primero explica la estructura del programa en maximo 3 lineas y luego presenta el codigo completo en un solo bloque. No agregues nada mas. |

## Evaluacion del resultado

| Criterio | Cumple |
|----------|--------|
| Usa los pesos correctos (30%, 30% y 40%) | Si |
| Valida el rango de 0 a 20 y vuelve a pedir la nota invalida | Si |
| Separa el codigo en metodos con los nombres pedidos (leerNota y calcularPromedio) | Si |
| Explica la estructura en maximo 3 lineas | Si |
| Entrega el codigo en un solo bloque, sin agregar secciones extra | Si |
| La salida respeta el formato del ejemplo (Promedio final y Estado) | Si |
| Maneja entradas que no son numeros (por ejemplo, letras) sin fallar | No |

**Observacion:** el unico criterio que no se cumple es el manejo de letras en lugar de numeros. No lo pedi en el prompt, asi que una proxima version podria agregarlo.

## Errores que evite

| Error frecuente | Como lo evite |
|-----------------|---------------|
| Asumir informacion no proporcionada | En la v1 la IA invento el lenguaje, la cantidad de notas, los pesos y la nota minima. En la v3 yo di todos esos datos en el contexto (tres notas, 30/30/40, escala de 0 a 20 y nota minima de 11), asi que no tuvo que adivinar. |

