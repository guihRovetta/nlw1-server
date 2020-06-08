<h2 align="center">
Ecoleta - back-end
<br/>

</h2>

<blockquote align="center">
  Projeto realizado durante a Next Level Week #01 da Rocketseat
</blockquote>

<hr/>

## 📓 Sobre:

Eu desenvolvi esse projeto durante a Next Level Week #01 da Rocketseat, com o intuito de aprofundar meus conhecimentos em back-end utilizando o NodeJS.

## 🎓 Aplicação de conhecimentos:

- Utilização do TypeScript
- Criação de api seguindo as melhores práticas
- Aprendizado sobre SQLite3
- Uso do Knex.js para manipulação do banco de dados
- Validação de campos das rotas com Celebrate
- Tratamento de uploads de imagens através do Multer

## 🚀 Tecnologias:

- NodeJS
- TypeScript

## 🖥️ Como executar:

Clone o repositório com:

```bash
$ git clone https://github.com/guihRovetta/nlw1-server.git
```

Para baixar as dependências, utilize o comando na raiz do projeto:

```bash
npm i
```

Logo depois execute os seguintes comandos:

```bash
npm run knex:seed
npm run knex:migrate
```

E para rodar o projeto, execute:

```bash
npm run dev
```

## 🗺️ Rotas:

### Items

| Rota     | Método | Parâmetros     | Descrição                      |
| :------- | :----- | :------------- | :----------------------------- |
| `/items` | GET    | Sem Parâmetros | Lista todos os itens de coleta |

### Points

| Rota          | Método | Parâmetros                                                                                                 | Descrição                                 |
| :------------ | :----- | :--------------------------------------------------------------------------------------------------------- | :---------------------------------------- |
| `/points`     | GET    | `city` , `uf` , `items` in query                                                                           | Listar pontos através dos filtros         |
| `/points/:id` | GET    | point id                                                                                                   | Listar um ponto por id                    |
| `/points`     | POST   | `name` , `email` , `whatsapp`, `latitude` , `longitude` , `city` , `uf` , `image` in multipart form / body | Criar um ponto com os parâmetros passados |
| `/point/:id`  | PUT    | `name` , `email` , `whatsapp`, `latitude` , `longitude` , `city` , `uf` in body and point id               | Editar um ponto por id                    |
| `/point/:id`  | DELETE | point id                                                                                                   | Excluir um ponto por id                   |

---

<h3 align="center">
Autor: <a alt="Guilherme de Almeida Rovetta" href="https://github.com/guihRovetta">Guilherme de Almeida Rovetta</a>
</h3>

<p align="center">

  <a alt="Guilherme de Almeida Rovetta Linkedin" href="https://www.linkedin.com/in/guilherme-rovetta-381a89b0">
  <img src="https://img.shields.io/badge/LinkedIn-Guilherme%20Rovetta-blue?logo=linkedin"/></a>
  <a alt="Guilherme de Almeida Rovetta GitHub" href="https://github.com/guihRovetta">
  <img src="https://img.shields.io/badge/GitHub-guihRovetta-lightgrey?logo=github"/></a>

</p>
