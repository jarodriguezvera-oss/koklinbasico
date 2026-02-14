# Evaluación: Conceptos Básicos de Kotlin 🚀

¡Bienvenido a tu primera actividad práctica de Kotlin! En este ejercicio, aplicarás los pilares fundamentales del lenguaje construyendo la lógica de un sistema para un mini-RPG.

## 📋 Objetivos de la Actividad
Deberás demostrar el dominio de:
* Declaración de variables (`val` vs `var`).
* Sistemas de tipos y **Nulabilidad**.
* Interpolación de cadenas (Strings).
* Estructuras de control modernas (`when`).
* Clases, constructores primarios y parámetros opcionales.

---

## 🛠️ Instrucciones del Proyecto

Deberás trabajar en el archivo `src/main/kotlin/Main.kt`. La tarea consiste en implementar la clase `Personaje` siguiendo estas especificaciones:

### 1. La Clase `Personaje`
Crea una clase que reciba los siguientes parámetros en su **constructor primario**:
* **`nombre`**: Una constante de tipo texto.
* **`nivel`**: Una variable numérica que, si no se especifica, debe iniciar en **1**.
* **`apodo`**: Un texto que **puede ser nulo** (null). Por defecto, debe ser nulo.

### 2. Lógica de Rangos (`obtenerRango`)
Implementa una función llamada `obtenerRango()` que devuelva un `String` basado en el nivel actual usando la sentencia `when`:
* **1 a 10**: "Novato"
* **11 a 20**: "Guerrero"
* **Más de 20**: "Leyenda"
* Cualquier otro caso: "Desconocido"

### 3. Presentación (`presentarse`)
Implementa una función llamada `presentarse()` que devuelva un `String` con el siguiente formato, usando **interpolación de cadenas**:
> `"Soy [nombre], nivel [nivel] ([apodo]). Rango: [rango]"`

* **Importante:** Si el `apodo` es nulo, debe mostrar el texto `"Sin apodo"` en su lugar (puedes usar el operador Elvis `?:`).

---

## 🧪 Cómo probar tu código
Este repositorio tiene configurado **Autograding**. Cada vez que hagas un `push` de tus cambios a GitHub, se ejecutarán pruebas automáticas para calificar tu entrega.

Si quieres probar de forma local antes de subir:
1. Abre una terminal en la carpeta del proyecto.
2. Ejecuta el comando:
   ```bash
   ./gradlew test
