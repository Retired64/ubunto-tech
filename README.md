Para seguir las recomendaciones y evitar problemas con los permisos al usar `pip` como usuario 'root', puedes crear y utilizar un entorno virtual. Aquí te indico los pasos para hacerlo:

1. **Instalar `virtualenv` (si no está instalado):**
   Ejecuta el siguiente comando para instalar `virtualenv` si aún no lo tienes:
   ```
   pip3 install virtualenv
   ```

2. **Crear un entorno virtual:**
   En tu terminal, ve al directorio donde quieras crear tu entorno virtual y ejecuta:
   ```
   virtualenv nombre_de_tu_entorno
   ```
   Reemplaza `nombre_de_tu_entorno` con el nombre que quieras darle a tu entorno virtual.

3. **Activar el entorno virtual:**
   Dependiendo de tu sistema operativo, la activación puede variar:

   - **En Linux/macOS:** Ejecuta el comando:
     ```
     source nombre_de_tu_entorno/bin/activate
     ```

   - **En Windows:** Ejecuta el comando:
     ```
     nombre_de_tu_entorno\Scripts\activate
     ```

   Al activar el entorno virtual, verás que el prompt de tu terminal cambia para mostrar el nombre de tu entorno entre paréntesis, indicando que estás dentro del entorno virtual.

4. **Instalar paquetes dentro del entorno virtual:**
   Dentro del entorno virtual activado, puedes usar `pip` para instalar paquetes sin necesidad de usar `sudo` o ser usuario 'root'. Por ejemplo:
   ```
   pip install opencv-python
   ```

5. **Desactivar el entorno virtual:**
   Para salir del entorno virtual cuando hayas terminado, simplemente escribe:
   ```
   deactivate
   ```

Siguiendo estos pasos, podrás crear un entorno virtual, instalar paquetes con `pip` y evitar los problemas relacionados con los permisos de usuario 'root'. Esto también ayuda a mantener tu sistema limpio y separar las dependencias de tus proyectos.
