# Exercício 1: Desfrute de Codespaces com VS Code para Copilot

### Duração estimada: 15 minutos

O GitHub Copilot é como um programador a pares de IA concebido para tornar a escrita de código mais fácil e rápida. Extrai contexto de comentários e código para sugerir linhas individuais e funções completas. O GitHub Copilot é baseado em Codex, um modelo de linguagem generativa pré-treinado criado pela OpenAI.

**O Copilot é compatível com uma grande variedade de editores de código, como o Neovim, JetBrains IDE, Visual Studio e VS Code.**

Além disso, o GitHub Copilot está treinado em todas as linguagens que podem ser encontradas nos repositórios públicos. A quantidade e variedade de dados de treino para cada linguagens de programação podem ter impacto na qualidade das recomendações obtidas.

**GitHub Codespace** é um ambiente de desenvolvimento alojado na nuvem. Pode personalizar o seu projeto para GitHub Codespaces enviando ficheiros de configuração para o seu repositório (geralmente conhecido como Configuração como Código), que cria uma configuração de codespace repetível para todos os utilizadores do seu projeto.

A utilização do Copilot num Codespace demonstra sem esforço a simplicidade de começar com as ferramentas abrangentes de [Escrita de Código Colaborativa](https://github.com/features#features-collaboration).

Neste exercício, terá a tarefa de criar um container. Especificará determinadas extensões ou configurações a utilizar ou instalar no seu Codespace. Como parte deste processo, certifique-se de que inclui o Copilot na sua lista de extensões.

## Objetivos do laboratório

Poderá completar as seguintes tarefas:

- Tarefa 1: Activar o Copilot dentro de um Codespace

## Tarefa 1: Ativar o Copilot dentro de um codespace

1. Navegue de volta para a página inicial do seu repositório, clique no separador **Code** **(1)** do seu repositório, clique no botão pendente **Add file** **(2)** e selecione `+ Create new file` **(3)**.

   ![](../../media/Exercise-01-v2-01.png)

1. Digite ou cole o seguinte no campo de texto vazio para nomear o seu ficheiro **(1)**.

    ```
    .devcontainer/devcontainer.json
    ```

1. No corpo do novo ficheiro **.devcontainer/devcontainer.json**, adicione o seguinte conteúdo **(2)** e clique em **Commit changes** **(3)**:

   ```
   {
       // Name this configuration
       "name": "Codespace for Skills!",
       "customizations": {
           "vscode": {
               "extensions": [
                   "GitHub.copilot",
                   "hashicorp.terraform"
               ]
           }
       },
       "features": {
          "ghcr.io/devcontainers/features/terraform:1": {},
          "ghcr.io/devcontainers/features/azure-cli:1": {}
      }
   }
   ```

   ![](../../media/c14.png)

1. Selecione a opção **Commit directly to the `main` branch** e clique no botão **Commit changes**.

   ![](../../media/commit-file.png)

1. Navegue de volta para a página inicial do seu repositório clicando no separador **Code** **(1)** localizado no canto superior esquerdo do ecrã. Clique no botão **Code** **(2)** localizado no meio da página.

   ![](../../media/code-code.png)

1. Clique no separador **Codespaces (1)** na caixa que aparece e, em seguida, clique no botão **Create codespace on main (2)**.

   ![](../../media/create-codespace.png)

   >**Nota**: Se o pedido de pop-up não aparecer no browser para abrir o código do Visual Studio, inicie manualmente o código do Visual Studio na área de trabalho e feche-o. De seguida, volte ao browser, atualize a página e inicie o codespace que foi criado anteriormente.

1. Encontrará um prompt pop-up. Clique em **Abrir** para continuar. Posteriormente, surgirá outra janela pop-up dentro do Visual Studio Code (VS Code), onde deverá selecionar **Install Extension and Open URI** para continuar.

   ![](../../media/p1.png)

   ![](../../media/p2.png)

   >**Nota**: Clique em **Allow** se a extensão **Github Codepsaces** pretender iniciar sessão utilizando o Github.

   ![](../../media/inn-2.png)

1. No canto inferior direito, receberá um pedido para entrar no GitHub.

   ![](../../media/c2.png)

1. Clique em **Open** para abrir o Visual Studio Code

   ![](../../media/c3.png)

1. De seguida, assim que o pop-up aparecer, clique em **Allow**

   ![](../../media/loaded-repo.png)

1. Clique em **Continue** quando Selecionar usuário para autorizar o Visual Studio Code aparecer no navegador.

    ![](../../media/p3.png)

1. De seguida, assim que o pop-up aparecer, clique em **Abrir**

    ![](../../media/p4.png)

1. Verifique se o seu codespace está em execução. Certifique-se de que o código VS está como mostrado abaixo:

    ![](../../media/loaded-repo.png)

1. Clique em **Extensions** **(1)** no menu esquerdo, e a extensão **GitHub Copilot** **(2)** deverá aparecer na lista de extensões do VS Code. Clique na extensão Copilot e verifique a sua instalação como se mostra abaixo:

    ![](../../media/verify-copilot.png)

    >**Nota**: Se a extensão GitHub Copilot não estiver instalada, clique em Instalar.

 <validation step="2c3e393f-eade-43e1-a96a-f8ea659b3047" />

1. Clique em **Próximo** abaixo para passar para a página seguinte.

### Resumo

Neste exercício, criou um desenvolvimento container e adicionou o Copilot à lista de extensões.

### Concluiu o laboratório com sucesso
