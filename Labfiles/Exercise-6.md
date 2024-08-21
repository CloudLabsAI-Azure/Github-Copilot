# Ejercicio 6: Usar IDEs como JetBrains IntelliJ para Java

### Duración Estimada: 20 minutos

IntelliJ IDEA es un entorno de desarrollo integrado (IDE) para Java y Kotlin diseñado para maximizar la productividad de los desarrolladores. Realiza las tareas rutinarias y repetitivas por usted al proporcionar completado de código inteligente, análisis de código estático y refactorizaciones, y le permite concentrarse en el lado positivo del desarrollo de software, lo que lo convierte no solo en una experiencia productiva sino también agradable.

GitHub Copilot, una innovadora herramienta de generación de código, se puede integrar con JetBrains IntelliJ, un IDE ampliamente utilizado para el desarrollo en Java. Esta integración mejora la experiencia de programación en Java proporcionando sugerencias de código inteligentes y autocompletado dentro de IntelliJ, aumentando la productividad y la calidad del código.

En este ejercicio, utilizará el IDE JetBrains IntelliJ Idea para Java. Instalará el complemento GitHub Copilot y creará un nuevo proyecto.

>**Descargo de responsabilidad**: GitHub Copilot sugerirá automáticamente todo el cuerpo de una función o código en texto gris. A continuación, se muestran ejemplos de lo que probablemente verá en este ejercicio, pero la sugerencia exacta puede variar.

>**Nota**: Si no puede ver ninguna sugerencia de GitHub Copilot en VS Code, reinicie VS Code una vez e intente nuevamente.

## Objetivos del laboratorio

Será capaz de completar las siguientes tareas:

- Tarea 1: Instalar el complemento GitHub Copilot y crear un nuevo proyecto en el IDE IntelliJ Idea
- Tarea 2: Crear un proyecto básico de Java
- Tarea 3: Obtener más sugerencias
- Tarea 4: Obtener código a partir de un comentario

## Tarea 1: Instalar el complemento GitHub Copilot y crear un nuevo proyecto en el IDE IntelliJ Idea

1. Vaya al escritorio y abra el IDE **IntelliJ IDEA Community**.

   ![](../media/E6-T1-S1.png)

1. En el Acuerdo de IntelliJ IDEA, marque **I confirm that I have read and accept the terms of this User Agreement (1)** y haga clic en **Continue (2)**.

   ![](../media/E6-T1-S2.png)

   >**Nota:** Cuando aparezca el cuadro para compartir datos, haga clic en **Don't Send**.

   ![](../media/E6-T1-S2.1.png)

1. En el menú de la izquierda, haga clic en **Plugins** **(1)** y seleccione **Marketplace** **(2)**. Busque **GitHub Copilot** **(3)** y, una vez que encuentre el complemento **GitHub Copilot**, haga clic en **Install** **(4)**.

   ![](../media/install-plugin.png)

   >**Nota**: En el aviso de Plugins de Terceros, haga clic en **Aceptar**.

1. Verifique que el complemento GitHub Copilot esté instalado. A continuación, debe reiniciar el IDE haciendo clic en **Restart IDE**. Haga clic en **Restart** en la ventana emergente una vez más para reiniciar el IDE.

   ![](../media/restart-ide(1).png)

1. Una vez que se reinicie el IDE **IntelliJ Idea Community**, seleccione **Projects** **(1)** en el menú de la izquierda y haga clic en **New Project** **(2)**.

   ![](../media/create-project.png)

1. En el panel de nuevo proyecto, ingrese el nombre del proyecto como **demo-copilot** **(1)**. Coloque el lenguaje como **Java** **(2)** y el sistema de compilación (Build system) como **IntelliJ** **(3)**. Para el JDK, seleccione el valor predeterminado **Download Oracle OpenJDK 22** **(4)** y haga clic en **Create** **(5)**.

   ![](../media/Exercise-06-v2-02.png)

1. Revise el proyecto **demo-copilot** creado como se muestra a continuación:

   ![](../media/demo-copilot-project.png)

