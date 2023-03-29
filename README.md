# Travel Agency - API

Esta é uma fake API construida por mim para o projeto em grupo chamado "Travel Agency - Expedição Amazônia" de tema livre e com a participaçao dos seguintes colegas: Noelle Franco, Mariana Cardoso, Luana Morais e Germano Lop. 

## Endpoints

Seguem os endpoinst disponíveis na aplicação:

### URI

```https://expedicao-amazonia.herokuapp.com```

### Cadastro

```POST /register - Cadastro de usuários - FORMATO DA REQUISIÇÃO```<br/>

```json
{
	"email": "romana@email.com",
	"password": "Senh@123",
	"name": "Romana",
	"phone_number": "85985480622"
}
```
<br/>

```POST /register - Cadastro de usuários - FORMATO DA RESPOSTA```<br/>

```json
{
	"accessToken": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJlbWFpbCI6InJvbWFuYUBlbWFpbC5jb20iLCJpYXQiOjE2Nzc4OTIzODcsImV4cCI6MTY3Nzg5NTk4Nywic3ViIjoiMyJ9.ApXPdkmhKVikauaMyI4NyGepijT2H7rB8i3Ucr8vUQk",
	"user": {
		"email": "romana@email.com",
		"name": "Romana",
		"phone_number": "85985480622",
		"id": 3
	}
}
```

<br/>

```POST /favoritesActivities - Favoritar Atividade - FORMATO DA REQUISIÇÃO``` <br/>

```json
{
	"userId": 1,
	"activityId": 6
}
```

<br/>

```POST /favoritesActivities - Favoritar Atividade - FORMATO DA RESPOSTA``` <br/>

```json
{
	"userId": 1,
	"activityId": 6,
	"id": 2
}
```

<br/>

```POST /favoritesHotels - Favoritar Hotel - FORMATO DA REQUISIÇÃO``` <br/>

```json
{
	"userId": 1,
	"hotelId": 6
}
```

<br/>

```POST /favoritesHotels - Favoritar Hotel - FORMATO DA RESPOSTA``` <br/>

```json
{
	"userId": 1,
	"hotelId": 6,
	"id": 2
}
```

<br/>

```POST /reservedHotels - Reservar Hotel - FORMATO DA REQUISIÇÃO``` <br/>

```json
{
	"userId": 1,
	"hotelId": 2
}
```

<br/>

```POST /reservedHotels - Reservar Hotel - FORMATO DA RESPOSTA``` <br/>

```json
{
	"userId": 1,
	"hotelId": 2,
	"id": 1
}
```

<br/>

```POST /hotelsReviews - Adicionar nova review de Hotel - FORMATO DA REQUISIÇÃO``` <br/>

```json
{
	"userId": 1,
	"hotelId": 2,
	"comment": "Otimo hotel!",
	"rating": 5
}
```

<br/>

```POST /hotelsReviews - Adicionar nova review de Hotel - FORMATO DA RESPOSTA``` <br/>

```json
{
	"userId": 1,
	"hotelId": 2,
	"comment": "Otimo hotel!",
	"rating": 5,
	"id": 4
}
```

<br/>


Qualquer um desses 3 endpoints irá cadastrar o usuário na lista de "Users", sendo que os campos obrigatórios são os de email e password.
Você pode ficar a vontade para adicionar qualquer outra propriedade no corpo do cadastro dos usuários.


### Login

POST /login <br/>
POST /signin

Qualquer um desses 2 endpoints pode ser usado para realizar login com um dos usuários cadastrados na lista de "Users"
