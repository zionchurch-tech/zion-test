# Desafio Back-End | Zion Church

### Objetivo do Desafio: 

Desenvolver uma aplicação web de "comunidade zion church" onde os membros da comunidade possam criar e visualizar postagens, interagir com comentários e visualizar um feed de notícias em tempo real. O foco é avaliar habilidades de desenvolvimento com JavaScript, autenticação, integração com Websockets e boas práticas de código.

### Descrição do Projeto:

Você deve criar uma aplicação web que permita aos usuários da Zion Church interagirem de maneira simples e intuitiva, conforme as funcionalidades descritas abaixo:

--------------


### 🗒️ User Story:
> Como membro da comunidade Zion Church, quero poder criar uma conta, acessar um feed de postagens, interagir (curtir/comentar), enviar mensagens em tempo real para outros membros,
para que eu possa me conectar, compartilhar experiências e fortalecer minha fé junto à comunidade.


--------------


### 🔍 Detalhes do escopo do projeto:


#### 1. Login e Registro:

Crie os endpoints necessários para o usuário se registrar, fazer login na plataforma e fazer reset de senha. Pense em uma autenticação simples utilizando e-mail e senha. 

> Você pode usar uma lib para Auth e para gerenciar a sessão, como Supabase / Firebase / Cognito, etc.
**Você se destacará se implementar Auth0 com Google ou Facebook**


#### 2. Feed de Postagens (Real-time):


> Exibir um feed com as postagens mais recentes de todos os usuários. Cada postagem deve exibir o nome do autor, conteúdo do post, e a data/hora da postagem. O feed deve ser atualizado em tempo real usando Websockets quando novos posts forem adicionados.


#### 3. Criação e Reação em Postagens:

> Permitir que o usuário autenticado crie novas postagens com um campo de texto. As postagens devem aparecer automaticamente no feed sem necessidade de recarregar a página.

> Permitir que os usuários comentem nas postagens. Os comentários também devem ser atualizados em tempo real.

### 🔥 POWER UP

**Você se destarará se implementar um Backend com Node.js (Express / Nest.js / Bun) integrado ao front-end com o Websocket e registro em Banco de Dados / CDN 100% funcional.**

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






## Desafio Técnico – Desenvolvedor(a) Back-End  
**Plataforma Zion Global – Comunidade Cristã**

### Objetivo do Desafio

Você irá desenvolver uma **API back-end** para uma plataforma global de comunidade cristã, focada em conectar membros da Igreja Zion. O projeto deve ser entregue em até **7 dias** e será avaliado em code-review, considerando critérios técnicos, arquitetura, documentação e clareza de código.

### Instruções Gerais

- O projeto deve ser desenvolvido em **Node.js** (preferencialmente com TypeScript).
- Utilize **PostgreSQL** como banco de dados relacional.
- Implemente **Websockets** para comunicação em tempo real (ex: chat ou notificações).
- Siga princípios de **Clean Code**, **DDD** e **Clean Architecture**.
- Provisione e documente o deploy em **AWS** (pode ser via scripts, Docker, ou instruções detalhadas).
- Entregue a documentação da API utilizando **Swagger**.
- O contrato da API deve ser pensado para integração com o front-end, baseado na tela ilustrativa fornecida.
- O repositório deve conter instruções claras de setup, execução e deploy.

### User Story

> **Como** membro da comunidade Zion,  
> **quero** poder criar uma conta, acessar um feed de postagens, interagir (curtir/comentar), enviar mensagens em tempo real para outros membros,  
> **para que** eu possa me conectar, compartilhar experiências e fortalecer minha fé junto à comunidade.

### Requisitos Técnicos

#### Mínimo Esperado

- **Endpoints RESTful** para:
  - Cadastro e autenticação de usuário
  - CRUD de postagens (feed)
  - Curtidas e comentários em postagens
  - Listagem de membros
- **Websocket** para:
  - Chat privado entre membros
  - Notificações em tempo real (ex: nova mensagem, novo comentário)
- **Banco de Dados**:
  - Modelagem relacional (Postgres) com migrations
- **Documentação Swagger** cobrindo todos os endpoints
- **Boas práticas** de Clean Code, DDD e Clean Architecture
- **Provisionamento AWS**: instruções para deploy (EC2, RDS, ou Docker + ECS)
- **README** detalhado com setup, execução, deploy e exemplos de uso da API

#### Bônus (Pontos Extras)

- Testes automatizados (unitários e/ou integração)
- Integração com serviços AWS (ex: S3 para upload de imagens de perfil/post)
- Autenticação JWT e refresh token
- Rate limiting e segurança básica (CORS, Helmet, etc)
- CI/CD configurado (GitHub Actions, GitLab CI, etc)
- Scripts de seed para dados de exemplo
- Versionamento de API

### Tela Ilustrativa (Base para Contrato de API)

Abaixo, uma sugestão de tela para o feed principal da comunidade, que servirá de referência para o contrato de endpoints:

