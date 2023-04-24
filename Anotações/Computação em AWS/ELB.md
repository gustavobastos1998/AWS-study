## Elastic Load Balance

 - Balanceamento de carga de aplicação, gateway e rede.

 - Escopo regional.

 - Escala de forma automática, sem custos.

 - Junto ao EC2 AutoScaling permite ciar aplicações altamente disponíveis.

 - É um algorítmo, que pode ficar entre o cliente e as instâncias EC2 (server), quue determina os destinos das requisições feitas pelo cliente, ou seja, para qual instância irá a requisição. Por ele ter comunicação com o EC2 AutoScaling, a aplicação estará disponível pela maior parte do tempo possível já que caso uma instância seja parada ou tenha algum problema, o ELB mudará o curso da requisição.