# Taller de Innovación de GitHub Copilot

### Duración Total Estimada: 4 Horas

## Descripción General

El propósito de este laboratorio es explorar cómo las herramientas de IA como GitHub Copilot y GitHub Codespaces mejoran el proceso de desarrollo. Al proporcionar sugerencias contextuales y crear entornos de desarrollo consistentes alojados en la nube, estas herramientas agilizan la codificación y mejoran la eficiencia. El laboratorio se centra en varias características y aplicaciones de GitHub Copilot, demostrando cómo puede ayudar a completar el código en tiempo real, a detectar errores y a optimizar diferentes lenguajes de programación y tareas de desarrollo.

## Objetivo

Al finalizar este laboratorio, mejorará su flujo de trabajo de codificación aprovechando herramientas impulsadas por IA. Podrá:

- **Aprovechar Codespaces con VS Code para Copilot**: Este ejercicio práctico sugiere código a partir de comentarios y contexto, admite varios editores y lenguajes y se integra con GitHub Codespaces para la programación colaborativa. Como resultado de habilitar Copilot en Codespaces, experimentará una mayor productividad con sugerencias de código en tiempo real, una mejor calidad del código y una aceleración del aprendizaje y la incorporación.
- **Explorar Sugerencias de Código Impulsadas por IA en JavaScript**: Este ejercicio práctico tiene como objetivo examinar cómo la IA mejora la codificación en JavaScript con complementos en tiempo real, la detección de errores, las optimizaciones y las mejoras de eficiencia. Al habilitar Copilot en un Codespace, experimentará una mayor productividad con sugerencias de código en tiempo real mientras añade y escribe un archivo JavaScript, agilizando el proceso de enviar código a su repositorio y adhiriéndose a las mejores prácticas, mejorando la calidad general del código y reduciendo los errores.
- **Explorar Python con GitHub Copilot**: Este ejercicio práctico tiene como objetivo ofrecer excelentes sugerencias para lenguajes como Python, JavaScript, Ruby y más, y ayuda con las consultas a bases de datos. Como resultado de este ejercicio, habrá agregado con éxito el código del método Python con sugerencias en tiempo real de GitHub Copilot, habrá visto varias sugerencias de código en la pestaña Copilot y habrá enviado el código refinado a su repositorio desde VS Code Codespace.
- **Usar GitHub Copilot Chat para generar código ARM y Terraform con Copilot**: Este ejercicio práctico tiene como objetivo proporcionar asistencia de programación directamente dentro de los IDE compatibles, ofreciendo sugerencias de código, explicaciones, pruebas unitarias y correcciones de errores. Habilitar Copilot en Codespaces dará como resultado una mayor productividad con sugerencias de código en tiempo real y una mejor calidad del código mientras se generan scripts ARM, Terraform y PowerShell para implementar recursos en Azure.
- **Usar GitHub Copilot para Refactorizar Código**: Este ejercicio práctico tiene como objetivo mejorar la calidad del código mediante la reestructuración para mejorar la legibilidad, el mantenimiento y el rendimiento sin alterar el comportamiento externo, reduciendo la deuda técnica y los errores. Al utilizar GitHub Copilot para refactorizar el código y emplear Copilot Chat con el código, se mejora la calidad y la productividad del código. Este ejercicio también facilita una mejor comprensión del código refactorizado, acelera la creación de pruebas unitarias y agiliza el envío de código a su repositorio.
- **Usar IDEs como JetBrains IntelliJ para Java**: Este ejercicio práctico tiene como objetivo mejorar la codificación en Java en IntelliJ ofreciendo sugerencias inteligentes y autocompletado, elevando la productividad y la calidad del código. Instale el complemento GitHub Copilot y cree un proyecto Java básico en IntelliJ IDEA. Utilice Copilot para obtener sugerencias de código mejoradas y generar código a partir de comentarios.
- **Mejorar la Accesibilidad Web con GitHub Copilot Chat y Accessibility Insights**: Este ejercicio práctico tiene como objetivo acelerar la codificación con sugerencias impulsadas por IA, mientras que Accessibility Insights for Web garantiza un contenido web inclusivo y accesible. Al completar el ejercicio, habrás configurado correctamente la extensión Accessibility Insights for Web en Microsoft Edge, que ahora le permite evaluar y abordar de manera eficaz los problemas de accesibilidad en proyectos web.
- **Usar GitHub Copilot para Código T-SQL y YAML [Opcional]**: Este ejercicio práctico tiene como objetivo aprovechar GitHub Copilot para generar código en T-SQL y YAML, utilizando comentarios para guiar sus sugerencias. Como resultado de completar el ejercicio, el usuario habrá generado con éxito una consulta SQL y una configuración YAML utilizando GitHub Copilot, aprovechando los comentarios para guiar la asistencia de la IA.
- **Generar Documentación con GitHub Copilot [Opcional]**: Este ejercicio práctico tiene como objetivo agilizar la documentación mediante la generación automática de comentarios, Markdown y garantizar la coherencia, mejorando la accesibilidad del proyecto. Como resultado de este ejercicio, generará documentación de manera eficaz con GitHub Copilot.
- **Trabajar con Copilot para Machine Learning [Opcional]**: Este ejercicio práctico tiene como objetivo utilizar GitHub Copilot con frameworks de ML para tareas como el preprocesamiento de datos, la creación de modelos y la evaluación. Al final de este ejercicio, habrá configurado un entorno, experimentado con el autocompletado de código, aplicado técnicas matemáticas y de machine learning, realizado la visualización y la transformación de datos, y entrenado un modelo de ejemplo.
- **Crear un Minijuego con GitHub Copilot [Opcional]**: Este ejercicio práctico tiene como objetivo construir un minijuego, perfeccionando las habilidades de Python en el desarrollo de aplicaciones de consola. Después de completar el ejercicio, habrá configurado con éxito su entorno, probado su GitHub Codespace para asegurarse de que funciona correctamente y creado la lógica del juego, proporcionando una configuración completamente operativa para su proyecto.

