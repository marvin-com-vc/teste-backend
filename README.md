
# Olá!

Obrigado por se interessar em trabalhar conosco :D

Ficamos muito feliz em ver você por aqui!

## Teste Back-end: Autenticação

Faça uma aplicação Kotlin com Spring Webflux com dois endpoints:

1. /login: Recebe um Header HTTP Basic e autentica o usuário com retorno OK ou FORBIDDEN
2. /signup: Recebe um payload com usuário e senha e cadastra no banco.

O usuário é sempre um CPF. Valide antes de qualquer coisa!

Você pode usar um banco in-memory ou um mapa na sua aplicação. Este modelo já tem o driver para o H2, mas nada está configurado.

Importante: faça testes! Os que você achar necessário: unitários, integração, funcionais, e2e...

Testes são muito importantes para nós e iremos avaliar o que você está testando e como.

Não deixe mais de um usuário ser criado com o mesmo CPF. Retorne um erro na API caso isso ocorra.

### Exemplo de requisições

#### /login
`curl -X POST -u username:password http://localhost:8080/login`

#### /signup
```json
{
	"username": "80503465011",
	"password": "very_safe_password"
}
```

`curl -d '{"username":"80503465011", "password": "very_safe_password"}' -H "Content-Type: application/json" -X POST http://localhost:8080/signup`


## Sobre o código já existente
Este código foi criado com [Spring Initializr](https://start.spring.io/). 4 dependências foram escolhidas: H2 Database, Spring Data R2DBC, Spring Reactive Web e Spring Boot DevTools.

Caso prefira, pode usar outro template de projeto Spring Webflux que te deixe mais confortável, mas precisa utilizar Kotlin e Spring Webflux, ok?

## Entrega
Faça um fork deste repositório dentro do seu repositório pessoal no GitHub e envie o link para nós!

Quaisquer instruções a mais que precisemos saber, pode deixar no README.md do seu repositório.

Boa sorte! :D
