# UD1_Ej6 - Cuadernillo de ejercicios Java

---

## 📂 Instrucciones de trabajo

### 1. Abrir el repositorio en Codespaces
1. Entra en tu repositorio personal de GitHub (el que se ha creado a partir de la plantilla).  
2. Pulsa el botón verde **Code**.  
3. Elige la pestaña **Codespaces** y pulsa en **Create codespace on main**.  
4. Se abrirá un entorno de **Visual Studio Code en la nube** donde podrás programar sin instalar nada en tu ordenador.  

---

### 2. Crear un archivo por ejercicio
- Si es código Java → `ej01.java`, `ej02.java`, …  
- Si es una respuesta escrita → `ej05.txt`, `ej17.txt`.  

Ejemplo de estructura esperada:  
```
ej01.java
ej02.java
ej03.java
ej05.txt
...
ej20.java
```

---

### 3. Estructura básica de un programa en Java
Cada archivo `.java` debe contener:  
- Una clase pública con el mismo nombre que el archivo.  
- Un método `main` para ejecutar el programa.  

Ejemplo (`prueba.java`):  
```java
public class prueba {
    public static void main(String[] args) {
        System.out.println("Hola mundo");
    }
}
```

---

### 4. Compilar y ejecutar un programa
Todos los ejercicios **que sean `.java` deben compilarse y ejecutarse**, incluso si producen errores o resultados inesperados (en esos casos deberás escribir la observación en un comentario dentro del código).  

Para ejecutar:  
1. Abre la **terminal integrada** en Codespaces: menú *Terminal → New Terminal*.  
2. Compila el archivo con:  
   ```bash
   javac ej03.java
   ```  
   Esto genera un archivo `ej03.class`.  
3. Ejecuta el programa con:  
   ```bash
   java ej03
   ```  

⚠️ Importante: cuando ejecutes, **no pongas la extensión `.java` o `.class`**, solo el nombre de la clase.  

---

### 5. Guardar y enviar tu trabajo (commit y push desde la terminal)
Tus cambios se guardan en Codespaces, pero para **entregarlos en GitHub** debes hacer *commit* y *push* desde la terminal.  

1. Abre la terminal en Codespaces.  
2. Añade los archivos modificados:  
   ```bash
   git add .
   ```  
3. Haz commit con un mensaje:  
   ```bash
   git commit -m "Terminado ej03"
   ```  
4. Haz push para subir tu trabajo a GitHub:  
   ```bash
   git push
   ```  

⚠️ Si no haces *push*, la profesora no podrá ver tu trabajo.  

---

## ✅ Entrega
- Crea un archivo para cada ejercicio con la nomenclatura indicada.  
- Todos los archivos `.java` deben compilarse y ejecutarse en Codespaces.  
- Escribe las observaciones en comentarios dentro del propio código cuando se pida.  
- Haz commit y push cada vez que termines un ejercicio.  
- No subas archivos `.class`.  
- La profesora revisará tu trabajo directamente en tu repositorio de GitHub.
