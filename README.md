![Blox](logo_blox.png)

# Sobre a Empresa

  Blox é uma EdTech que propõe uma abordagem radicalmente nova no ensino superior.
Acreditamos que cada aluno é único e que portanto, sua trilha formativa também
deveria ser única, personalizada às suas necessidades. Desenvolvemos todas as
ferramentas e processos necessários para apoiar as universidades na verdadeira
transformação da educação.

[Website](https://blox.education)

[Youtube](https://www.youtube.com/channel/UCoU3Z5EheoYz3YQFRAaaeTw)

# Sobre o teste

  Este teste é apresentado às pessoas que estão se candidatando às vagas de
desenvolvimento para avaliar os quesitos técnicos. O código deve ser escrito
utilizando Javascript + ReactJS.

## O Desafio

Seu objetivo é implementar o front-end de duas telas.
- Tela de Cadastro
- Tela de Listagem de Unidades Curriculares

A Tela de cadastro deverá conter os seguintes campos: 
<img width="593" alt="Captura de Tela 2022-08-24 às 11 57 55" src="https://user-images.githubusercontent.com/34753722/186452005-808610ed-3bc2-4adc-9499-6ec2b9fc0630.png">


A Tela de Listagem de listagem de Unidades Curriculares a partir da resposta JSON de uma API.

![Tela listagem de unidades curriculares](tela_listagem_unidades_curriculares.png)

Os endpoints a serem usados nesse desafio são:

### Curricular Units

`curl --request GET \
  --url 'https://app-api.blox.education/v1/public/institutions/22/blox_offerings?page=1&per=5' \
  --header 'Accept: application/json, text/plain, */*' \`

Retorna a listagem de unidades curriculares a serem implementadas como listagem. 

### Mapeamento dos campos

![Sugestão de tela](fields.png)

### Requisitos

  - Deve ser possível paginar as unidades curriculares
  - Deve ser possível listar as unidades curriculares de acordo com sua situação. `blox#status`

### O que esperamos

 - Utilização de versionamento de código (git)
 - Criar uma documentação de como rodar sua aplicação - README
 - Criar uma breve descrição da solução utilizada

### Avaliação / Critérios Obrigatórios

  - Compreensão dos requisitos
  - Aplicação de conceitos de clean code, DRY, SOLID, KISS, YAGNI, etc.
  - Compreensão do ecossistema React, React Hooks e seus fundamentos
  - Estruturação dos componentes
  - Estruturação do CSS
  - Utilização de [Context API](https://reactjs.org/docs/context.html)

### Plus / Diferencial

  - Desafio extra para os que querem ir além. Não é obrigatório o mini-desafio abaixo para sua entrega ser avaliada.

  - Feature extra: Modal de detalhes

  ![Modal](desafio-front-modal.jpg)

  - Styled Components
  - Teste dos componentes (JEST)
  - Web hooks

### Entrega do desafio

  - O código deve ser disponibilizado no github ou bitbucket para avaliação.
  - A aplicação deve ser disponibilizada remotamente.
    Ex: [Heroku Deploy](https://blog.heroku.com/deploying-react-with-zero-configuration)
