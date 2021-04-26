# Teste Técnico Desenvolvedor Backend

O teste se baseia no desenvolvimento de um serviço que contenha uma API REST e um sistema de processamento assíncrono. Deverá conter as seguintes funcionalidades:

- O usuário deverá poder realizar um POST para pedido de crédito, informando alguns dados para validação. Essa chamada deve disparar uma rotina de validação assíncrona e retornar um ticket para consulta do resultado.
- O usuário deverá poder realizar um GET, informando o número do ticket que recebeu, para consultar o resultado da validação (Proposta aprovada ou rejeitada).

As regras de validação são as seguintes:
 - O tomador de crédito deve ser maior de 18 anos
 - O valor solicitado deve ser menor que R$ 100.000,00

 ### Observações

 1) Os payloads das chamadas ficam a cargo do desenvolvedor, mas devem conter os dados necessários para a validação
 2) A rota de consulta de resultado deve informar se a proposta foi aprovada ou rejeitada, com base nas regras de validação.
 3) É mandatório que a rotina de validação seja executada de forma ASSÍNCRONA.


## O que esperamos

Alguns pontos que esperamos encontrar na solução desse desafio

- Testes unitários
- Tratamento de erros
- Dockerfile funcional
- Logging das chamadas em nível suficiente para debugging (pode ser para o stdout)
- Migrações de bancos de dados, se necessário
