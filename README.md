<p align="center">
  <a href="http://nestjs.com/" target="blank"><img src="https://nestjs.com/img/logo-small.svg" width="200" alt="Nest Logo" /></a>
</p>

# Ejecutar en desarrollo

1. Clonar el repositorio
2. Ejecutar `yarn install`
3. Tener Nest CLI instalado `npm i -g @nestjs/cli`
4. Levantar la base de datos con `docker-compose up -d`
5. Clonar el archivo **.env.template** y renombrarlo a **.env**
6. Completar las variables de entorno en el archivo **.env**
7. Ejecutar `yarn start:dev`
8. Reconstruir la base de datos con la semilla `localhost:3000/api/v2/seed`

## Stack utilizado

- MongoDB
- NestJS
- Docker

## Production build

1. Crear el archivo **.env.prod** con las variables de entorno necesarias
2. Crear la nueva imagen `docker-compose -f docker-compose.prod.yml --env-file .env.prod up --build
`
