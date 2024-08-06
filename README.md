# API Cadastro de Cliente consumindo API do ViaCep

![Java](https://img.shields.io/badge/java-%23ED8B00.svg?style=for-the-badge&logo=openjdk&logoColor=white)
![Spring](https://img.shields.io/badge/spring-%236DB33F.svg?style=for-the-badge&logo=spring&logoColor=white)

Esse projeto é uma API construída usando Java e Java Spring, Consumindo a API do viaCEP

## Problema
A API foi desenvolvida para fazer um cadastro simples de um Cliente que precisa apenas ser inserido seu endenreço cujo qual será consultado através da API externa ViaCep.

## Solução
A API espera receber do usuário as informações: Nome e CEP.
Através destas informações é feita uma requisição à API do ViaCep para receber e persistir as informações tais como: Endereço, Rua, Cidade, Estado etc.

## API Endpoints
```json
GET /clientes/{id}
PUT /clientes/{id}
DELETE /clientes/{id}
GET /clientes
POST /clientes
```
BODY do POST:
```markdown
{
  "nome": "string",
  "endereco": {
    "cep": "string"
  }
}
```
## 

Resposta aguardada no POST:
```json
{
  "id": 0,
  "nome": "string",
  "endereco": {
    "cep": "string",
    "logradouro": "string",
    "complemento": "string",
    "unidade": "string",
    "bairro": "string",
    "localidade": "string",
    "uf": "string",
    "ibge": "string",
    "gia": "string",
    "ddd": "string",
    "siafi": "string"
  }
}
```


## Objetivo
este é um projeto desenvolvido a fim de aprimorar meu portfólio e mostrar meus conhecimentos.

## Qualquer sugestão, crítica ou oportunidade de trabalharmos juntos, contate : 
## paulorubensbarbosa@outlook.com
