# Exercício 6: Utilização de IDEs como o JetBrains IntelliJ para Java

### Duração estimada: 20 minutos

O IntelliJ é um ambiente de desenvolvimento integrado (IDE) para Java e Kotlin, concebido para maximizar a produtividade do programador. Realiza as tarefas rotineiras e repetitivas por si, proporcionando uma conclusão de código inteligente, análise estática de código e refactorings, e permite-lhe concentrar-se no lado positivo do desenvolvimento de software, tornando-o não só produtivo, mas também uma experiência agradável.

O GitHub Copilot, uma ferramenta inovadora de geração de código, pode ser integrado no JetBrains IntelliJ, um IDE muito utilizado para o desenvolvimento Java. Esta integração melhora a experiência de codificação Java, fornecendo sugestões de código inteligentes e preenchimento automático no IntelliJ, aumentando a produtividade e a qualidade do código.

Neste exercício, irá utilizar o IDE JetBrains IntelliJ Idea para Java. Irá instalar o plugin GitHub Copilot e criar um novo projeto.

> **Nota**: O GitHub Copilot irá sugerir automaticamente um corpo de função completa ou código em texto cinzento. A seguir, apresentamos alguns exemplos do que provavelmente verá neste exercício, mas a sugestão exata pode variar.

>**Nota**: Se não conseguir ver nenhuma sugestão do GitHub Copilot no VS Code, reinicie o VS Code uma vez e tente novamente.

## Objetivos do laboratório

Poderá completar as seguintes tarefas:

- Tarefa 1: Instalar o plugin GitHub Copilot e criar um novo projeto no IntelliJ Idea IDE
- Tarefa 2: Criar um projeto Java básico
- Tarefa 3: Obter mais sugestões
- Tarefa 4: Obter código a partir de um comentário

## Tarefa 1: Instalar o plugin GitHub Copilot e criar um novo projeto no IntelliJ Idea IDE

1. Navegue até ao ambiente de trabalho e abra o IDE **IntelliJ IDEA Community**.

   ![](../../media/30-10-24(4).png)

1. No Contrato IntelliJ IDEA, assinale **I confirm that I have read and accept the terms of this User Agreement (1)** e clique em **Continue (2)**.

   ![](../../media/E6-T1-S2.png)

    >**Nota:** Quando a caixa de partilha de dados for apresentada, clique em **Don't Send**.

    ![](../../media/E6-T1-S2.1.png)

1. Clique em **Skip import**.    

1. No menu esquerdo, clique em **Plugins** **(1)** e selecione **Marketplace** **(2)**. Pesquise **GitHub Copilot** **(3)** e, quando encontrar o plugin **GitHub Copilot**, clique em **Install** **(4)**.

   ![](../../media/install-plugin.png)

   >**Nota** : No aviso de plug-ins de terceiros, clique em **Accept**.

1. Verifique se o plugin GitHub Copilot está instalado. De seguida, precisa de reiniciar o IDE clicando em **Restart IDE**. Clique em **Restart** no pop-up mais uma vez para reiniciar o IDE.

   ![](../../media/restart-ide(1).png)

1. Depois de o IDE **IntelliJ Idea Community** ser reiniciado, selecione **Projects** **(1)** no menu esquerdo e clique em **New Project** **(2)**.

   ![](../../media/create-project.png)

1. No painel do novo projeto, introduza o nome do projeto como **demo-copilot** **(1)**. Selecione o idioma como **Java** **(2)** e compile o sistema como **IntelliJ** **(3)**. Para JDK, seleccione o padrão **Download Oracle OpenJDK 22** **(4)** e clique em **Create** **(5)**.

   ![](../../media/Exercise-06-v2-02.png)

1. Reveja o projeto **demo-copilot** criado como mostrado abaixo:

   ![](../../media/demo-copilot-project.png)

## Tarefa 2: Criar um projeto Java básico

1. Clique no **ícone** conforme imagem abaixo.

   ![](../../media/icon.png)

1. Clique em **Tools (1)**. Clique em GitHub Copilot e em **Login to GitHub (2)**.

   ![](../../media/login.png)

1. Na caixa de diálogo "Sign in to GitHub", para copiar o código do dispositivo e abrir a janela de ativação do dispositivo, clique em **Copy and Open**.

   ![](../../media/ex6-copy-code.png)

1. Uma janela de ativação do dispositivo será aberta no seu browser. Cole o **code (1)** do dispositivo que copiou no passo anterior e clique em **Continue (2)**.

   ![](../../media/ex6-device-activation.png)

1. O GitHub irá solicitar as permissões necessárias para o GitHub Copilot. Para aprovar estas permissões, clique em **Authorize GitHub Copilot Plugin**.

1. Após a aprovação das permissões, o seu IDE JetBrains irá mostrar uma confirmação.

   ![](../../media/Exercise-06-v2-04.png)

1. No seu IDE JetBrains, clique com o botão direito do rato em **src (1)**, seleccione **New (2)** e clique em **File (3)** para criar um novo ficheiro Java (*.java) denominado **Test.java**.

   ![](../../media/ex6-test-java.png)

1. Crie uma classe digitando **class Test**. O Copilot irá sugerir um corpo de classe, e poderás premir **tab** para aceitar a sugestão.

   ![](../../media/ex6-class-test.png)

1. Abaixo do parêntesis recto da função principal, introduza o seguinte cabeçalho da função:

    ```
    int calculateDaysBetweenDates(
    ```

1. O GitHub Copilot irá sugerir automaticamente um corpo de função inteiro em texto cinzento, como se mostra abaixo. A sugestão exata pode variar.

   ![](../../media/ex6-days.png)

1. Prima **Tab** para aceitar a sugestão.

## Tarefa 3: Obter mais sugestões

Por vezes, pode não querer utilizar nenhuma das sugestões iniciais. Pode pedir ao GitHub Copilot para devolver mais.

1. Remova a função introduzida e volte a introduzir o seguinte:

    ```
    int calculateDaysBetweenDates(
    ```

1. Abra o GitHub Copilot.

    - No macOS, prima `Option + Enter`.

    - No Windows ou Linux, prima `Alt + Enter`.

    >**Nota**: Se 'Alt + Enter' não estiver a funcionar, selecione Github Co-pilot no painel direito, como mostra a imagem abaixo.

    ![](../../media/github.png)

1. Selecione "Open Copilot". O GitHub Copilot abrirá um novo separador e sugerirá várias opções, conforme mostrado abaixo.

   ![](../../media/ex6-copilot-suggestion.png)

1. Escolha uma sugestão que pretende utilizar e clique em "Accept solution".

1. Caso não goste de nenhuma das sugestões devolvidas, basta fechar o separador sugestões.


## Tarefa 4:  Obter código a partir de um comentário

O GitHub Copilot pode compreender significativamente mais contexto do que a maioria dos assistentes de código e pode gerar funções inteiras a partir de algo tão simples como um comentário.

1. Remova a função introduzida e digite o seguinte comentário:

   ```
   // Identify all the images without alternate text
   // and add a red border to them
   void process(java.util.List<Image> images) {
   ```

2. O GitHub Copilot irá sugerir automaticamente uma implementação.

   ![](../../media/ex6-image-suggestion.png)

 <validation step="364115e7-deff-4c32-96e9-fa5d2122a86f" />

3. Clique em **Próximo** abaixo para passar para a página seguinte.

### Resumo

Neste exercício, configurou com sucesso o IDE JetBrains IntelliJ Idea para Java, instalou o plugin GitHub Copilot e explorou o código Java básico que produziu as sugestões utilizando o Copilot.

### Concluiu o laboratório com sucesso