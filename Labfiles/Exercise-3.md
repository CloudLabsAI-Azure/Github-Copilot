# Ejercicio 3: Explorar Python con GitHub Copilot: Sugerencias de Código Inteligentes

### Duración Estimada: 10 minutos

GitHub Copilot ofrece sugerencias para una gran variedad de lenguajes y frameworks, y destaca particularmente con Python, JavaScript, TypeScript, Ruby, Go, C# y C++. Además, Copilot ofrece una valiosa asistencia para generar consultas para bases de datos.

En este ejercicio, tendrá la oportunidad de profundizar en Python y aprovechar las capacidades de Copilot, beneficiándose de una variedad de sugerencias.

>**Descargo de responsabilidad**: GitHub Copilot sugerirá automáticamente todo el cuerpo de una función o código en texto gris. A continuación, se muestran ejemplos de lo que probablemente verá en este ejercicio, pero la sugerencia exacta puede variar.

>**Nota**: Si no puede ver ninguna sugerencia de GitHub Copilot en VS Code, reinicie VS Code una vez e intente nuevamente.

## Objetivos del laboratorio

Será capaz de completar las siguientes tareas:

- Tarea 1: Agregar código de un método en Python
- Tarea 2: Ver la pestaña GitHub Copilot con múltiples sugerencias
- Tarea 3: Enviar código a su repositorio desde VS Code codespace

## Tarea 1: Agregar código de un método en Python

### Instalando la extensión Python en VS Code

1. Para instalar la extensión Python, se deben realizar los siguientes pasos dentro de Visual Studio Code:
    - Haga clic en el ícono **Extensiones** **(1)** en la barra de actividades presente en el lado izquierdo de la ventana de Visual Studio Code.
    - En el cuadro de búsqueda "Buscar Extensiones en Marketplace", escriba y busque la extensión **Python** **(2)**.
    - Seleccione **Python** **(3)** de la lista de resultados que aparecen.
    - Haga clic en el botón **Instalar** **(4)**.

   ![](../media/python-install.png)

1. Dentro del codespace en la ventana Explorador de VS Code, cree un Nuevo Archivo.

   ![](../media/ex-3-create-py.png)

1. Nombre el archivo `app.py`. Escriba el siguiente código dentro de este archivo recién creado y luego use la tecla Enter para ir a la siguiente línea.

   ```
   def hello():
   ```

1. GitHub Copilot sugerirá automáticamente un código completo en texto gris. Presione la tecla Tab para aceptar la sugerencia y luego guarde el archivo.

   ![](../media/ex-3-apppy.png)

   > **Nota**: Este es un ejemplo de lo que probablemente verá; sin embargo, la recomendación precisa podría variar.

### Tarea 2: Ver la pestaña GitHub Copilot con múltiples sugerencias

En esta tarea, continuará usando Copilot y es posible que necesite algunas de las sugerencias que ofrece GitHub Copilot. GitHub Copilot sintetizará alrededor de 10 sugerencias de código diferentes en una nueva pestaña.

1. Dentro del codespace en la ventana Explorador de VS Code, cree un nuevo archivo llamado `prime.py` **(1)** y escriba el siguiente código **(2)**.

   ```
   def prime(n):
   ```

   ![](../media/co-suggestion1.png)

   > **Nota**: Este es un ejemplo de lo que probablemente verá; sin embargo, la recomendación precisa podría variar.

1. Para abrir una nueva pestaña con múltiples soluciones sintetizadas, presione `Ctrl + Enter`. GitHub Copilot sintetizará alrededor de 10 sugerencias de código diferentes en una nueva pestaña. Puede ver las soluciones y, para aceptar una sugerencia, debe hacer clic en **Accept suggestion** debajo de la sugerencia deseada y luego guardar el archivo.

   ![](../media/accpet-suggestion.png)

    > **Nota**: En caso de que no aparezcan las sugerencias de Github Copilot, cierre y vuelva a abrir Visual Studio Code.

### Tarea 3: Enviar código a su repositorio desde VS Code codespace

1. Vuelva a la Terminal de VS Code y agregue archivos al repositorio.

2. Ejecute el siguiente comando para agregar los archivos `app.py` y `prime.py` al repositorio:

   ```
   git add app.py prime.py
   ```

3. A continuación, desde la Terminal de VS Code, envíe los cambios al repositorio:

   ```
   git commit -m "Copilot second commit"
   ```

4. Por último, desde la Terminal de VS Code, envíe el código al repositorio:

   ```
   git push
   ```

   ![](../media/ex-3-push2.png)

   >**Nota**: Espere unos 60 segundos y luego actualice la página de inicio de su repositorio para el siguiente paso.

5. Puede verificar los archivos `app.py` y `prime.py` disponibles en su repositorio de GitHub.

   ![](../media/ex-3-github3.png)

   <validation step="95754ad8-7b5c-486d-8e7c-d034df03ff1b" />
   
6. Haga clic en **Siguiente** a continuación para pasar a la página siguiente.

### Resumen

En este ejercicio, ha finalizado con éxito la tarea de usar Python en conjunto con Copilot y lo ha hecho con el beneficio de recibir múltiples sugerencias.

### Ha completado el laboratorio con éxito
