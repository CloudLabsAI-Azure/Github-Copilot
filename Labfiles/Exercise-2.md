# Ejercicio 2: Explorar Sugerencias de Código Impulsadas por IA en JavaScript

### Duración Estimada: 20 minutos

Si bien GitHub Copilot ofrece recomendaciones en varios lenguajes y frameworks, destaca particularmente con Python, JavaScript, TypeScript, Ruby, Go, C# y C++. Aunque los siguientes ejemplos están en JavaScript, también deberían ser compatibles con otros lenguajes.

En este ejercicio, tendrá la oportunidad de explorar y utilizar JavaScript, guiado por el apoyo de GitHub Copilot y GitHub Copilot Chat.

>**Descargo de responsabilidad**: GitHub Copilot sugerirá automáticamente todo el cuerpo de una función en texto gris. Sin embargo, la recomendación precisa podría variar.

>**Nota**: Si no puede ver ninguna sugerencia de GitHub Copilot en VS Code, reinicie VS Code una vez e intente nuevamente.

## Objetivos del laboratorio

Será capaz de completar las siguientes tareas:

- Tarea 1: Agregar un archivo JavaScript y comenzar a escribir código
- Tarea 2: Enviar código a su repositorio desde el codespace
- Tarea 3: Mejores prácticas para usar GitHub Copilot

## Tarea 1: Agregar un archivo JavaScript y comenzar a escribir código

1. Desde la ventana Explorador de VS Code, cree un Nuevo Archivo.

   ![](../media/create-newfile.png)

2. Nombre el archivo como `skills.js` y compruebe que su nuevo archivo se vea como se muestra a continuación:

   ![](../media/name-skills.png)

3. En el archivo `skills.js`, escriba el siguiente encabezado de función y presione Enter:

   ```
   function calculateNumbers(var1, var2)
   ```
   
   > **Nota**: GitHub Copilot sugerirá automáticamente un cuerpo de función completo en texto gris. Este es un ejemplo de lo que probablemente verá; sin embargo, la recomendación precisa podría variar.

   ![](../media/skills(1).png)

4. Presione `Tab` para aceptar la sugerencia y luego presione `Ctrl + S` para guardar el archivo.

   ![](../media/skills(2).png)

## Tarea 2: Enviar código a su repositorio desde el codespace

En esta tarea, usará la Terminal de VS Code para agregar el archivo `skills.js` al repositorio de GitHub.

1. Abra la Terminal de VS Code haciendo clic en los **Puntos suspensivos (...)** **(1)**, seleccione **Terminal** **(2)** y haga clic en **Nuevo terminal** **(3)**.

   ![](../media/open-terminal.png)

2. Ejecute el siguiente comando para agregar el archivo `skills.js` al repositorio de GitHub.

   ```
   git add skills.js
   ```

3. A continuación, desde la Terminal de VS Code, confirme los cambios en el repositorio:


   ```
   git commit -m "Copilot first commit"
   ```

4. Por último, desde la Terminal de VS Code, envíe el código al repositorio:

   ```
   git push
   ```

   ![](../media/githubcopilot.png)

   >**Nota**: Espere unos 60 segundos y luego actualice la página de inicio del repositorio de GitHub para el siguiente paso.


## Tarea 3: Mejores prácticas para usar GitHub Copilot

### Verificar la extensión GitHub Copilot Chat en VS Code

1. Para verificar la extensión GitHub Copilot Chat, se deben realizar los siguientes pasos dentro de Visual Studio Code:
    - Haga clic en el ícono **Extensiones (1)** en la barra de actividades presente en el lado izquierdo de la ventana de Visual Studio Code.
    - En el cuadro de búsqueda "Buscar Extensiones en Marketplace", escriba y busque la extensión **GitHub Copilot Chat (2)**.
    - Seleccione **GitHub Copilot Chat (3)** de la lista de resultados que aparecen y verifique que **GitHub Copilot Chat** se encuentre instalado.
    - De lo contrario, haga clic en el botón **Instalar (4)**.

   ![](../media/ghc-chat-extension.png)

1. Una vez que se complete la instalación, en el panel de navegación izquierdo podrá ver el ícono de GitHub Copilot Chat como se muestra a continuación.

   ![](../media/git-chat-icon.png)

## Tarea 3.1: Ejemplo: Prepare el escenario con un objetivo de alto nivel

Esto es más útil si tiene un archivo en blanco o una base de código vacía. En otras palabras, puede ser bastante útil para preparar el terreno para el programador en pares de IA si GitHub Copilot no tiene idea de lo que usted desea construir o lograr. Es útil preparar a GitHub Copilot con una descripción general de lo que quiere que genere, antes de entrar en detalles.

