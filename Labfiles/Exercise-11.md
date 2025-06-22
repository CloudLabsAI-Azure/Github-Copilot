# Ejercicio 11: Crear un Minijuego con GitHub Copilot [Opcional]

### Duración Estimada: 20 minutos

En este ejercicio, utilizará las capacidades de GitHub Copilot para construir un clásico minijuego de piedra, papel o tijera. A través de este ejercicio práctico, no solo perfeccionará sus conocimientos de programación, sino que también reforzará su destreza en la creación de aplicaciones de consola con Python.

## Objetivos del laboratorio

Será capaz de completar las siguientes tareas:

- Tarea 1: Probar su GitHub Codespace
- Tarea 2: Crear la lógica del juego

### Tarea 1: Probar su GitHub Codespace

1. Haz clic en **Archivo (1)** y luego haz clic en **Nueva Ventana (2)**.

   ![](../media/190625(17).png)

1. Haga clic en los **puntos suspensivos (1)** en la parte superior, haga clic en **Terminal (2)** y seleccione **New terminal (3)**.

   ![](../media/190625(15).png)  

1. Ejecute el siguiente comando para clonar el repositorio **Mini-game-with-copilot**.

   ```
   git clone https://github.com/MicrosoftDocs/mslearn-challenge-project-create-mini-game-with-copilot.git
   ```

1. Haga clic en **Explorador** y seleccione **Abrir carpeta** en las opciones.

1. En el Explorador de archivos, vaya a la sección **Quick access** y seleccione la carpeta **mini-game-with-copilot**.

1. Abra el archivo **app.py**.

   ![](../media/vs19.png)

1. Pegue el siguiente comentario y haga clic en **Enter** y verifique que el próximo comentario sea generado por **GitHub Copilot**.

   ```
   # write 'hello world' to the console
   ```

   ![](../media/vs14.png)
   
      >**Nota:** En los casos en que el código no sea generado por **GitHub Copilot**, haga clic en **Extensiones**, busque GitHub Copilot, selecciónelo y haga clic en **Instalar en Codespaces: shiny acorn**.

      ![](../media/vs13.png)

1. Haga clic en **Guardar**.
   
1. Haga clic en **Terminal (1)** y seleccione **Nuevo Terminal (2)**.

   ![](../media/vs15.png)

1. Ejecute la aplicación con el comando **python app.py** en la terminal y compruebe si el resultado es similar al siguiente mensaje de consola:

   ![](../media/vs16.png)


### Tarea 2: Crear la lógica del juego

1. Elimine el código generado en el paso anterior y luego use el atajo CTRL + I para solicitar a GitHub Copilot que realice una acción. Pegue el siguiente **comentario (1)** para obtener el código y haga clic en el botón Realizar solicitud **(Enter) (2)** y haga clic en **Aceptar (3)** para utilizar el código.
   
   ```
    The player can choose rock, paper, or scissors, and invalid inputs are handled gracefully. After each round, display whether the player won, lost, or tied. Allow the player to play again after each round and display their score at the end of the game. Inputs are converted to lowercase for consistency.
   ```

   ![](../media/10-1.png)

      >**Nota:** Sin embargo, es importante tener en cuenta que las sugerencias proporcionadas por GitHub Copilot pueden variar y, en ocasiones, pueden ser irrelevantes y requerir una comprensión clara del código de Python y su uso.

1. Haga clic en **Guardar**.

1. Ejecute la aplicación con el comando **python app.py** en la terminal.

   ![](../media/vs17.png)

### Resumen

En este ejercicio, ha creado con éxito un minijuego usando Python y GitHub Copilot.

### Ha completado el laboratorio con éxito
