## Guía de Ejercicios Prácticos: Listas, Tuplas y Diccionarios en Python

### 1. Inventario de Laboratorio (Listas)
* **Objetivo:** Comprender la mutabilidad de las listas mediante la adición y eliminación de elementos.
* **Contexto:** El encargado del laboratorio de computación necesita un programa para llevar el registro de los equipos disponibles. El programa debe comenzar con una lista de equipos, permitir agregar un "Proyector", eliminar un "Mouse defectuoso" y mostrar la cantidad total de equipos.
* **Salida Esperada:**
    ```text
    Inventario inicial: ['Monitor', 'Teclado', 'Mouse defectuoso', 'CPU']
    Actualizando inventario...
    Inventario final: ['Monitor', 'Teclado', 'CPU', 'Proyector']
    Total de equipos registrados: 4
    ```

### 2. Análisis de Asistencia (Listas)
* **Objetivo:** Iterar sobre una lista para realizar cálculos matemáticos básicos (sumatorias y promedios).
* **Contexto:** Un docente tiene una lista con la cantidad de alumnos que asistieron a clases cada día durante una semana. El programa debe calcular el total de asistencias en la semana, el día con mayor asistencia y el promedio diario.
* **Salida Esperada:**
    ```text
    Asistencias de la semana: [35, 42, 38, 45, 40]
    Total de alumnos en la semana: 200
    Mayor asistencia registrada: 45 alumnos
    Promedio de asistencia diaria: 40.0 alumnos
    ```

### 3. Fila de Impresión (Listas)
* **Objetivo:** Utilizar métodos específicos de listas (`append`, `pop`) para simular el comportamiento de una cola (Queue).
* **Contexto:** La biblioteca tiene una cola de trabajos enviados a la impresora. El programa debe simular la llegada de tres documentos, y luego simular cómo se imprimen (se eliminan) en el mismo orden en que llegaron (el primero en llegar es el primero en salir).
* **Salida Esperada:**
    ```text
    Documentos en cola: ['Ensayo.pdf', 'Guia_Ejercicios.docx', 'Tesis.pdf']
    Imprimiendo: Ensayo.pdf...
    Imprimiendo: Guia_Ejercicios.docx...
    Cola restante: ['Tesis.pdf']
    ```

### 4. Coordenadas Geográficas de Sedes (Tuplas)
* **Objetivo:** Comprender la inmutabilidad y el acceso por índice en las tuplas.
* **Contexto:** Una aplicación móvil necesita almacenar las coordenadas exactas (Latitud, Longitud) de las distintas sedes de la universidad. El estudiante debe crear tuplas para dos sedes, imprimir sus valores y luego *intentar* modificar un valor para observar y explicar el error que arroja Python.
* **Salida Esperada:**
    ```text
    Sede Norte - Latitud: -33.412, Longitud: -70.615
    Sede Sur - Latitud: -33.589, Longitud: -70.678
    (Nota: El programa debe fallar intencionalmente al intentar hacer sede_norte[0] = -33.000)
    ```

### 5. Configuración de Base de Datos (Tuplas)
* **Objetivo:** Empaquetar y desempaquetar datos heterogéneos usando tuplas.
* **Contexto:** Los parámetros para conectarse a un servidor de base de datos universitario no deben cambiar durante la ejecución. Crea una tupla que contenga la IP del servidor, el puerto y el nombre de la base de datos. Luego, "desempaqueta" esos valores en tres variables distintas e imprímelas en un mensaje de conexión.
* **Salida Esperada:**
    ```text
    Iniciando conexión a la base de datos...
    Conectando a IP: 192.168.1.100
    Puerto: 3306
    Base de datos: bd_alumnos
    Conexión exitosa.
    ```

### 6. Diccionario de Términos de Programación (Diccionarios)
* **Objetivo:** Crear un diccionario, acceder a sus valores mediante claves y agregar nuevos pares.
* **Contexto:** Crea un glosario básico para la clase de Aplicaciones Computacionales. El diccionario debe tener al menos tres conceptos (ej. "Algoritmo", "Variable", "Bucle") con sus definiciones. El usuario debe poder ingresar un concepto por consola y ver su definición, o recibir un mensaje si no existe.
* **Salida Esperada (Ejemplo de ejecución):**
    ```text
    Ingrese término a buscar: Variable
    Definición: Espacio en memoria para almacenar un dato que puede cambiar.
    ```

### 7. Conversor de Monedas (Diccionarios)
* **Objetivo:** Utilizar un diccionario como una tabla de búsqueda (Lookup table) para realizar cálculos.
* **Contexto:** Un estudiante de intercambio necesita convertir un monto en Pesos Chilenos (CLP) a diferentes divisas. El programa debe tener un diccionario con las tasas de conversión (Dólar, Euro, Real). Debe pedir un monto en CLP y mostrar su equivalencia en las tres divisas.
* **Salida Esperada:**
    ```text
    Monto ingresado: 100000 CLP
    Equivalencia en Dólares: 105.2 USD
    Equivalencia en Euros: 98.5 EUR
    Equivalencia en Reales: 520.4 BRL
    ```

### 8. Frecuencia de Caracteres (Diccionarios)
* **Objetivo:** Iterar sobre una cadena de texto y poblar un diccionario dinámicamente.
* **Contexto:** Se necesita analizar la seguridad de una contraseña ingresada por un usuario. El programa debe leer una contraseña y crear un diccionario donde las claves sean cada carácter utilizado y el valor sea la cantidad de veces que se repite.
* **Salida Esperada:**
    ```text
    Contraseña analizada: 'supersecreto'
    Frecuencia de caracteres:
    {'s': 2, 'u': 1, 'p': 1, 'e': 3, 'r': 2, 'c': 1, 't': 1, 'o': 1}
    ```

### 9. Carrito de Compras de la Cafetería (Lista de Diccionarios)
* **Objetivo:** Integrar listas y diccionarios para manejar colecciones de entidades.
* **Contexto:** Simula el sistema de cobro de la cafetería. Crea una lista llamada `carrito` que contenga varios diccionarios. Cada diccionario representa un producto con las claves `"nombre"`, `"precio"` y `"cantidad"`. El programa debe recorrer la lista y calcular el total a pagar por el estudiante.
* **Salida Esperada:**
    ```text
    Resumen de compra:
    - 2 x Café (Total: $3000)
    - 1 x Sandwich (Total: $2500)
    - 3 x Galletas (Total: $1500)
    --------------------------
    Total a pagar: $7000
    ```

### 10. Gestión de Bibliografía del Curso (Diccionario con Listas y Tuplas)
* **Objetivo:** Integración avanzada de las tres estructuras de datos (Diccionario principal, que contiene Listas, que contienen Tuplas).
* **Contexto:** El sistema de la biblioteca estructura sus datos de forma compleja. Crea un diccionario llamado `bibliografia`. Sus claves serán las categorías (ej. `"Programación"`, `"Bases de Datos"`). El valor de cada clave será una lista. Dentro de la lista, cada libro será una tupla inmutable con `(Titulo, Autor, Año)`. El programa debe imprimir todos los libros del año 2020 en adelante.
* **Salida Esperada:**
    ```text
    Buscando libros recientes (Año >= 2020)...
    - Categoría: Programación -> 'Python Crash Course' por Eric Matthes (2023)
    - Categoría: Bases de Datos -> 'SQL para Principiantes' por Ana Pérez (2021)
    Búsqueda finalizada.
    ```