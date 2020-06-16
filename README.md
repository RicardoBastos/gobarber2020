<h1 align="center">
	<img alt="GoStack" src="logo.svg" width="200px" />
</h1>
<h1 align="center">
	<img alt="Mockup" src="https://res.cloudinary.com/dpicpf4yh/image/upload/v1592254901/gobarber_ag8weh.png">
</h1>

## GoBarber 2020 - Curso Rocketseat

GoBarber é uma aplicação que ajuda controlar agendamentos de clientes a ida até a barbearia. Com ele o cliente efetua um agendamento e o barbeiro consegue controlar o fluxo de seus clientes pela web ou pelo celular.

---

## Requisitos

Tenha o yarn ou npm instalado

```bash
 $ git clone https://github.com/ricardobastos/gobarber2020.git && cd gobarber2020
```

### API

#### Tecnologias Usadas

[Node.js](https://nodejs.org/en/), [TypeScript](https://www.typescriptlang.org/), [Express](https://expressjs.com/pt-br/), [Multer](https://github.com/expressjs/multer), [TypeORM](https://typeorm.io/#/), [JWT-token](https://jwt.io/), [uuid v4](https://github.com/thenativeweb/uuidv4/), [PostgreSQL](https://www.postgresql.org/), [Date-fns](https://date-fns.org/), [Jest](https://jestjs.io/), [SuperTest](https://github.com/visionmedia/supertest), [Husky](https://github.com/typicode/husky), [Commitlint](https://github.com/conventional-changelog/commitlint), [Commitizen](https://github.com/commitizen/cz-cli), [Eslint](https://eslint.org/), [Prettier](https://prettier.io/), [EditorConfig](https://editorconfig.org/)

**Para rodar a API siga os passos abaixo**

```bash
# Instalando as dependências
$ yarn

# Faça uma cópia de '.env.example' para '.env'
$ cp .env.example .env
# coloque os valores correspondentes

# Criando uma imagem do postgreSQL usando docker
$ docker run --name gobarber-postgres -e POSTGRES_USER=docker \
              -e POSTGRES_DB=gobarber -e POSTGRES_PASSWORD=docker \
              -p 5432:5432 -d postgres

# Criando uma imagem mongoDB usando docker
$ docker run --name gobarber-mongodb -p 27017:27017 -d -t mongo

# Criando uma imagem do redis using docker
$ docker run --name gobarber-redis -p 6379:6379 -d -t redis:alpine

# Faça uma cópia do 'ormconfig.example.json' to 'ormconfig.json'
$ cp ormconfig.example.json ormconfig.json
# coloque os valores correspondentes


# Rode as migrations para criar as tabelas no banco de dados
$ yarn typeorm migration:run

# Rode o serviço de API
$ yarn dev:server

# Projeto está sendo executado!
```

---

### FRONTEND

#### Tecnologias Usadas

[ReactJS](https://reactjs.org/), [TypeScript](https://www.typescriptlang.org/), [React Router DOM](https://reacttraining.com/react-router/), [React Icons](https://react-icons.netlify.com/#/), [UnForm](https://unform.dev/), [Yup](https://github.com/jquense/yup), [Styled Components](https://styled-components.com/), [Polished](https://github.com/styled-components/polished), [Axios](https://github.com/axios/axios), [Husky](https://github.com/typicode/husky), [Commitlint](https://github.com/conventional-changelog/commitlint), [Commitizen](https://github.com/commitizen/cz-cli), [Eslint](https://eslint.org/), [Prettier](https://prettier.io/), [EditorConfig](https://editorconfig.org/)

**Para rodar o Frontend**

```bash
# Instalar as dependências
$ yarn

# Start o projeto
$ yarn start

# Necessário a API estar rodando
```

---

### MOBILE

#### Tecnologias Usadas

[ReactJS](https://reactjs.org/), [TypeScript](https://www.typescriptlang.org/)
, [React Native](https://reactnative.dev/), [React Navigation](https://reactnavigation.org/)
, [React Native Vector Icons](https://github.com/oblador/react-native-vector-icons), [UnForm](https://unform.dev/)
, [Yup](https://github.com/jquense/yup), [Styled Components](https://styled-components.com/)
, [Axios](https://github.com/axios/axios), [Husky](https://github.com/typicode/husky)
, [Commitlint](https://github.com/conventional-changelog/commitlint), [Commitizen](https://github.com/commitizen/cz-cli), [Eslint](https://eslint.org/), [Prettier](https://prettier.io/), [EditorConfig](https://editorconfig.org/)

**Para rodar o Mobile**

```bash
# Instalar as dependências
$ yarn

# Certifique que 'src/services/api.ts' tenha seu IP

# Para rodar android
$ yarn android

# Para rodar ios
$ yarn ios

# Necessário a API estar rodando
```

---

Desenvolvido por Ricardo Bastos 🙏 [Linkedin](https://www.linkedin.com/in/ricardo3bastos/)
