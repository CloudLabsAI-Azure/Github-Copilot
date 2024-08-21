# Ejercicio 1: Aprovechar Codespaces con VS Code para Copilot

### Duración Estimada: 15 minutos

GitHub Copilot es un programador de pares de IA diseñado para que escribir código sea más fácil y rápido. Extrae el contexto de los comentarios y el código para sugerir líneas individuales y funciones completas al instante. GitHub Copilot está impulsado por OpenAI Codex, un modelo de lenguaje generativo preentrenado creado por OpenAI.

**GitHub Copilot es compatible con una amplia gama de editores de código, como Neovim, JetBrains IDE, Visual Studio y VS Code.**

Además, GitHub Copilot está entrenado en todos los lenguajes que se pueden encontrar en repositorios públicos. La cantidad y variedad de datos de entrenamiento para cada lenguaje puede tener un impacto en la calidad de las recomendaciones que obtenga.

**GitHub Codespace** es un entorno de desarrollo alojado en la nube. Puede personalizar su proyecto para GitHub Codespaces enviando archivos de configuración a su repositorio (a menudo conocido como Configuración-como-Código), lo que crea una configuración de codespace repetible para todos los usuarios de su proyecto.

El uso de Copilot dentro de un Codespace demuestra sin esfuerzo la simplicidad de comenzar con las herramientas integrales de [Programación Colaborativa](https://github.com/features#features-collaboration) de GitHub.

En este ejercicio, se le asigna la tarea de crear un contenedor de desarrollo. Deberá especificar ciertas extensiones o configuraciones a utilizar o instalar en su Codespace. Como parte de este proceso, asegúrese de incluir Copilot en su lista de extensiones.

## Objetivos del laboratorio

Será capaz de completar las siguientes tareas:

- Tarea 1: Habilitar Copilot dentro de un Codespace

## Tarea 1: Habilitar Copilot dentro de un Codespace

1. Navegue de regreso a la página de inicio de su repositorio, haga clic en la pestaña **Code** **(1)** de su repositorio, haga clic en el botón desplegable **Add file** **(2)** y luego seleccione `+ Create new file` **(3)**.

    ![](../media/Exercise-01-v2-01.png)

2. Escriba o pegue lo siguiente en el campo de texto vacío para nombrar su archivo **(1)**.

   ```
   .devcontainer/devcontainer.json
   ```

3. En el cuerpo del nuevo archivo **.devcontainer/devcontainer.json**, agregue el siguiente contenido **(2)** y haga clic en **Commit changes** **(3)**:

   ```
   {
       // Name this configuration
       "name": "Codespace for Skills!",
       "customizations": {
           "vscode": {
               "extensions": [
                   "GitHub.copilot"
               ]
           }
       }
   }
   ```

   ![](../media/devcontainer-commit.png)
   
4. Seleccione la opción **Commit directly to the `main` branch** y luego haga clic en el botón **Commit changes**.

   ![](../media/commit-file.png)

5. Vuelva a la página de inicio de su repositorio haciendo clic en la pestaña **Code** **(1)** ubicada en la parte superior izquierda de la pantalla. Haga clic en el botón **Code** **(2)** ubicado al centro de la página.

   ![](../media/code-code.png)

6. Haga clic en la pestaña **Codespaces (1)** en el cuadro emergente y luego haga clic en el botón **Create codespace on main (2)**.

   ![](../media/create-codespace.png)

   >**Nota**: Si no aparece el mensaje emergente en el navegador para abrir Visual Studio Code, inicie Visual Studio Code manualmente desde el escritorio y ciérrelo. A continuación, vuelva al navegador, actualice la página e inicie el codespace que se creó anteriormente.

7. Aparecerá un mensaje emergente. Haga clic en **Abrir** para continuar. Posteriormente, aparecerá otra ventana emergente dentro de Visual Studio Code (VS Code), donde debe seleccionar **Instalar Extensión y Abrir URI** para continuar.

   ![](../media/open.png)

   ![](../media/innovation-1.png)

    >**Nota**: Haga clic en **Permitir** si la extensión **Github Codespaces** desea iniciar sesión con Github.

   ![](../media/inn-2.png)

8. En la esquina inferior derecha, aparecerá un mensaje emergente para iniciar sesión en GitHub.

   ![](../media/signingit.png)

   > **Nota**: Si aparece el error **No access to GitHub Copilot found**, comuníquese con `cloudlabs-support@spektrasystems.com` para obtener más ayuda.

      ![](../media/3.png)

9. A continuación, cuando aparezca la ventana emergente, haga clic en **Permitir**

   ![](../media/allow.png)

   >**Nota**: espere unos 2 minutos para que el codespace se active por sí solo.

10. Haga clic en **Authorize Visual-Studio-Code** una vez que aparezca la pestaña Authorize GitHub for VS code en el navegador.

    ![](../media/Exercise-01-v2-02.png)

11. A continuación, cuando aparezca la ventana emergente, haga clic en **Permitir**

12. Verifique que su codespace se esté ejecutando. Asegúrese de que VS Code se vea como se muestra a continuación:

    ![](../media/loaded-repo.png)

13. Haga clic en **Extensiones** **(1)** en el menú de la izquierda y la extensión **GitHub Copilot** **(2)** debería aparecer en la lista de extensiones de VS Code. Haga clic en la extensión Copilot y verifique su instalación como se muestra a continuación:

    ![](../media/verify-copilot.png)

   >**Nota**: Si la extensión GitHub Copilot no está instalada, haga clic en Instalar.

   <validation step="ccef791a-3558-4efe-be78-c5a218e874a3" />
 
14. Haga clic en **Siguiente** a continuación para pasar a la página siguiente.

### Resumen

En este ejercicio, ha creado un contenedor de desarrollo y ha agregado Copilot a la lista de extensiones.

### Ha completado el laboratorio con éxito