| **Feed da Comunidade Zion** |
|----------------------------|
| [Foto do usuário] Nome do usuário - Data/Hora |
| Texto da postagem |
| [Imagem opcional] |
| [Curtir] [Comentar] [Compartilhar] |
| Comentários recentes... |
| [Campo para novo comentário] |
| [Botão: Nova Postagem] |
| [Menu lateral: Lista de membros online] |
| [Botão: Chat] |

**Funcionalidades esperadas a partir da tela:**
- Listar postagens (com paginação)
- Criar nova postagem (texto e imagem)
- Curtir/comentar postagens
- Listar comentários
- Listar membros online
- Iniciar chat privado via websocket

### Entrega

- Repositório público (GitHub, GitLab, etc) com todo o código, documentação e instruções.
- Link para acesso à documentação Swagger.
- Scripts ou instruções para deploy na AWS.
- O projeto deve ser funcional e possível de rodar localmente via Docker ou instruções claras.

### Avaliação

Serão avaliados:
- Organização do código e arquitetura
- Clareza e cobertura da documentação
- Qualidade dos endpoints e uso de websockets
- Modelagem do banco de dados
- Aderência ao Clean Code, DDD e Clean Architecture
- Facilidade de deploy e setup
- Implementação dos bônus

**Boa sorte!**  
Qualquer dúvida, envie perguntas durante o período do desafio.

[1] https://coodesh.com/blog/rh-tech/assessment/confira-testes-de-node-js-on-line-e-avalie-habilidades-de-desenvolvedores/
[2] https://www.testgorilla.com/pt/biblioteca-de-teste/funcao/desenvolvedor-a-node-js/
[3] https://www.youtube.com/watch?v=rVwVMkHiBUM
[4] https://www.dio.me/articles/teste-tecnico-dev-backend
[5] https://coodesh.com/blog/rh-tech/assessment/como-avaliar-back-end-veja-dicas-de-testes-tecnicos/
[6] https://www.atlassian.com/br/agile/project-management/user-stories
[7] https://www.thiengo.com.br/android-about-page-api-para-construir-a-tela-sobre
[8] https://www.youtube.com/watch?v=Ru6Tr7Q75IQ
[9] https://blog.myscrumhalf.com/user-stories-o-que-sao-como-usar/
[10] https://www.youtube.com/watch?v=WL5R4vAHuKk
[11] https://github.com/RogaLabs/teste-backend-nodejs
[12] https://metodoagil.com/historias-de-usuario/
[13] https://www.ibm.com/br-pt/products/api-connect/socialize
[14] https://www.testgorilla.com/pt/biblioteca-de-teste/funcao/desenvolvedor-a-back-end/
[15] https://awari.com.br/user-story/
[16] https://www.locaweb.com.br/blog/temas/codigo-aberto/12-apis-que-todo-desenvolvedor-precisa-conhecer/
[17] https://www.devmedia.com.br/personas-e-user-story-mapping-identificando-o-seu-verdadeiro-publico-alvo/31699
[18] https://developers.huggy.io/pt/API/api-v3.html
[19] https://www.youtube.com/watch?v=U4FoR0UsLRA
[20] https://developer.chrome.com/docs/capabilities/web-apis/wake-lock
[21] https://play.google.com/store/apps/details?id=br.painelstream2.comunidadecristlivre
[22] https://play.google.com/store/apps/details?id=com.inpeaceapp.comunidadecristaide.pr
[23] https://www.instagram.com/churchsomosum/
[24] https://www.youtube.com/watch?v=yIqsTrnldhU
[25] https://br.freepik.com/fotos-vetores-gratis/comunidade-crista/3
[26] https://pplware.sapo.pt/informacao/tutorial-como-desenvolver-uma-api-com-node-js-e-swagger/
[27] https://kinsta.com/pt/base-de-conhecimento/endpoint-api/
[28] https://www.youtube.com/watch?v=3Arz8E2kaws
[29] https://apidog.com/pt/blog/use-swagger-create-node-js-api-pt/
[30] https://awari.com.br/endpoints-api/
[31] https://portalamoregraca.com.br
[32] https://gist.github.com/roger-dev-br/ec36a02bbd25eec4764b43b70e9591ea
[33] https://www.ibm.com/br-pt/think/topics/api-endpoint
[34] https://www.canva.com/pt_br/cartazes/modelos/igreja/
[35] https://docs.nestjs.com/recipes/swagger
[36] https://www.cloudflare.com/pt-br/learning/security/api/what-is-api-endpoint/
[37] https://guiame.com.br/gospel/missoes-acao-social/cristaos-na-siria-continuam-protestando-contra-perseguicao-nao-estamos-mais-seguros.html
[38] https://cursa.app/pt/pagina/documentando-api-s-nodejs-com-swagger
[39] https://mailchimp.com/pt-br/resources/what-is-an-api-endpoint/
[40] https://dev.to/przpiw/document-express-api-with-swagger-51in
