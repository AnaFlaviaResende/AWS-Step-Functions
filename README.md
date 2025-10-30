# AWS-Step-Functions

Este repositório faz parte do desafio proposto pela DIO, com o objetivo de consolidar os conhecimentos sobre orquestração de workflows automatizados usando o serviço AWS Step Functions

# O que é o AWS Step Functions

O AWS Step Functions é um serviço gerenciado da Amazon Web Services (AWS) que permite criar, visualizar e automatizar fluxos de trabalho (workflows) compostos por várias etapas — chamadas de estados.

Esses estados podem executar funções Lambda, chamar APIs, acessar bancos de dados, enviar mensagens via SQS ou SNS, entre muitas outras integrações, tudo sem precisar escrever código de forma manual.

# Como funciona

Você define uma State Machine (máquina de estados) usando JSON ou YAML, onde descreve:

A ordem das tarefas;

As condições de decisão (if/else ou choice states);

O tratamento de erros e repetições;

E como cada etapa se conecta à próxima.

O Step Functions executa esse fluxo de forma visual, controlada e rastreável, permitindo acompanhar cada execução em tempo real pelo console da AWS.

# Exemplo prático

Imagine um processo de cadastro de usuário:

Receber os dados pelo API Gateway

Validar com uma função Lambda

Salvar no DynamoDB

Enviar um e-mail de boas-vindas pelo SNS

O Step Functions conecta todas essas etapas em uma única sequência automatizada, garantindo que cada parte só execute quando a anterior for concluída com sucesso (ou redirecionando em caso de erro).

# Principais vantagens

Automação: orquestra múltiplos serviços AWS com pouco ou nenhum código.

Visibilidade total: cada execução pode ser monitorada graficamente.

Resiliência: tratamento automático de erros, tentativas e fluxos alternativos.

Integração nativa: conecta-se com Lambda, ECS, DynamoDB, SNS, SQS, SageMaker, entre outros.

Escalabilidade: gerencia fluxos simples ou altamente complexos, com milhões de execuções.