## Requisitos previos

Conocimientos básicos de **Visual Studio Code** y **lenguajes de programación** populares como Python, Javascript, C#, etc.

## Arquitectura

GitHub Copilot es una herramienta de completado de código impulsada por IA que ayuda a los desarrolladores sugiriendo fragmentos de código y completando el código según el contexto proporcionado. GitHub Copilot Chat complementa esto ofreciendo una interfaz de chat interactiva donde los desarrolladores pueden hacer preguntas y recibir sugerencias de código y asistencia para la depuración. Integrado con Visual Studio Code Codespaces, GitHub Copilot se beneficia de los entornos de desarrollo alojados en la nube, lo que garantiza la coherencia y la confiabilidad desde cualquier lugar. Para mejorar el desarrollo web, Accessibility Insights for Web ayuda a identificar y resolver problemas de accesibilidad, garantizando aplicaciones web inclusivas. GitHub Copilot admite varios lenguajes de programación como Python, JavaScript y C#, lo que lo convierte en una herramienta versátil para una amplia gama de tareas de programación.

## Diagrama de Arquitectura

   ![](../media/arch02.PNG)

## Explicación de los Componentes

1. **GitHub Copilot**: Una herramienta de completado de código impulsada por IA que ayuda a los desarrolladores sugiriendo fragmentos de código y completando el código según el contexto proporcionado.

1. **GitHub Copilot Chat**: Una interfaz de chat interactiva que permite a los desarrolladores hacer preguntas y recibir sugerencias de código y asistencia de depuración de GitHub Copilot.

1. **Codespaces**: Visual Studio Code Codespaces proporciona entornos de desarrollo alojados en la nube a los que se puede acceder desde cualquier lugar, lo que garantiza la coherencia y la confiabilidad.

1. **Accessibility Insights for Web**: Una extensión del navegador que ayuda a los desarrolladores a encontrar y solucionar problemas de accesibilidad en aplicaciones web.

1. **Lenguajes de programación**: Son herramientas que se utilizan para escribir instrucciones que las computadoras deben ejecutar, como Python, Javascript, C#, etc.

# Primeros Pasos con el Laboratorio

1. Puede ver un escritorio de máquina virtual 💻 (**LABVM**) cargado en la parte izquierda de su navegador. Use esta máquina virtual durante todo el taller para realizar el laboratorio. También puede conectarte a la máquina virtual mediante cualquier cliente RDP utilizando las credenciales de **LABVM** proporcionadas en la pestaña **Ambiente**.
   
   ![](../media/190625(01).png)

1. Una vez que estés en la pestaña **Entorno (1)**, desplázate hacia abajo y encontrarás **nombre de usuario de github y contraseña de github (2)**
 
   ![](../media/190625(02).png)


## Utilizando la función de ventana dividida

1. Para su conveniencia, puede abrir la guía del laboratorio en una ventana separada seleccionando el botón de ventana dividida en la esquina superior derecha.

   ![](../media/190625(03).png)

