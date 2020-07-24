# API para controle de notas ![Badge](https://img.shields.io/badge/Status-Conclu%C3%ADdo-green)

Aplicação para disponibilizar via API RestFull notas de alunos desenvolvido no bootcamp fullstack da IGTI

## <img src="https://img.icons8.com/ios-filled/20/000000/browser-window.png"/> Insomnia

<p align="center">
  <img src="https://github.com/cicerorod/igti-fullstack-mod3-react-controle-de-notas-backend-hooks/blob/master/img/tela.PNG">
</p>

<!--
## ![](https://img.icons8.com/ios-glyphs/20/000000/api.png)  API

`<link>` : <https://randomuser.me/api/?seed=javascript&results=100&nat=BR&noinfo> -->

## ![](https://img.icons8.com/metro/20/000000/run-command.png) Execução

1. Clonar via prompt de comando o projeto em uma pasta de sua preferência: `git clone https://github.com/cicerorod/igti-fullstack-mod3-react-controle-de-notas-backend-hooks.git`
2. Acessar a pasta principal do projeto via prompt de comando. Ex: `cd igti-fullstack-mod3-react-controle-de-notas-backend-hooks`;
3. Executar o comando `yarn` para baixar as dependências. Ex: `yarn`;
4. Executar o comando `yarn start`. Ex: `yarn start`
5. Acessar o endereço `http://localhost:3001/` conforme rotas definidas no item rotas

### ![](https://img.icons8.com/metro/20/000000/run-command.png) Rotas

#### `/grade/`

HTTP GET solicitação que retorna uma resposta JSON contendo as notas.

##### `GET`: `http://localhost:3001/grade/`

##### Exemplo de retorno:

```json
{
  "grades": [
    {
      "id": 1,
      "student": "John Petrucci",
      "subject": "01 - JavaScript",
      "type": "Exercícios",
      "value": 4,
      "timestamp": "2020-07-23T23:08:13.477Z"
    },
    {
      "id": 2,
      "student": "Cícero Rodrigues",
      "subject": "01 - JavaScript",
      "type": "Exercícios",
      "value": 5,
      "timestamp": "2020-07-23T23:26:02.027Z"
    },
    {
      "id": 3,
      "student": "João da Silva",
      "subject": "2 - Node",
      "type": "Exercícios",
      "value": 4,
      "timestamp": "2020-07-23T23:27:11.660Z"
    }
  ]
}
```

#### `/grade/id`

HTTP GET solicitação que retorna uma resposta JSON contendo as informações do `id` pesquisado.

##### `GET`: `http://localhost:3001/grade/id`

##### Exemplo: `http://localhost:3001/grade/2`

##### Exemplo de retorno:

```json
{
  "id": 2,
  "student": "Cícero Rodrigues",
  "subject": "01 - JavaScript",
  "type": "Exercícios",
  "value": 5,
  "timestamp": "2020-07-23T23:26:02.027Z"
}
```

#### `/grade/id`

HTTP DEL, solicitação para excluir um registro referente ao `id`.

##### `DEL`: `http://localhost:3001/grade/id`

##### Exemplo: `http://localhost:3001/grade/4`

##### Exemplo de retorno:

```Request
true
```

#### `/grade/`

HTTP POST para inserção de registros. O formato da solicitação é JSON.

##### `Post`: `http://localhost:3001/grade/`

##### Exemplo de parâmetro:

```json
{
  "student": "Maria Barbosa",
  "subject": "3 - React",
  "type": "Exercícios",
  "value": 10
}
```

##### Exemplo de retorno:

```Json
{
  "id": 4
}

```

### ![](https://img.icons8.com/wired/20/000000/react.png) Frontend

Para utilização da API, foi desenvolvido uma camada de apresentação que pode ser baixada [aqui][frontend]


<!-- :hammer:-->

## ![](https://img.icons8.com/ios-filled/20/000000/hammer.png) Recursos utilizados:

- **[NodeJS](https://nodejs.org/en/)**
- **[Json](https://www.w3schools.com/js/js_json_intro.asp)**
- **[Express](http://expressjs.com/)**
- **[Insomnia](https://insomnia.rest/download/)**
- **[Visual Studio Code](https://code.visualstudio.com/?WT.mc_id=hackingcarreira_wmc-github-gllemos)**

## ![](https://img.icons8.com/ios-glyphs/20/000000/pull-request.png) Contribuições

1. Faça o _fork_ do projeto (<https://github.com/cicerorod/igti-fullstack-mod3-react-controle-de-notas-backend-hooks/fork>)
2. Crie uma _branch_ para sua modificação (`git checkout -b feature/[nome]`)
3. Faça o _commit_ (`git commit -am 'Add files [nome]'`)
4. _Push_ (`git push origin feature/[nome]`)
5. Crie um novo _Pull Request_

## ![](https://img.icons8.com/windows/20/000000/regular-document.png) Licença

Este projeto está sob a licença do MIT. Consulte [LICENSE](https://github.com/cicerorod/igti-fullstack-mod3-react-controle-de-notas-backend-hooks/blob/master/LICENSE) para obter mais informações.

## ![](https://img.icons8.com/ios-glyphs/22/000000/code-file.png) Desenvolvedor

<img src="https://avatars.githubusercontent.com/cicerorod" width=115>

[![](https://img.icons8.com/fluent/30/000000/github.png)](https://github.com/cicerorod)
[![](https://img.icons8.com/metro/25/000000/linkedin.png)](https://www.linkedin.com/in/c%C3%ADcero-rodrigues-89623784/)
[![](https://img.icons8.com/metro/25/000000/facebook.png)](https://www.facebook.com/cicero.rodrigues.90834)
[![](https://img.icons8.com/material-rounded/29/000000/instagram-new.png)](https://www.instagram.com/cicero_rod/)
[![](https://img.icons8.com/metro/26/000000/email.png)](mailto:cicerorod@gmail.com)

<p align="center">
  <img src="https://img.icons8.com/wired/32/000000/icons8-new-logo.png" >
  </br>
  <a href="https://icons8.com/icon/">Icons by Icons8</a>
  
</p>


[frontend]: https://github.com/cicerorod/igti-fullstack-mod3-react-controle-de-notas-frontend-hooks
