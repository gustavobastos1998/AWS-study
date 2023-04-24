## O que são?

 - São serviços de mensageria.


## Simple Queue Service

 - É um sistema de mensageria onde serviços se comunicam mas de forma assíncrona.

 - Um exemplo do uso do SQS são os e-commerce. Quando uma conta é efetuada, o SQS enfileira as compras que vieram de um micro-serviço de compras e outros micro-serviço lê as informações da Queue.

 - Um usuário envia uma mensagem para a fila, outro lê, processa e a exclui da fila.


## Simple Notification Service

 - Sistema pub/sub (publisher/subscriber).

 - Utiliza tópicos como estrutura de dados.

 - Usuário publica mensagens no tópico e assinantes escutam.