# EditorHTML

EditorHTML é uma aplicação simples de linha de comando desenvolvida em C# para criar, editar e visualizar arquivos HTML de maneira interativa.

## Funcionalidades

- Criar novos arquivos HTML
- Editar conteúdo HTML em modo texto
- Visualizar arquivos HTML com destaque para elementos `<strong>`
- Interface simplificada para navegação via menu

## Requisitos

- .NET Core SDK instalado

## Como executar

1. Clone o repositório ou baixe os arquivos do projeto.
2. Abra um terminal na pasta do projeto.
3. Compile o projeto com o seguinte comando:

   ```bash
   dotnet build
   ```

4. Execute o programa com:

   ```bash
   dotnet run
   ```

## Uso

1. Ao iniciar, será exibido um menu com as seguintes opções:
   - `1 - Novo arquivo`: Inicia o modo de edição de um novo arquivo HTML.
   - `2 - Abrir`: (Ainda não implementado)
   - `0 - Sair`: Encerra o programa.

2. No modo editor:
   - Digite o conteúdo desejado.
   - Pressione `ESC` para finalizar a edição.
   - Será perguntado se deseja salvar o arquivo e o conteúdo será exibido no modo de visualização.

3. No modo visualização:
   - O conteúdo digitado será exibido com elementos `<strong>` em azul.
   - Pressione qualquer tecla para retornar ao menu principal.

## Estrutura do Projeto

- `Program.cs`: Ponto de entrada do programa.
- `Menu.cs`: Exibe o menu principal e lida com a seleção do usuário.
- `Editor.cs`: Gerencia o modo de edição do arquivo.
- `Viewer.cs`: Exibe o conteúdo HTML com formatação destacada.

## Exemplo de uso

1. Execute o programa.
2. Escolha a opção `1 - Novo arquivo`.
3. Digite:
   ```html
   <strong>Texto em negrito</strong>
   Texto normal
   ```
4. Pressione `ESC` para sair da edição.
5. Visualize o texto, onde "Texto em negrito" aparecerá em azul.