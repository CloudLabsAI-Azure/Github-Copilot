# Exercício 3: Explorar o Python com o GitHub Copilot: sugestões de código inteligente

### Duração estimada: 30 minutos

O GitHub Copilot acelera a criação de scripts usando linguagens de programação gerando código baseado em IA e ferramentas inteligentes. Ao analisar o contexto e os comentários, o Copilot gera código e oferece sugestões dinâmicas para melhorias e otimizações. Além da geração de código, o Copilot disponibiliza recursos avançados, como autocompletação, expansão de código e sugestões para aprimorar o código existente ou introduzir novas funcionalidades.

>**Aviso**: Um corpo de função inteiro será sugerido automaticamente pelo GitHub Copilot em texto cinza. Aqui está um exemplo do que você provavelmente verá; no entanto, a recomendação exata pode variar.

## Objetivos do laboratório

Neste laboratório irá completar as seguintes tarefas:

- Tarefa 1: Desenvolver um script Python para implementar uma calculadora
- Tarefa 2: Explorar as ferramentas do GitHub Copilot

## Tarefa 1: Desenvolver um script Python para implementar uma calculadora

1. Na janela do Explorer do VS Code, crie um **Novo Arquivo**.

   ![](../media/py10.png)

1. Nomeie o arquivo como `app.py` e verifique se o seu novo arquivo está como mostrado abaixo:

   ![](../media/app1.png)

1. Agora pressione `Ctrl + I` para abrir o GitHub Copilot Chat e cole os seguintes **comments (1)** e clique em > ou pressione **Enter (2)**. O Copilot fornecerá uma resposta, e você pode revisá-la e clicar em **Accept (3)**. Também é possível ignorar **Discard** a sugestão conforme mostrado na imagem abaixo.
   
   ```
   Create a simple calculator that can add, subtract, multiply or divide depending upon the input from the user.
   ```

   ![](../media/hub66.png)

1. Pressione `CTRL + S` para salvar o arquivo.

1. Clique na **reticências (1)** no topo, clique em **Terminal (2)** e selecione **New Terminal (3)**.

   ![](../media/openterminal.png)

1. Execute o aplicativo com o comando **python app.py** no terminal e verifique se o output foi gerado.

   ![](../media/image.png)   

      > **Parabéns** por concluir a tarefa! Agora, é hora de validá-la. Aqui estão os passos:
      > - Clique no botão Validar para a tarefa correspondente. Se você receber uma mensagem de sucesso, pode prosseguir para a próxima tarefa.
      > - Se não, leia atentamente a mensagem de erro e repita o passo, seguindo as instruções no guia do laboratório.
      > - Se precisar de assistência, entre em contato conosco pelo e-mail cloudlabs-support@spektrasystems.com. Estamos disponíveis 24/7 para ajudar você.

      <validation step="37a79ae8-73af-4ce6-a2f0-c3895b352cd3" />

### Tarefa 2: Explorar as ferramentas do GitHub Copilot

Ao aproveitar o código gerado anteriormente, você explorará ferramentas específicas fornecidas pelo Copilot que simplificam tarefas importantes.

1. Pressione `CTRL + A` para selecionar todo o código.

1. Clique com o botão direito no código selecionado, selecione **Copilot (1)** e escolha **Editor Inline Chat (2)**.

      ![](../media/app.py.png)

1. A janela seguinte solicita que você sugira melhorias que gostaria de fazer no código. Cole os seguintes **comentários (1)** e clique em > ou pressione **Enter (2)**. O Copilot fornecerá uma resposta, e você pode revisá-la e clicar em **Aceitar (3)**. Também pode ignorar **Discard** a sugestão conforme mostrado na imagem abaixo.

   ```
   Include calculation of percentages
   ```
   
   ![](../media/py4.png)

1. Pressione `CTRL + S` para salvar o arquivo.

1. Clique nas **reticências (1)** no topo, clique em **Terminal (2)** e selecione **New Terminal (3)**.

      ![](../media/openterminal.png)
   
1. Execute o aplicativo com o comando **python app.py** no terminal e verifique se o output foi gerado.

      ![](../media/pythonapp.png)

1. Selecione o código novamente e clique com o botão direito sobre o código selecionado, selecione **Copilot (1)** e escolha **Explain (2)**.

   ![](../media/explain.png)

1. Isso abrirá o GitHub Copilot Chat à direita, oferecendo uma explicação detalhada do código, conforme mostrado abaixo.

      ![](../media/hub65.png)

1. Selecione o código novamente e clique com o botão direito sobre o código selecionado, selecione **Copilot (1)** e escolha **Fix (2)**.

   ![](../media/fix.png)

1. O GitHub Copilot usará automaticamente o comentário `/fix` para propor melhorias potenciais em partes específicas do código para aprimoramento. Clique em **Accept** para aplicar as correções no seu código.

      ![](../media/py7.png)

1. Selecione o código novamente e clique com o botão direito sobre o código selecionado, selecione **Copilot (1)** e escolha **Generate Docs (2)**.

      ![](../media/docs.png)

1. O GitHub Copilot usará automaticamente o comentário `/doc` para fornecer uma explicação detalhada de uma linha específica de código. Clique em **Accept** para obter uma compreensão mais profunda enquanto reve o código.

      ![](../media/py8.png)

1. Selecione o código novamente e clique com o botão direito sobre o código selecionado, selecione **Copilot (1)** e escolha **Generate Tests(2)**.

      ![](../media/tests1.png)

1. O GitHub Copilot usará automaticamente o comentário `/tests`. Clique em **Accept**.

      ![](../media/c9.png)

1. Pressione `CTRL + S` para salvar o arquivo.       

1. Isso abrirá um novo arquivo chamado **test_app.py**, exibindo os casos de teste.

      ![](../media/testapp7.png)



### Resumo

Neste exercício, concluiu com sucesso a tarefa de utilizar Python em conjunto com o GitHub Copilot e fê-lo com o benefício de receber várias sugestões.

### Concluiu o laboratório com sucesso