## Amazon EC2 Ato Scalling

 - Provê escalabilidade horizontal para ses serviços. Escalabilidade horizontal é a utilização de mais instâncias EC2 caso as que estão em execução não estejam dando conta de maneira boa as requisições requeridas.

 - Melhora a tolerância a falhas com identificação de instâncias indisponíveis e implantação multi-AZ. 


## Como funciona?

 - Como o nome sugere, é uma instância EC2 que escala automaticamente as necessidades de acordo com o que e preciso.

 - Imagine que em dias diferentes da semana sua aplicação apresenta diferentes necessidades de capacidade computacional. Com o EC2 AutoScalling, essas capacidades vão variar dependendo do dia da semana, já que a necessidade difere entre os dias.


## Como é a configuração?

 - Basicamente ao criar o auto scaling devemos dizer um número mínimo, desejado, necessário além das utilizadas e máxima de instâncias. 


## Scaling Preditivo

 - Precisa conhecer bem o serviço, ter em mãos dados fiéis à realidade para que possa gerenciar as instâncias de maneira correta. 


## Scaling Dinâmico

 - Uma métrica dirá a necessidade deste scaling. Digamos qe uma instância esteja utilizando 80% do seu processador, devido a essa métrica é preciso escalonar e utilizar outra instância.


## Observações

 - É possível combinar os dois tipos de Scallings.