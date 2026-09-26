# Receta: Guardar los números pares

1. Mostrar mensaje de bienvenida
2. totalPares ← ___0___
3. contador ← ___0___
4. MIENTRAS contador ______ CANTIDAD HACER
       numero ← leerEntero("___Numeros enteros:___")
       SI numero ___%2==0___ ENTONCES
           pares[___totalPares___] ← numero
           totalPares ← ____totalPares + 1__
       FIN SI
       contador ← ___contador+1___
   FIN MIENTRAS
5. Mostrar "Pares encontrados: " + totalPares ___
Mostrar "Valores:"
6. i ← 0
7. MIENTRAS i ______<totalPares ______ HACER
       Mostrar pares[i]
       i ← ___i+1___
   FIN MIENTRAS