## Tarea 2: Crear un proyecto básico de Java

1. Haga clic en el **ícono** como se muestra en la siguiente imagen.

   ![](../media/icon.png)

1. Haga clic en **Tools (1)**. Haga clic en GitHub Copilot y, luego, en **Login to GitHub (2)**.

   ![](../media/login.png)

1. En el cuadro de diálogo "Sign in to GitHub", para copiar el código del dispositivo y abrir la ventana de activación del dispositivo, haga clic en **Copy and Open**.

   ![](../media/ex6-copy-code.png)

1. Se abrirá una ventana de activación del dispositivo en su navegador. Pegue el **código (1)** del dispositivo que copió en el paso anterior y luego haga clic en **Continue (2)**.

   ![](../media/ex6-device-activation.png)

1. GitHub solicitará los permisos necesarios para GitHub Copilot. Para aprobar estos permisos, haga clic en **Authorize GitHub Copilot Plugin**.

1. Una vez que se hayan aprobado los permisos, su IDE de JetBrains mostrará una confirmación.

   ![](../media/Exercise-06-v2-04.png)

1. En su IDE de JetBrains, haga clic derecho en **src (1)**, seleccione **New (2)** y haga clic en **File (3)** para crear un nuevo archivo Java (*.java) denominado **Test.java**.

   ![](../media/ex6-test-java.png)

1. Cree una clase escribiendo **class Test**. Copilot sugerirá un cuerpo de clase y puede presionar la tecla **Tab** para aceptar la sugerencia.

   ![](../media/ex6-class-test.png)

1. Debajo de la llave de la función main, escriba el siguiente encabezado de función:

   ```
   int calculateDaysBetweenDates(
   ```

1. GitHub Copilot sugerirá automáticamente todo el cuerpo de la función en texto gris, como se muestra a continuación. La sugerencia exacta puede variar.

   ![](../media/ex6-days.png)

1. Presione **Tab** para aceptar la sugerencia.


## Tarea 3: Obtener más sugerencias

En ocasiones, es posible que no quiera usar ninguna de las sugerencias iniciales. Puede solicitarle a GitHub Copilot que devuelva más.

1. Elimine la función que ingresó y escriba lo siguiente nuevamente:

   ```
   int calculateDaysBetweenDates(
   ```

1. Abra GitHub Copilot.

   - En macOS, presione `Option + Enter`.

   - En Windows o Linux, presione `Alt + Enter`.
   
   >**Nota**: Si `Alt + Enter` no funciona, seleccione Github Copilot en el panel derecho como se muestra en la siguiente imagen.

   ![](../media/github.png)
   
1. Seleccione "GitHub Copilot". GitHub Copilot abrirá una nueva pestaña y sugerirá múltiples opciones, como se muestra a continuación.

   ![](../media/ex6-copilot-suggestion.png)

1. Elija una sugerencia que desee utilizar y luego haga clic en "Accept solución".

1. Si no le gusta ninguna de las sugerencias devueltas, simplemente cierre la pestaña de sugerencias.


## Tarea 4: Obtener código a partir de un comentario

GitHub Copilot puede entender mucho más contexto que la mayoría de los asistentes de código y puede generar funciones completas a partir de algo tan simple como un comentario.

1. Elimine la función que ingresó y escriba el siguiente comentario:
   
   ```
   // Identify all the images without alternate text
   // and add a red border to them
   void process(java.util.List<Image> images) {  

   ```

2. GitHub Copilot sugerirá automáticamente una implementación.
  
   ![](../media/ex6-image-suggestion.png)

   <validation step="0ad0a930-79b9-4b15-bb7a-0806f50ca3b0" />

6. Haga clic en **Siguiente** a continuación para pasar a la página siguiente.
        
### Resumen

En este ejercicio, ha configurado con éxito JetBrains IntelliJ Idea IDE para Java, ha instalado el complemento GitHub Copilot y ha explorado código básico de Java que generó las sugerencias usando Copilot.

### Ha completado el laboratorio con éxito
