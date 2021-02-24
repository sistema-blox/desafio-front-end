![Blox](logo_blox.png)

# Sobre a Empresa

Blox é uma EdTech que propõe uma abordagem radicalmente nova no ensino superior. Acreditamos que cada aluno é único e que portanto, sua trilha formativa também deveria ser única, personalizada às suas necessidades. Desenvolvemos todas as ferramentas e processos necessários para apoiar as universidades na verdadeira transformação da educação.

WebSite: https://blox.education

Youtube: https://www.youtube.com/channel/UCoU3Z5EheoYz3YQFRAaaeTw

# Sobre o teste

Este teste é apresentado às pessoas que estão se candidatando às vagas de desenvolvimento para avaliar os quesitos técnicos. 
O código deve ser escrito utilizando Javascript + ReactJS.

## O Desafio

Seu objetivo é implementar uma tela de listagem de unidades curriculares.
![Tela listagem de unidades curriculares](tela_listagem_unidades_curriculares.png)

Para isso você deve consumir a api disponível em:
https://api-dev.plataformablox.com.br/api-docs/index.html

os endpoints a serem usados nesse desafio são:

### Token - api/token

POST em api/token, com os params:
{
  "username": "EXAMPLE",
  "password": "EXAMPLE",
  "institution_id": EXAMPLE
}

retorna o token a ser utilizado nos endpoints onde há necessidade de autenticação:

comando curl:
`curl -X POST "https://api-dev.plataformablox.com.br/api/token" -H "accept: */*" -H "Content-Type: application/json" -d "{\"username\":\"EXAMPLE\",\"password\":\"EXAMPLE\",\"institution_id\":EXAMPLE}"`

ver aquivo: `token_response_example.json` nesse repositório

### Curricular Units - api/bloxes

GET em api/bloxes, com os params per e page (query string)

retorna a listagem de unidades curriculares a serem implmentadas.

comand curl:
`curl -X GET "https://api-dev.plataformablox.com.br/api/bloxes?per=1&page=1" -H "accept: */*" -H "Authorization: TOKEN_RETORNADO_NO_ENDPOINT_ANTERIOR"`

ver aquivo: `curricular_units_response_example.json` nesse repositório

### Mapeamento dos campos

![Sugestão de tela](fields.png)

### Requisitos: 

- Deve ser possível paginar as unidades curriculares
- Deve ser possível listar as unidades curriculares de acordo com sua situação. `blox#status`

### O que esperamos:

 - Utilização de versionamento de código (git);
 - Criar uma documentação de como rodar sua aplicação - README
 - Criar uma breve descrição da solução utilizada;

### Plus

 - Desenvolver utilizando o padrão api context https://rapidapi.com/blog/react-context-api/?utm_source=google&utm_medium=cpc&utm_campaign=DSA&gclid=Cj0KCQiAj9iBBhCJARIsAE9qRtACLBdDOqNysczgOTFa6P4dSSpPHovWBFGzjrckH6clet_hAM2uO9EaAujREALw_wcB
 - Teste dos componentes
 - Web hooks

### Entrega do desafio:

- O código deve ser disponibilizado no github ou bitbucket para avaliação.
- A aplicação deve ser disponibilizada remotamente. ex: https://blog.heroku.com/deploying-react-with-zero-configuration
