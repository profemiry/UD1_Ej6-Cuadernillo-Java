# UD1_Ej6 - Cuadernillo de ejercicios Java

---

## 📂 Instrucciones de trabajo

### 1. Abrir el repositorio en Codespaces
1. Entra en tu repositorio personal de GitHub (el que se ha creado a partir de la plantilla).  
2. Pulsa el botón verde **Code**.  
3. Elige la pestaña **Codespaces** y pulsa en **Create codespace on main**.  
4. Se abrirá un entorno de **Visual Studio Code en la nube** donde podrás programar sin instalar nada en tu ordenador.  

---

### 2. Instalar extensión Live Preview (solo la primera vez)
Para poder visualizar los archivos `.html` (JavaDoc) dentro de Codespaces:  
1. En Codespaces, abre la pestaña de **Extensiones** (icono de 4 cuadrados en la barra lateral izquierda).  
2. Busca **Live Preview (Microsoft)**.  
3. Instálala.  
4. Cuando abras un archivo `.html`, podrás hacer clic derecho → **Show Preview** para verlo renderizado como una página web.  

---

### 3. Crear un archivo por ejercicio
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

### 4. Estructura básica de un programa en Java
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

### 5. Compilar y ejecutar un programa
Todos los ejercicios **que sean `.java` deben compilarse y ejecutarse**, incluso si producen errores o resultados inesperados (en esos casos deberás escribir la observación en un comentario dentro del código).  

Para ejecutar:  
1. Abre la **terminal integrada** en Codespaces: menú *Terminal → New Terminal*.  
2. Compila el archivo con:  
   ```bash
   javac prueba.java
   ```  
   Esto genera un archivo `prueba.class`.  
3. Ejecuta el programa con:  
   ```bash
   java prueba
   ```  

⚠️ Importante: cuando ejecutes, **no pongas la extensión `.java` o `.class`**, solo el nombre de la clase.  

---

### 6. Guardar y enviar tu trabajo (commit y push desde la terminal)
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

### 7. Generar y publicar la documentación JavaDoc (solo ejercicio 20)
En el ejercicio 20 aprenderás a usar **JavaDoc** para documentar tu programa.

1. Genera la documentación desde la terminal (incluyendo autor y versión):  
   ```bash
   javadoc -d docs -author -version ej20.java
   ```  
   Esto creará una carpeta **docs** con los archivos `.html`.

2. Comprueba que puedes ver `index.html` o `ej20.html` con **Live Preview** (clic derecho → *Show Preview*).  

3. Sube la carpeta a GitHub (junto con tu código):  
   ```bash
   git add .
   git commit -m "Subida documentación JavaDoc del ej20"
   git push
   ```

4. Activa **GitHub Pages**:  
   - Entra en tu repositorio en GitHub.  
   - Ve a **Settings → Pages**.  
   - En *Source*, elige la rama `main` y la carpeta `/docs`.  
   - Guarda los cambios.  

5. Abre el enlace que te da GitHub Pages (del estilo):  
   ```
   https://tu-usuario.github.io/nombre-repo/
   ```
   Ahí podrás ver tu JavaDoc como si fuera una web oficial.  

---

## ✅ Entrega
- Crea un archivo para cada ejercicio con la nomenclatura indicada.  
- Todos los archivos `.java` deben compilarse y ejecutarse en Codespaces.  
- Escribe las observaciones en comentarios dentro del propio código cuando se pida.  
- Haz commit y push cada vez que termines un ejercicio.  
- No subas archivos `.class`.  
- La profesora revisará tu trabajo directamente en tu repositorio de GitHub.  
