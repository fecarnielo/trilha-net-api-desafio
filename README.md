# DIO - Trilha .NET - API e Entity Framework
www.dio.me

## Desafio de projeto
Desafio de projeto proposto pela Pottencial juntamente com a DIO, ministrado pelo @Leonardo Buta.

## Contexto
Construção de um gerenciador de tarefas, onde é possível cadastrar uma lista de tarefas que permite organizar melhor a rotina.

Essa lista de tarefas trabalha com o CRUD, ou seja, permite obter os registros, criar, salvar e deletar esses registros.

A sua aplicação é do tipo Web API.

A classe principal (tarefa) é a seguinte:

![Diagrama da classe Tarefa](diagrama.png)


## Métodos esperados
Os métodos criados são os seguintes:


**Swagger**


![Métodos Swagger](swagger.png)


**Endpoints**


| Verbo  | Endpoint                | Parâmetro | Body          |
|--------|-------------------------|-----------|---------------|
| GET    | /Tarefa/{id}            | id        | N/A           |
| PUT    | /Tarefa/{id}            | id        | Schema Tarefa |
| DELETE | /Tarefa/{id}            | id        | N/A           |
| GET    | /Tarefa/ObterTodos      | N/A       | N/A           |
| GET    | /Tarefa/ObterPorTitulo  | titulo    | N/A           |
| GET    | /Tarefa/ObterPorData    | data      | N/A           |
| GET    | /Tarefa/ObterPorStatus  | status    | N/A           |
| POST   | /Tarefa                 | N/A       | Schema Tarefa |


```json
{
  "id": 0,
  "titulo": "string",
  "descricao": "string",
  "data": "2022-06-08T01:31:07.056Z",
  "status": "Pendente"
}
```
