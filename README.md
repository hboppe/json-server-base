# Travel Agency - API

Esta é uma fake API construida por mim para o projeto em grupo chamado "Travel Agency - Expedição Amazônia" de tema livre e com a participaçao dos seguintes colegas: Noelle Franco, Mariana Cardoso, Luana Morais e Germano Lop. 

## Endpoints

Seguem os endpoinst disponíveis na aplicação:

### URI

```https://expedicao-amazonia.herokuapp.com```

### Cadastro de usuários

```POST /register - FORMATO DA REQUISIÇÃO ```<br/>

```
{
	"email": "romana@email.com",
	"password": "123456",
	"name": "Romana",
	"phone_number": "85985480622"
}
```
<br/>
```POST /signup``` <br/>
```POST /users```

Qualquer um desses 3 endpoints irá cadastrar o usuário na lista de "Users", sendo que os campos obrigatórios são os de email e password.
Você pode ficar a vontade para adicionar qualquer outra propriedade no corpo do cadastro dos usuários.


### Login

POST /login <br/>
POST /signin

Qualquer um desses 2 endpoints pode ser usado para realizar login com um dos usuários cadastrados na lista de "Users"
