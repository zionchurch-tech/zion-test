# Desafio Back-End | Zion Church

### 📖 Objetivo do Desafio: 

Desenvolver uma aplicação web que utilize Inteligência Artificial para analisar, correlacionar e sugerir conexões entre textos bíblicos. O foco é avaliar habilidades avançadas de lógica de programação, manipulação de dados textuais, uso de IA e boas práticas de arquitetura back-end.

### Descrição do Projeto:

O DeepBible é uma plataforma onde você faz perguntas e recebe textos biblicos como resposta, você ainda pode conversar e aprofundar seu estudo com um versiculo biblico.

--------------


### 🗒️ User Story:
> Como estudante da Bíblia, quero pesquisar temas ou versículos e receber sugestões de passagens correlatas, com explicações,
> para aprofundar meu estudo e descobrir novas conexões entre os textos sagrados.


--------------


### 🔍 Detalhes do escopo do projeto:

#### 1. Consulta de Textos Bibicos (Bible):

Crie os endpoints necessários para buscar um texto biblico através do livro / capitulo / versiculo. Você deve armazenar no seu banco de dados os textos biblicos e organizar para que a busca por versiculos sejam eficientes, performáticos e responsivos.

> Você não pode usar APIs prontas da biblia, você deve importar alguma versão da biblia no seu banco de dados e organizar para suas APIs consultarem.


#### 2. Pesquisa e Correlação de Textos (Search):

Crie endpoints para pesquisar por tema, palavra-chave ou referência bíblica. Você deve retornar uma lista de versículos/passagens correlacionadas, com os assuntos referentes a esse texto.

> Você pode utilizar recursos de indexação do Postgres, queries do Prisma ou bibliotecas de IA (ex: embeddings, modelos de linguagem) para identificar conexões semânticas e contextuais.
> Exemplo: ao pesquisar “o que é o amor”, retornar versículos correlatos em diferentes textos biblicos, com explicação da relação e tags de assuntos.

> (🔥 Você ganhará um Bônus) Se desenvolver Algoritmo próprio de similaridade textual


#### 3. Conversa com texto biblico com I.A (Chat):

Crie endpoints para que o usuário possa "conversar" com o versiculo, você deve receber uma pergunta como "Porque devemos perdoar setenta vezes sete?" e um texto biblico como "Mateus 18:21-22". 
Seu endpoint deverá retornar um texto respondendo a pergunta do usuário, pode também listar passagens correlacionadas e sugestões de estudo.

> Utilizar IA (ex: modelo pré-treinado (open-ai / claude / Llama / deepseek), embeddings, ou integração com API de IA) para sugerir conexões não triviais entre textos e responder perguntas.


#### 4. (🔥 BONUS) Registro e Login:

Não é obrigatório, mas você se destarará se implementar endpoints necessários para o usuário se registrar e fazer login na plataforma. Pense em uma autenticação simples utilizando e-mail e senha. 

> Você pode usar uma lib para Auth e para gerenciar a sessão, como Supabase / Firebase / Cognito, etc.
**Você se destacará mais ainda se salvar um histórico de pesquisas daquele usuário na plataforma (ultimas buscas de textos-biblicos)**


--------------

### Requisitos técnicos:

1. Node.js (Express, Nest.js ou similar) ou Bun

2. Banco de dados relacional (Postgres)

3. Integração com modelo de IA (OpenAI, HuggingFace, ou modelo próprio)

4. API RESTful documentada com Swagger ou similar (pronta para um dev front-end usar)

5. Deploy no AWS ou Ambiente cloud similar (Railway / GCP / Azure / etc)

6. (🔥 BONUS) Se destacará se desenvolver os testes automatizados (unitários/integrados)


--------------

### Critérios de Avaliação:

1. Qualidade do Código
2. Modelagem do banco de dados
3. Boas práticas de Clean Code, DDD e Clean Architecture
4. Funcionalidade e eficiência da lógica de correlação
5. Documentação da API e facilidade de uso dos endpoints
6. README detalhado com setup, execução, deploy e exemplos de uso da API
7. Arquitetura Limpa e organizada (DDD / Clean Archtecture)
8. Preocupação com Escalabilidade e Performance
9. Deploy funcional (Docker, AWS)


--------------


### 🔥 Bônus (Ganhará Pontos Extras):

1. Desenvolvimento de Algoritmo próprio de similaridade textual
2. Endpoints de Registro e Login
3. Testes automatizados (unitários e/ou integração)
4. Rate limiting e segurança básica (CORS, Helmet, etc)
5. CI/CD configurado (GitHub Actions, GitLab CI, etc)
6. Scripts de seed para dados de exemplo
7. Versionamento de API


--------------


### Layout do Figma com Refinamento técnico:

Você conseguirá entender a aplicação, fluxo de telas e contratos de API através do Figma abaixo:

https://www.figma.com/design/BkomH2qiwzoXDw8lRtIf2Z/Teste---ZION-DEVELOPER?node-id=486-622&t=Lov4WrpFvqTsV9EN-1