Al preparar un prompt para GitHub Copilot, piense en el proceso como si estuviera teniendo una conversación con alguien: ¿Cómo debería desglosar el problema para que podamos resolverlo juntos? ¿Cómo abordaría la programación en pareja con esta persona?

1. Desde la ventana Explorador de VS Code, cree un Nuevo Archivo.

   ![](../media/E2-T3.1-S1.png)

2. Nombre el archivo `index.js` y compruebe que su nuevo archivo se vea como se muestra a continuación:

   ![](../media/E2-T3.1-S2.png)

3. Ahora, presione Ctrl + I para abrir GitHub Copilot Chat y pegue el siguiente **comentario (1)** para obtener el código y haga clic en el botón Realizar solicitud **(Entrar) (2)** y haga clic en **Aceptar (3)** para usar el código.

   ```
   /*
   Create a basic markdown editor in Next.js with the following features:
   - Use react hooks
   - Create a state for markdown with the default text "type markdown here"
   - A text area where users can write markdown 
   - Show a live preview of the markdown text as I type
   - Support for basic markdown syntax like headers, bold, and italics 
   - Use React markdown npm package 
   - The markdown text and resulting HTML should be saved in the component's state and updated in real-time 
   */
   ```

   ![](../media/ex-2-1.png)

# Tarea 3.2- Ejemplo: Intentar recibir un resultado breve de GitHub Copilot para una petición simple y específica

Una vez que haya explicado su objetivo principal al programador de pares de IA, explique el razonamiento y los procedimientos que debe seguir para alcanzar ese objetivo. Esto ayudará a GitHub Copilot a entender mejor el resultado que se pretende obtener cuando desglose las cosas. Por ejemplo, imagine que está escribiendo una receta. En lugar de escribir un párrafo en el que describa la comida que pretende preparar, dividiría el procedimiento de cocción en distintas partes.
Entonces, en lugar de pedirle a GitHub Copilot que genere una gran cantidad de código a la vez, deje que genere el código después de cada paso.

1. En el mismo archivo index.js, ingrese las siguientes instrucciones paso a paso para invertir una oración.

    ```
      // take a sentence as input
      // reverse the input sentence
      // the start of the sentence must start with a capital
      // for javascript
    ```

2. El resultado generado se vería similar a la imagen de abajo.

   ![](../media/ex-2-2.png)


## Tarea 3.3: Ejemplo: Dar a GitHub Copilot uno o dos ejemplos

No solo las personas pueden beneficiarse del aprendizaje a partir de ejemplos, sino que también puede hacerlo su programador de pares de IA. Por ejemplo, para sacar los nombres de la matriz de datos de abajo y ponerlos en una
nueva matriz:

   ```
          const data = [
        [
          { name: 'John', age: 25 },
          { name: 'Jane', age: 30 }
        ],
        [
          { name: 'Bob', age: 40 }
        ]
      ];    
   ```

1. Escriba el siguiente comentario en el chat para generar el resultado sin mostrar un ejemplo a GitHub Copilot.

   ```
    // As an illustration, pull names out of the data array  
   ```

2. Se generó un uso incorrecto de la función map.

   ![](../media/ex-2-3.png)

3. En contraste, ahora escriba los siguientes comentarios para proporcionar un ejemplo de cómo generar el resultado deseado.

    ```
      // Map through an array of arrays of objects
      // Example: Extract names from the data array
      // Desired outcome: ['John', 'Jane', 'Bob']    
    ```

4. Ahora, hemos recibido el resultado deseado. Guarde el archivo `index.js` recién creado usando las teclas de acceso directo `CTRL + S`.

   ![](../media/ex-2-4.png)

5. Abra una **Nueva terminal** para enviar el código.

6. Ejecute el siguiente comando para obtener los últimos cambios.

   ```
   git pull
   ```

1. Ejecute el siguiente comando para agregar el archivo `index.js` al repositorio de GitHub.
   
   ```
   git add index.js
   ```

8. A continuación, desde la Terminal de VS Code, confirme los cambios en el repositorio:

   ```
   git commit -m "Copilot commit"
   ```

9. Por último, desde la Terminal de VS Code, envíe el código al repositorio:

   ```
   git push
   ```

   >**Nota**: Espere unos 60 segundos y luego actualice la página de inicio de su repositorio de GitHub para el siguiente paso.

   <validation step="2a3fed6c-67bd-4fdb-93d9-acd9b65c9d19" />

10. Haga clic en **Siguiente** a continuación para pasar a la página siguiente.
    
### Resumen

En este ejercicio, ha generado con éxito código JavaScript y otras prácticas recomendadas con GitHub Copilot y GitHub Copilot Chat.

### Ha completado el laboratorio con éxito
