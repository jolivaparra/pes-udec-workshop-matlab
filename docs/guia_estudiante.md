# 📖 Guía de Aprendizaje Autónomo
**Workshop MATLAB® — IEEE PES Universidad de Concepción**

## 🛠️ 1. Preparación del Entorno (Setup)

Para que los scripts funcionen correctamente con los datos del taller, sigue este orden:

1. **Clonación Directa:** En la pestaña **Home** de MATLAB, ve a **New** > **Git Clone** y pega el link del repositorio: 
   `https://github.com/jolivaparra/pes-udec-workshop-matlab`
2. **Ubicación de Trabajo (Crítico):** * Una vez clonado, navega en el panel *Current Folder* hasta entrar en la carpeta `scripts/`.
   * **IMPORTANTE:** Debes estar posicionado **dentro** de `scripts/` para que las rutas de carga de datos (`../data/...`) funcionen sin errores.

---

## 🚀 2. Flujo de Trabajo por Bloques

El taller está dividido en módulos. No saltes directamente al código; sigue este ciclo de aprendizaje:

### Step A: La Teoría (Presentación)
Abre el archivo `presentacion.pdf` en la raíz del proyecto. Lee el bloque correspondiente (ej. **Bloque 1: Fundamentos**). Detente cuando llegues a la diapositiva del siguiente Bloque.

### Step B: La Práctica (Live Scripts)
Abre el archivo `.mlx` asociado al bloque dentro de la carpeta `scripts/`:
* **B1.mlx:** Arreglos, matrices e indexación.
* **B2.mlx:** Importar tablas `.csv` y crear gráficas profesionales.

### Step C: Ejecución y Desafíos
* Lee las explicaciones dentro del Live Script.
* Completa los bloques de código vacíos o marcados como "Ejercicio".
* Usa `Ctrl + Enter` para ejecutar y ver los resultados inmediatamente.

---

## 📈 3. Proyecto Final Aplicado

Una vez domines los Bloques 1 y 2, dirígete al archivo `scripts/P1.mlx`. 
En este reto final deberás:
1. Importar y desempaquetar datos reales de un proceso térmico.
2. Procesar la información usando máscaras lógicas y operaciones de arreglos.
3. Generar una visualización de buen nivel para un informe.

---

## 💡 Tips de Supervivencia

* **Documentación:** Si no conoces una función, escribe `doc nombre_de_la_funcion` en la Command Window.
* **Anexos:** Si quieres aprender los bloques que utilizan la lógica de programación (ciclos o condicionales), revisa el [Anexo de Lógica](./anexos/bloques-if-for.md).
* **Rutas:** Si obtienes un error de "File not found", verifica que tu panel de *Current Folder* sea efectivamente la carpeta `scripts/`.

---
<p align="center"><b>Desarrollado por Joshua Oliva Parra para IEEE PES UdeC</b></p>