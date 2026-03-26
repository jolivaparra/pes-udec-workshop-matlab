# 🚀 Hoja de Trucos (Cheatsheet): MATLAB® Workshop PES

Este es un resumen de comandos rápidos para usar durante y después del taller. 

---

## 1. Configuración y Limpieza
Comandos para "limpiar la mesa" antes de empezar un programa:
* `clc`: Borra el texto de la Ventana de Comandos.
* `clear`: Borra todas las variables de la memoria (Workspace).
* `;`: Silenciador. Se pone al final de una línea para que MATLAB® no sature la pantalla con resultados.
* `%`: Comentarios. Todo lo que escribas después de esto es una nota para ti y MATLAB® no lo ejecuta.

---

## 2. Creación de Arreglos
En MATLAB®, todo es un arreglo (colección de números).
* **Manual:** Usa `[ ]` y separa con comas/espacios para filas, o punto y coma (`;`) para saltar de fila.
* **Operador de dos puntos:** `inicio : paso : fin` (Ej: `0:2:10` genera 0, 2, 4, 6, 8, 10).
* **Linspace:** `linspace(inicio, fin, num_puntos)` (Se usa cuando sabes cuántos datos quieres en total).
* **Funciones de llenado:**
    * `zeros(f, c)`: Matriz llena de ceros.
    * `ones(f, c)`: Matriz llena de unos.
    * `rand(f, c)`: Matriz con números aleatorios entre 0 y 1.

---

## 3. Operaciones de Ingeniería (Elemento a elemento)
Para aplicar fórmulas matemáticas a listas de datos (como sensores), usa siempre el **punto**:
* Multiplicación: `.*` 
* División: `./` 
* Potencia: `.^` 
> **Regla de oro:** Si sumas o restas no necesitas punto, pero si multiplicas o elevas a potencia, ¡pon el punto!.

---

## 4. Indexación y Máscaras
Acceder a la información dentro de los arreglos.
* **Índices:** `A(1)` es el primer elemento (MATLAB® cuenta desde 1).
* **Último:** `A(end)` siempre apunta al final del vector.
* **Recortes:** `A(2:5)` extrae desde la posición 2 a la 5. 
* **Recortes (2):** `A(2:3:15)` extrae desde la posición 2 a la 15 saltando de a 3. 
* **Recortes (3):** `Matriz(3, :)` extrae toda la tercera fila. 
* **Máscaras Lógicas:** Creas un "mapa" de verdaderos/falsos con preguntas como `==`, `<`, `>` o combinando con `&` (Y) y `|` (O).
* **Filtrado:** `datos(datos < 100)` extrae solo los valores que cumplen la condición.



---

## 5. Datos y Gráficos
Para procesar archivos y visualizar resultados.
* **Importar:** `T = readtable('archivo.csv')`.
* **Sacar columna:** `variable = T.NombreColumna` (Operador punto).
* **Graficar:** `plot(x, y)`.
* **Control:**
    * `hold on`: Para dibujar más de una línea en la misma ventana.
    * `xlim/ylim`: Para controlar los límites de cada eje.
    * `grid on`: Pone la rejilla de fondo.
    * `title('...')`, `xlabel('...')`, `ylabel('...')`: Títulos y ejes.
* **Estilo:** `plot(x, y, 'Color', 'r', 'LineWidth', 2)`.

---

## 6. Funciones Estadísticas
* `size(A)`: Te da el número de filas y columnas.
* `sum(A)`: Suma todos los números.
* `mean(A)`: Saca el promedio.
* `max(A) / min(A)`: Encuentra el valor más alto o más bajo.

---
<p align="center"><b>Departamento de Ingeniería Eléctrica - Facultad de Ingeniería — Universidad de Concepción</b></p>