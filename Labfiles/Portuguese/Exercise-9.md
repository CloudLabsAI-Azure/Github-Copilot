# Exercício 9: Gerar documentação utilizando o GitHub Copilot [opcional]

### Duração estimada: 10 minutos

O GitHub Copilot pode ajudar a agilizar o processo de geração de documentação para os seus projetos de software. Auxilia na geração automática de comentários de código, na criação de documentação Markdown, no fornecimento de modelos para secções comuns, na garantia de consistência gramatical e de estilo e na referência cruzada de código e documentação. Esta ferramenta pode poupar tempo e melhorar a qualidade da documentação do seu projeto, tornando-a mais acessível e fácil de utilizar.

Neste exercício, irá gerar documentação utilizando o GitHub Copilot.

>**Aviso**: O GitHub Copilot irá sugerir automaticamente um corpo de função completa ou código em texto cinzento. Exemplos do que provavelmente verá neste exercício, mas a sugestão exata pode variar.

>**Nota**: Se não conseguir ver nenhuma sugestão do GitHub Copilot no VS Code, reinicie o VS Code uma vez e tente novamente.


## Objetivos do laboratório

Poderá completar as seguintes tarefas:

- Tarefa 1: Gerar um arquivo README com o GitHub Copilot usando comentários
- Tarefa 2: Enviar código para seu repositório a partir do Codespace

## Tarefa 1: Gerar um arquivo README com o GitHub Copilot usando comentários

1. No Codespace, na janela do VS Code Explorer, crie um novo arquivo e nomeie-o como `Document.md`.

    ![](../../media/chat-code-new.png)

1. Pressione `CTRL + I` para fornecer instruções ao GitHub Copilot.

1. Forneça a seguinte instrução (1) para que o GitHub Copilot crie um documento demonstrando a criação de um aplicativo Node.js de exemplo. Pressione **Send (2)**.

    ```
    Create a markdown document for a sample Node.js application with mermaid diagrams and reference links
    ```

    ![](../../media/hub20.png)

1.  O Copilot fornecerá uma resposta, e você poderá reve-la. Clique em **Accept**, e pressione `CTRL + S` para salvar o arquivo.

    ![](../../media/hub21.png)

1.  Observe como o Copilot gerou os diagramas Mermaid e incluiu os links de referência conforme nossa solicitação.

    ![](../../media/hub22.png)
    
    ![](../../media/hub23.png)


## Tarefa 2: Enviar código para seu repositório a partir do Codespace

1. Execute o seguinte comando para adicionar os arquivos:

    ```
    git add .
    ```
1. Execute o seguinte comando para confirmar (commit) os arquivos:

    ```
    git commit -m "files"
    ```

1. Execute o seguinte comando para enviar (push) todos os arquivos para o repositório:

    ```
    git push
    ```

## Resumo

Neste exercício, gerou com sucesso um documento utilizando o GitHub Copilot Chat e enviou os arquivos para o seu repositório.

### Concluiu o laboratório com sucesso. Clique em **Próximo >>** para prosseguir com o próximo exercício.