# Ejercicio 8: Usar GitHub Copilot para Código T-SQL y YAML [Opcional]

### Duración Estimada: 15 minutos

En este ejercicio, el objetivo principal es aprovechar las capacidades de GitHub Copilot, una poderosa herramienta de codificación asistida por IA, para ayudarlo a generar código para dos lenguajes de programación distintos: T-SQL y YAML. ¡Puede aprovechar los comentarios para generar sugerencias de Copilot!

>**Descargo de responsabilidad**: GitHub Copilot sugerirá automáticamente todo el cuerpo de una función o código en texto gris. A continuación, se muestran ejemplos de lo que probablemente verá en este ejercicio, pero la sugerencia exacta puede variar.

>**Nota**: Si no puede ver ninguna sugerencia de GitHub Copilot en VS Code, reinicie VS Code una vez e intente nuevamente.

## Objetivos del laboratorio

Será capaz de completar las siguientes tareas:

- Tarea 1: Generar una consulta SQL con GitHub Copilot usando comentarios
- Tarea 2: Generar YAML con GitHub Copilot usando comentarios
- Tarea 3: Enviar código a tu repositorio desde el espacio de código


### Tarea 1: Generar una consulta SQL con GitHub Copilot usando comentarios

1. Vuelva a Visual Studio Code y, desde el codespace en la ventana Explorador de VS Code, cree un nuevo archivo.

    ![](../media/chat-code-new.png)

1. Nombre el archivo `demo.sql` y escriba el siguiente comentario:

   ```
   -- Create a table for 5 products with product names and prices
   ```

1. Para abrir una nueva pestaña con múltiples soluciones sintetizadas, presione `Ctrl+Enter`. GitHub Copilot sintetizará alrededor de 10 sugerencias de código diferentes en una nueva pestaña. Puede ver las soluciones y, para aceptar una sugerencia, debe hacer clic en **Accept suggestion** debajo de la solución y luego guardar el archivo.

   ![](../media/ex7-t1-s3.png)

1. Después de aceptar la sugerencia, revísela cuidadosamente antes de aplicarla.

   ![](../media/demo-sql-1.png)

   >**Nota**: Es posible que no vea las mismas sugerencias que se muestran en la captura de pantalla; las sugerencias exactas pueden variar.

### Tarea 2: Generar YAML con GitHub Copilot usando comentarios
   
1. Desde el codespace en la ventana Explorador de VS Code, cree un nuevo archivo.

    ![](../media/chat-code-new.png)

1. Nombre el archivo `deploy-app.yml` y escriba el siguiente comentario:

   ```
   # Create a GitHub action to email a report from a file at 6 a.m. daily
   ```

1. Para abrir una nueva pestaña con múltiples soluciones sintetizadas, presione `Ctrl+Enter`. GitHub Copilot sintetizará alrededor de 10 sugerencias de código diferentes en una nueva pestaña. Puede ver las soluciones y, para aceptar una sugerencia, debe hacer clic en **Accept suggestion** debajo de la solución y luego guardar el archivo.

   ![](../media/ex7-t2-s3.png)

1. Después de aceptar la sugerencia, revísela cuidadosamente antes de aplicarla.

   ![](../media/demo-yaml-1.png)

   >**Nota**: Es posible que no vea las mismas sugerencias que se muestran en la captura de pantalla; las sugerencias exactas pueden variar.

### Tarea 3: Enviar código a tu repositorio desde el espacio de código

1. Use la terminal de VS Code para agregar archivos al repositorio. Abra la Terminal de VS Code si aún no está abierta.

1. Ejecute el siguiente comando para agregar todos los archivos al repositorio:
   
   ```
   git add --all
   ```

1. A continuación, desde la terminal de VS Code, confirme los cambios en el repositorio:

   ```
   git commit -m "Copilot fourth commit"
   ```

1. Por último, desde la Terminal de VS Code, envíe el código al repositorio:

   ```
   git push
   ```

   ![](../media/ex-6-push.png)

   >**Nota**: Espere unos 60 segundos y luego actualice la página de inicio de su repositorio para el siguiente paso.

   >**Nota**: Si se enfrenta a algún error que dice Rechazado, ejecute el siguiente comando y vuelva a ejecutar el comando git push. Esto recuperará los cambios en la rama remota y los fusionará en la rama actual sin cambiar la base.
    
    ```
    git pull --no-rebase
    ```   

   >**Nota**: Aparece un mensaje en la terminal indicando que necesita cerrar el archivo recién abierto, además de los dos archivos que ya están abiertos. Cierre el archivo recién abierto.

1. Puede verificar los nuevos archivos disponibles en su repositorio de GitHub.

   ![](../media/ex-6-github.png)

### Resumen

En este ejercicio, ha generado código para SQL y YAML con éxito usando comentarios con la ayuda de GitHub Copilot.

### Ha completado el laboratorio con éxito
