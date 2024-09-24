# Desafio Front-End | Zion Church

### Objetivo do Desafio: 

Desenvolver uma aplicação web de "comunidade zion church" onde os membros da comunidade possam criar e visualizar postagens, interagir com comentários e visualizar um feed de notícias em tempo real. O foco é avaliar habilidades de desenvolvimento com Next.js, autenticação, integração com Websockets e boas práticas de código.

--------------

### Descrição do Projeto:

Você deve criar uma aplicação web que permita aos usuários da Zion Church interagirem de maneira simples e intuitiva, conforme as funcionalidades descritas abaixo:

#### 1. Página de Login e Registro:

> Criar um sistema de autenticação simples utilizando e-mail e senha. Após o login, o usuário deve ser redirecionado para o feed principal.

Você pode usar NextAuth para gerenciar a sessão e deixar 2 usuários "hard-coded" para logar. **Você se destarará se implementar um Auth com Clerk / StackAuth / Firebase / Supabase / Cognito / etc.**


#### 2. Feed de Postagens (Real-time):

> Exibir um feed com as postagens mais recentes de todos os usuários. Cada postagem deve exibir o nome do autor, conteúdo do post, e a data/hora da postagem. O feed deve ser atualizado em tempo real usando Websockets quando novos posts forem adicionados.


#### 3. Criação e Reação em Postagens:

> Permitir que o usuário autenticado crie novas postagens com um campo de texto. As postagens devem aparecer automaticamente no feed sem necessidade de recarregar a página.

> Permitir que os usuários comentem nas postagens. Os comentários também devem ser atualizados em tempo real.


--------------

### Requisitos técnicos:

1. Next.js
2. Autenticação (com NextAuth e provider de auth)
3. Websockets
4. Estado Global (ContextAPI)
5. Estilização com Tailwind CSS ou StyledComponents
6. Boas Práticas

--------------

### Critérios de Avaliação:

1. Qualidade do Código
2. Funcionalidade
3. Experiência do Usuário
4. Uso de Websockets
5. Documentação (README)

--------------


### Layout do Figma:

https://www.figma.com/design/BkomH2qiwzoXDw8lRtIf2Z/Untitled?node-id=3-39&t=NnN1AKAHkVdpNLtD-1

