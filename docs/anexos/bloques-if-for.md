# Anexo: Guía Rápida de Lógica en MATLAB®

Esta guía explica cómo "enseñarle" a MATLAB® a tomar decisiones y a repetir tareas automáticamente. 

---

## 1. El Bloque if

Imagina que el `if` es un **filtro**. El código solo pasará por ese filtro si la condición que pusiste es verdadera.

### Sintaxis Básica
```matlab
if condicion
    % Este código es como un "área VIP"
    % Solo se entra si la condición se cumple (es 1 o true)
end
```

### El camino alternativo: else
Si la condición no se cumple, puedes decirle a MATLAB® que tome otro camino usando `else` (que significa "si no...").

```matlab
if condicion
    % Opción A: Se cumple
else
    % Opción B: NO se cumplió la condición
end
```

### Ejemplo para entenderlo mejor:
Imagina que estás programando un sensor de riego:
```matlab
humedad = 15; % Porcentaje de humedad en la tierra

if humedad < 20
    disp('La tierra está seca. ¡Prender el agua!');
else
    disp('Hay suficiente humedad. Mantener apagado.');
end
```



---

## 2. El Bucle for (Repetir código sin copiar y pegar)

Un bucle `for` se usa cuando tienes que hacer lo mismo muchas veces. En lugar de escribir 100 líneas de código iguales, escribes una que se repita 100 veces.

### ¿Cómo funciona?
Usa una variable (normalmente llamada `i` o `n`) que funciona como un **contador**.

```matlab
for i = 1:5
    % Lo que escribas aquí se repetirá 5 veces.
    % En la vuelta 1, i vale 1.
    % En la vuelta 2, i vale 2... y así hasta llegar a 5.
end
```

### Ejemplo práctico:
Si quieres imprimir la tabla del 5:
```matlab
for i = 1:10
    resultado = 5 * i;
    disp(resultado);
end
```



---

## 3. Operadores Lógicos

Para que el `if` funcione, debes saber cómo comparar valores. Aquí están los símbolos que MATLAB® entiende:

| Símbolo | Significado | ¿Cómo se lee? |
| :--- | :--- | :--- |
| `==` | Igualdad | ¿Es X exactamente igual a Y? |
| `~=` | Diferencia | ¿Es X distinto de Y? |
| `>` / `<` | Mayor / Menor | ¿Es X más grande o más chico que Y? |
| `&` | "Y" (AND) | Se tiene que cumplir la condición 1 **Y** la 2. |
| `\|` | "O" (OR) | Se tiene que cumplir la 1 **O** la 2 (cualquiera sirve). |

---

## 💡 Consejos

* **El Cierre Eterno:** Cada bloque `if` o `for` es como una caja. Si la abres, tienes que cerrarla con un `end`. *Si te falta uno solo, el programa fallará.*
* **La Sangría (Indentación):** Nota que el código dentro del `if` o `for` está un poco más a la derecha. Eso se hace con la tecla **Tab** (arriba de Bloq Mayús) y sirve para que tú y otras personas puedan leer el código sin marearse.
* **Higiene:** Usa el punto y coma (`;`) al final de las operaciones dentro de un `for` para que MATLAB® no te llene la pantalla de números cada vez que da una vuelta.

---
***Material de apoyo para el Workshop de MATLAB® - IEEE PES UdeC***