# Colecciones de Datos

## Listas (Lists)
Son colecciones ordenadas y mutables (modificables) de elementos.

### ¿Por qué y cuándo se utilizan?
Se usan cuando tienes una colección de datos que va a cambiar durante la ejecución del programa.

Si necesitas agregar, eliminar o modificar elementos sobre la marcha, la lista es la herramienta adecuada.

### Sintaxis

Se definen utilizando corchetes [].

### Ejemplo 1: Sintaxis aplicada
```python
mi_lista = ["Java", "Python", "PHP"]
```
### Ejemplo 2: Aplicado

Imagina un sistema de registro donde los estudiantes se van inscribiendo a un ramo a lo largo del día.

```python
# Lista inicial de estudiantes inscritos
inscritos_ramo = ["Ana", "Pedro", "Diego"]

# Un nuevo estudiante se inscribe al ramo
inscritos_ramo.append("Sofía")

# Pedro bota el ramo
inscritos_ramo.remove("Pedro")

print(inscritos_ramo) 
# Salida: ['Ana', 'Diego', 'Sofía']
```

## Tuplas (Tuples)
Son colecciones ordenadas e inmutables de elementos. 
Una vez creadas, no se pueden modificar (no puedes agregar, eliminar ni cambiar sus elementos).

### ¿Por qué y cuándo se utilizan?
Se usan cuando quieres agrupar datos que no deben cambiar bajo ninguna circunstancia. 

Esto protege la integridad de los datos, evita errores accidentales en el código y, además, hace que la iteración sea ligeramente más rápida y consuma menos memoria que una lista.

### Sintaxis

Se definen utilizando paréntesis ().

### Ejemplo 1: Sintaxis

```python
mi_tupla = (10, 20, 30)
```

### Ejemplo 2: Aplicado

Almacenar las coordenadas geográficas fijas de las distintas sedes de una universidad. Es un dato que no va a cambiar durante la ejecución de la aplicación.

```python
# Coordenadas (Latitud, Longitud) de la sede principal
coordenadas_sede = (-33.4372, -70.6506)

print(f"La latitud de la sede es: {coordenadas_sede[0]}")

# Si intentas hacer coordenadas_sede[0] = -34.000, Python arrojará un error.
```

## Diccionarios (Dictionaries)

Son colecciones mutables y no ordenadas (aunque en las versiones recientes de Python mantienen el orden de inserción) que almacenan datos en pares de clave-valor (key-value).

### ¿Por qué y cuándo se utilizan?

Se usan cuando necesitas relacionar un identificador único (la clave) con un dato específico (el valor), de manera similar a cómo funciona un registro de una base de datos o un archivo JSON.

Son ideales para búsquedas rápidas y para representar entidades con múltiples atributos.

### Sintaxis

Se definen utilizando llaves {} y separando la clave del valor con dos puntos :

### Ejemplo 1: Sintaxis

```python
mi_diccionario = {"lenguaje": "Python", "version": 3.12}
```
### Ejemplo 2: Aplicado

Almacenar el perfil de un estudiante y sus notas en distintas evaluaciones, lo cual requiere etiquetas claras para cada dato.
```python
estudiante = {
    "rut": "12345678-9",
    "nombre": "Carlos",
    "carrera": "Ingeniería",
    "notas_solemnes": [4.5, 5.2, 6.0] # Un diccionario puede contener listas
}

# Accediendo a un dato específico
print(f"El estudiante {estudiante['nombre']} obtuvo un {estudiante['notas_solemnes'][2]} en su última solemne.")

# Agregando un nuevo par clave-valor
estudiante["estado"] = "Aprobado"
```