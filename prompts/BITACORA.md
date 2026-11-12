# Bitacora de prompts 
  
Laboratorio 06: Fundamentos de Ingenieria de Prompts. 
  
Herramienta de IA usada: (escribe aqui cual usaste) 
  
## Ejercicio 2: Tokens y ventana de contexto 
| Texto | Caracteres | Tokens | 
|-------|------------|--------| 
| Los estudiantes programan en Java. | 34| 7| 
| The students program in Java. | 6| 29| 
| desafortunadamente | 4| 18| 

  
## Ejercicio 3: Temperatura 

| Temperatura | % de BiblioTec | Nombres en los 5 intentos | 
|-------------|----------------|---------------------------| 
| 0 | 100%|BiblioTec, BiblioTec, BiblioTec, BiblioTec, BiblioTec | 
| 0.5 | 65%| BiblioTec, BiblioTec, BiblioTec, BiblioTec, BiblioTec| 
| 1 | 44%|BiblioTec, PrestaLibro, LibroYa, LibroYa, LectoGo | 
| 1.8 | 32.2%| BiblioTec, PrestaLibro, LibroYa, NubeDeTinta, BiblioTec| 

  
## Ejercicio 4: Prompt vago vs estructurado 

Al momento de preguntar en el mismo chat, la IA respondió correctamente lo que le pregunte, porque esa información estaba dentro del contexto de la conversación.
Al realizar la misma pregunta en un chat nuevo, la respondio que no sabia de que estaba hablando porque le faltaba el contexto.
  

  | Criterio | Prompt vago | Prompt estructurado | 
|----------|-------------|---------------------| 
| Menciona el objetivo del sistema | SI| SI| 
| Menciona a los usuarios principales | SI| SI| 
| Tiene exactamente 3 funcionalidades | NO| SI| 
| Esta en 3 parrafos | NO| SI| 
| Lo usaria en un informe real | NO| SI| 



## Ejercicio 5: Anatomia de un prompt 

Al momento de preguntar en el mismo chat, la IA respondió correctamente lo que le pregunte, porque esa información estaba dentro del contexto de la conversación.
Al realizar la misma pregunta en un chat nuevo, la respondio que no sabia de que estaba hablando porque le faltaba el contexto.
| Componente | Texto de mi prompt | 
|------------|--------------------| 
| Rol |La IA genera un código Java genérico y básico, sin saber exactamente qué construir ni cómo estructurarlo. | 
| Instruccion | El tono y enfoque técnico mejoran al asumir el papel de desarrollador Java, pero sigue siendo un programa genérico porque carece de un propósito específico.| 
| Contexto | La IA entiende que el programa debe resolver un problema real , por lo que empieza a proponer la lógica de inventario o la clase orientada a ese dominio| 
| Ejemplo |Se definen explícitamente los requerimientos técnicos | 
| Formato |Los métodos generados dentro de la clase adoptan estrictamente la convención de nomenclatura solicitada | 
