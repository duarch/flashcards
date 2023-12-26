# flashcards
App in Angular for flashcards



### Estrutura do Projeto:

1. **Componentes:**
   - `AppComponent`: O componente raiz que contém o roteamento e a barra de navegação, se houver.
   - `FlashCardListComponent`: Exibe a lista de grupos de flashcards e permite a criação de novos grupos.
   - `FlashCardGroupComponent`: Mostra os detalhes de um grupo específico de flashcards, exibindo os cartões e permitindo sua edição.
   - `FlashCardComponent`: Representa um cartão individual, exibindo a pergunta e resposta. Terá modos de edição e visualização.

2. **Serviços:**
   - `AuthService`: Gerencia a autenticação de usuários, criação de contas e autorização para salvar grupos privados.
   - `FlashCardService`: Lida com as operações dos flashcards, como criar, editar, excluir e recuperar grupos e cartões.

3. **Módulos:**
   - `AppModule`: Principal módulo da aplicação.
   - `RoutingModule`: Módulo para roteamento entre componentes.

4. **Roteamento:**
   - Configurar as rotas para os diferentes componentes, como a lista de flashcards, página de detalhes do grupo e página de cartões.

### Componentes Necessários:

1. **FlashCardListComponent:**
   - Exibirá a lista de grupos de flashcards.
   - Permitirá a criação de novos grupos.
   - Terá seções para grupos públicos e privados (para usuários logados).
   - Opções para criar novos grupos e navegar para os detalhes de cada grupo.

2. **FlashCardGroupComponent:**
   - Exibirá os detalhes de um grupo específico de flashcards.
   - Permitirá a edição do título do grupo.
   - Exibirá a lista de cartões dentro do grupo.
   - Opções para adicionar novos cartões, editar e excluir cartões existentes.

3. **FlashCardComponent:**
   - Exibirá um cartão individual, com a pergunta e resposta.
   - Modo de edição para alterar a pergunta e resposta usando Markdown.
   - Modo de visualização para girar ou revelar o cartão.

4. **AuthService:**
   - Implementará a lógica de autenticação e gerenciamento de contas de usuários.
   - Permitirá a criação de contas e login de usuários.
   - Verificará a autenticação para permitir o acesso aos grupos privados.

5. **FlashCardService:**
   - Lidará com as operações de CRUD (criar, ler, atualizar, excluir) para grupos de flashcards e cartões.
   - Salvará e recuperará os dados dos grupos de flashcards no backend (se houver).

Essa é uma estrutura básica e simplificada. Você pode expandi-la conforme sua necessidade, adicionando funcionalidades como a integração com um backend para persistência de dados, validações, notificações, entre outras melhorias.
