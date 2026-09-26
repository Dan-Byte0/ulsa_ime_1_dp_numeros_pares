# Práctica 2: Guardar los números pares
## 1. Descripción del problema (Fase 1)
<!-- Explica con tus palabras qué hace tu programa y para qué serviría en la vida real. Máximo 4 líneas. -->

___El programa se encargara de primero recibir números y tomar en cuenta solamente los números pares, descartando los impares, esto en la vida real seriviria para clasificar información en sistemas automatizados__

## 2. Entradas y salidas (Fase 1)
<!-- Define cada entrada y cada salida, con su tipo de dato y su objetivo. -->

**Entradas:**
1. __Los 5 numeros, objetivo es saber cuales son mis 5 numeros ___

**Salidas:**
1. __De los 5 numeros, solamente los pares en un indice, objetivo es el cumplir la función del programa___
2. _____

## 3. Restricciones e invariante (Fase 1 y 2)

**Restricciones** (¿qué debe cumplirse?):
- __Que se descarten los numeros impares y solo cuenten los pares___
- _____

**Tamaño del arreglo y por qué** (piensa en el peor caso):
__Con un indice del 0 al 4, que son 5 lugares, así porque solo usare 5 numeros___

**¿El 0 y los negativos son pares? ¿Por qué?**
__Sí, porque se pueden dividir entre dos, el 0 puede y varios negativos pueden___

**Invariante** (¿qué es verdad después de cada vuelta del ciclo?):
___Que habran numeros pares __

## 4. Casos resueltos a mano (Fase 1)

| Caso | Números | Pares guardados | Posición de cada par |
|---|---|---|---|
| 1 | 3, 8, 5, 2, 7 | __3, 8___ | _0, 1____ |
| 2 | __2, 8, 5, 9, 12___ | __2, 8, 12___ | __0, 1, 2___ |
| 3 | _1, 6, 4, 7, 3____ | __6, 4___ | __0, 1___ |

## 5. Receta en pseudocódigo (Fase 2)
<!-- Tu receta va en el archivo RECETA.md. Aquí solo responde las dos preguntas. -->

**¿Probé mi receta a mano con un caso?** Sí 
**¿Tuve que corregirla?** ___No, solo concluirla__

## 6. Cómo compilar y ejecutar (Fase 3)

```bash
g++ -Wall -Wextra -std=c++17 main.cpp -o numeros_pares
./numeros_pares
```

## 7. Ejemplo de ejecución (Fase 3)
<!-- Pega aquí lo que muestra tu programa en pantalla con un caso normal. -->

```
__Guardar los numeros pares de 5 numeros
Escribe un numero: 3
Escribe un numero: 8
Escribe un numero: 5
Escribe un numero: 6
Escribe un numero: 7
Se guardaron 2 numeros pares
8
6___
```

## 8. Experimentos (Fase 3)

**Experimento A: ¿qué apareció al imprimir las 5 posiciones del arreglo? ¿Por qué?**
_____

**Experimento B: ¿qué pasó al usar la variable del ciclo como posición del arreglo? ¿Por qué?**
_____

## 9. Tabla de pruebas (Fase 4)

| Caso | Números | Esperado | Obtenido | ¿Pasó? |
|---|---|---|---|---|
| Mezcla | 1, 2, 3, 4, 5 | 2 pares: 2, 4 | __2,4___ | ___Se ejecuto y me mostro el 2 y el 4 __ |
| Posiciones distintas | 3, 8, 5, 2, 7 | 2 pares: 8, 2 | __8,2___ | __Se ejecuto correctamente y me mostro el 8 y el 2___ |
| Todos pares | 2, 4, 6, 8, 10 | 5 pares | ___Los 5 pares__ | __Se ejecuto correctamente y me mostro los 5 pares sin problema___ |
| Todos impares | 1, 3, 5, 7, 9 | 0 pares | __ningun par___ | __Se ejecuto correctamente y no me mostro ningun par___ |
| Con cero y negativos | 0, -3, -4, 7, 1 | 2 pares: 0, -4 | __0,-4___ | __Se ejecuto correctamente y me mostro dos pares___ |
| Entrada inválida | `hola` o `3.5` | vuelve a pedir | __Entrada no valida___ | __Se ejectuto correctamente y me mostro que es invalido___ |
| Caso propio 1 | __Signo de expresión___ | __!12___ | __Invalido___ | __Se ejecuto correctamente y no detecta ningun numero___ |
| Caso propio 2 | __Signo de expresión___ | ___?15__ | ___Invalido__ | ___Se ejecuto correctamente y no detecta ningun numero__ |

## 10. Bitácora de mejoras (Fase 4)

| # | ¿Qué falló o qué quise mejorar? | ¿Qué cambié? | ¿Funcionó? |
|---|---|---|---|
| 1 | __No hubo nada en especifico que mejoraria, no conozco formas de mejorarla___ | ___Nada__ | ___No__ |
| 2 | _____ | _____ | _____ |

**Reto elegido (opcional):** _____

## 11. Dudas para el profesor (Fase 3)

| Duda | Lo que ya intenté |
|---|---|
| __No comprendi la sección 8, ninguno de los dos experimentos___ | __Lo revise con IA pero no comprendi, si lo podemos checar en clase porfavor___ |

## 12. Reflexión final

**¿Qué aprendí con esta práctica?**
__Aprendi a saber mas como anotar variables ___

**Ahora que terminé, ¿qué cambiaría de mi proceso?**
__Nada___

**¿Qué fue lo más difícil y cómo lo resolví?**
___Mi ciclo, lo resolvi con una guia con IA, no me la regalo, yo quiero aprender, me iba explicando y preguntando variables y comandos __

**¿Qué pregunta me quedó sin responder?**
__Ninguna___

**¿Por qué no puedo usar la variable del ciclo para guardar en el arreglo?**
___Porque i solo cuenta vueltas del ciclo si la uso pa guardar qudaria todo disperso, pero totalPares solo avanza si hay un par guardado, lo deja en la posición 0 y ya va avanzando.__

## 13. Lista de verificación antes de entregar (Fase 5)

- [ ] Llené todas las secciones (no quedan `_____`)
- [ ] Mi programa compila sin advertencias
- [ ] Probé todos los casos de la tabla
- [ ] Hice los Experimentos A y B y dejé el código correcto al terminar
- [ ] No modifiqué `utilerias.h`
- [ ] Hice al menos 3 commits con mensajes claros
- [ ] Hice `git push` y verifiqué mi fork en GitHub
- [ ] Entregué el enlace de mi fork en Classroom