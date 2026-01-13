# 📊 ¿Qué es Trabajar con Datos?

## Los datos son observaciones sobre el mundo

Un dato es simplemente **una observación registrada**.

Puede ser:
- Cuántas personas visitaron una web
- Qué temperatura hizo ayer
- Cuánto cuesta un producto
- Cuántos likes tiene una publicación

Cuando tienes muchos datos juntos, puedes empezar a ver patrones, hacer comparaciones, sacar conclusiones. Eso es trabajar con datos: **observar, organizar, entender, comunicar**.

No se trata de tener un don especial para los números. Se trata de hacer preguntas y buscar respuestas en la información que tienes.

---

## 🍎 Analogía: Tu lista de la compra

Imagina que durante un mes guardas todos los tickets de la compra. Al final del mes, los miras y te preguntas:

- **¿Cuánto he gastado en total?** (suma)
- **¿Qué día gasté más?** (buscar el máximo)
- **¿Compré más frutas o más precocinados?** (comparación)
- **¿Hay algún patrón? Por ejemplo, ¿gasto más los fines de semana?** (tendencias)

Eso es análisis de datos. Tienes información (los tickets), la organizas (por fecha, por categoría), la analizas (sumas, comparas) y sacas conclusiones (gasto más los domingos).

No usaste fórmulas complejas. No programaste nada. Solo observaste y pensaste. **Ese es el núcleo del trabajo con datos.**

---

## 🧩 ¿Qué es una tabla?

Cuando trabajas con datos, casi siempre los organizas en **tablas**: filas y columnas.

Cada **fila** es una observación. Cada **columna** es una característica de esa observación.

Ejemplo: si tienes datos de ventas de una tienda:

| Fecha       | Producto | Cantidad | Precio |
|-------------|----------|----------|--------|
| 2026-01-05  | Manzanas | 10       | 15€    |
| 2026-01-05  | Pan      | 5        | 7€     |
| 2026-01-06  | Manzanas | 8        | 12€    |

Cada fila es una venta. Cada columna es una información sobre esa venta.

Con esto puedes responder preguntas como:
- ¿Qué se vendió más?
- ¿Qué día se ganó más dinero?
- ¿Cuál es el precio medio de las manzanas?

**Trabajar con datos es hacerte preguntas y buscar las respuestas en las tablas.**

---

## � ¿Cómo se ve una tabla en la vida real?

Vale, ya sabes qué es una tabla conceptualmente: filas y columnas. Pero **¿dónde ves esa tabla en tu ordenador?**

La respuesta más común: **en una hoja de cálculo**.

### ¿Qué es una hoja de cálculo?

Una hoja de cálculo (como Excel o Google Sheets) es un programa que muestra datos organizados en una cuadrícula: filas numeradas, columnas con letras.

**Imagina una libreta cuadriculada gigante.** Cada cuadrito es un espacio donde puedes escribir algo: un número, un texto, una fecha. Esos cuadritos se llaman **celdas**.

- La celda **A1** es la primera: columna A, fila 1
- La celda **B3** es la que está en la columna B, fila 3

**Ejemplo visual:**

```
     A          B          C          D
1  Fecha      Producto   Cantidad   Precio
2  2026-01-05 Manzanas   10         15€
3  2026-01-05 Pan        5          7€
4  2026-01-06 Manzanas   8          12€
```

Cada celda contiene un dato. Juntas, forman la tabla.

### ¿Qué es una fórmula?

Una fórmula es una **instrucción que le das a la hoja de cálculo** para que haga un cálculo por ti.

Por ejemplo:
- "Suma todos los precios" 
- "Calcula el promedio de las cantidades"
- "Dime cuál es el valor máximo"

No tienes que hacer las cuentas tú. Le dices a la hoja de cálculo qué quieres calcular, y ella lo hace automáticamente. Si cambias un dato, el resultado se actualiza solo.

**Analogía:** Es como tener una calculadora integrada en cada celda. En lugar de sumar manualmente, le dices "suma estos números" y lo hace por ti.

### ¿Por qué esto es útil?

Porque cuando tienes 10 filas, puedes sumar a mano. Pero cuando tienes 1.000 filas, necesitas que la máquina lo haga por ti. Las hojas de cálculo te permiten:

- Ver todos los datos organizados de un vistazo
- Hacer cálculos sin equivocarte
- Cambiar un valor y ver cómo afecta al resultado
- Crear gráficos automáticamente

**Esto es lo que harás al principio del itinerario:** trabajar con tablas en una hoja de cálculo, viendo cada dato y cada cálculo de forma visual.

Más adelante aprenderás a automatizar esto con código (Python), pero primero necesitas entender qué estás haciendo. Y para eso, nada mejor que verlo con tus propios ojos en una hoja de cálculo.

---

## �🔍 ¿Qué hace una persona que analiza datos?

Su trabajo tiene 4 fases:

1. **Recopilar**: conseguir los datos (de una web, de una base de datos, de un archivo)
2. **Limpiar**: quitar errores, organizar, dejar solo lo que sirve
3. **Analizar**: calcular, comparar, buscar patrones
4. **Comunicar**: hacer gráficos, escribir informes, contar lo que has encontrado

No se trata de ser buena en matemáticas. Se trata de ser curiosa, organizada y clara al explicar.

---

## 💭 Preguntas para reflexionar

Piensa en esto (no hace falta escribir, solo reflexiona):

1. **¿Qué datos generas tú en tu día a día?**  
   Cada vez que compras algo, envías un mensaje, ves una serie... estás generando datos. Alguien los puede analizar. ¿Qué podrían descubrir sobre ti?

2. **¿Alguna vez has tomado una decisión basándote en información?**  
   Por ejemplo: "Voy al supermercado X porque es más barato". Eso es análisis de datos informal. Comparaste precios (datos) y decidiste.

3. **¿Qué pregunta te gustaría responder si tuvieras acceso a datos?**  
   Puede ser sobre tu ciudad, tu sector, tu hobby... Cualquier pregunta que empiece por "cuánto", "cuándo", "quién" o "por qué" puede responderse con datos.

---

## ✅ Después de leer esto, deberías poder…

- Explicar qué es un dato sin usar palabras técnicas
- Entender qué es una tabla (filas = observaciones, columnas = características)
- Describir en qué consiste el trabajo de una persona que analiza datos

---

## 🚫 Lo que NO necesitas saber todavía

No necesitas saber estadística. No necesitas saber **usar** Excel o Google Sheets (ya lo aprenderás). No necesitas conocer SQL, Python o cualquier herramienta de análisis. No necesitas entender términos como "dataframe", "variable", "base de datos", "query" o "visualización".

No necesitas saber qué es una media, una mediana, una desviación estándar o una correlación.

No necesitas saber escribir fórmulas ni saber qué teclas pulsar en Excel.

**Solo necesitas entender la idea:** trabajar con datos es observar, organizar, entender y comunicar información. Las hojas de cálculo son la herramienta donde eso sucede visualmente. El resto (cómo usarlas, qué fórmulas existen, cómo hacer gráficos) lo verás cuando sea el momento.