## Utilizando la función de acercar/alejar

1. Para ajustar el nivel de zoom en la página del entorno, haz clic en el ícono A↕ : 100% ubicado junto al temporizador en el entorno del laboratorio.

   ![](../media/190625(04).png)


## Iniciar Sesión en GitHub
1. En el escritorio de LABVM, busque **Microsoft Edge** **(1)**, haga clic en el navegador **Microsoft Edge** **(2)**.

   ![](../media/Edge.png)

1. Navegue a la página de inicio de sesión de GitHub utilizando la URL proporcionada a continuación:
   ```
   https://github.com/login
   ```
   
1. En la pestaña **Iniciar sesión en GitHub**, verá la pantalla de inicio de sesión. Ingrese su nombre de usuario de GitHub como **<inject key="GitHub User Name" enableCopy="true"/>** **(1)**, luego haga clic en
**Sign in with your identity provider** **(2)**.

   ![](../media/github-logina.png)
          
1. Haz clic en Continue en la página **Single sign-on to CloudLabs Organizations** para continuar.

   ![](../media/github-loginb.png)

1. Verás la pestaña** **Sign in** Aquí, ingresa tus credenciales de Azure Entra:

   - **Email/Username:** <inject key="AzureAdUserEmail"></inject>

      ![Enter Your Username](../media/login1.png)

1. A continuación, proporcione su contraseña para iniciar sesión:

   - **Password:** <inject key="AzureAdUserPassword"></inject>

      ![Enter Your Password](../media/login2.png)

1. Si se le solicita que permanezca conectado, puede hacer clic en **No**.

1. Ahora has iniciado sesión en GitHub con éxito y has sido redirigido a la página de inicio de GitHub.

      ![](../media/190625(05).png)

1. Haga clic en **Copiar enlace** y péguelo dentro de LabVM en el navegador Edge donde haya iniciado sesión en GitHub en los pasos anteriores.

   <!-- For start course, run in JavaScript:
   'https://github.com/new?' + new URLSearchParams({
     template_owner: 'skills',
     template_name: 'copilot-codespaces-vscode',
     owner: '@me',
     name: 'skills-copilot-codespaces-vscode',
     description: 'My clone repository',
     visibility: 'public',
   }).toString()
   -->

   ```
   https://github.com/new?template_owner=skills&template_name=copilot-codespaces-vscode&owner=%40me&name=skills-copilot-codespaces-vscode&description=My+clone+repository&visibility=public
   ```

1. En la nueva pestaña, la mayoría de los campos estarán rellenados automáticamente. Solo actualiza el** **Owner** **a** **Cloudlabs-Enterprises** **(1)**, cambia el nombre del repositorio a **skills-copilot-codespaces-vscode-<inject key="Deployment-id" enableCopy="false"/>** **(2)** para que sea único, y luego haz clic en **Create repository** **(3)** **para continuar.

   ![](../media/forka.png)

1. Después de crear su nuevo repositorio, espere unos 20 segundos y luego actualice la página.

   ![](../media/190625(06).png)

1. Una vez que se haya creado el repositorio, haz clic en tu foto de perfil y luego selecciona **Your organizations**.

   ![](../media/organization.png)

1. En Your organization, selecciona **Codespaces** desde el panel de navegación izquierdo.

   ![](../media/codespace.png)

1. Desplácese hacia abajo y asegúrese de que **Visual Studio Code** esté seleccionado en **Editor preference** .

     ![](../media/vscode1.png)

1. Ahora, haga clic en **Next** en la esquina inferior derecha para pasar a la página siguiente.

Este laboratorio práctico demuestra cómo GitHub Copilot y GitHub Codespaces mejoran el desarrollo a través de sugerencias de código en tiempo real y entornos de nube consistentes.

## Contacto de Soporte

1. El equipo de soporte de CloudLabs está disponible las 24 horas del día, los 7 días de la semana, los 365 días del año, por correo electrónico y chat en vivo para garantizar una asistencia sin inconvenientes en cualquier momento. Ofrecemos canales de soporte dedicados diseñados específicamente para estudiantes e instructores, garantizando que todas sus necesidades se aborden de manera rápida y eficiente.

   Contactos de Soporte para Estudiantes:

   - Soporte por Correo Electrónico: cloudlabs-support@spektrasystems.com
   - Soporte por Chat En Vivo: https://cloudlabs.ai/labs-support

1. Ahora, haga clic en Siguiente en la esquina inferior derecha para pasar a la página siguiente.
   
## ¡¡Feliz Aprendizaje!!
