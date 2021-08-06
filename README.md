# Entrada Caixa Eletrônico

Desenvolva um programa que simule a entrega de notas quando um cliente efetuar um saque em um caixa eletrônico. Os requisitos básicos são os seguintes:

 - Entregar o menor número de notas;

 - É possível sacar o valor solicitado com as notas disponíveis;

 - Saldo do cliente infinito;

 - Quantidade de notas infinito (pode-se colocar um valor finito de cédulas para aumentar a dificuldade do problema);
 - Notas disponíveis de R$ 100,00; R$ 50,00; R$ 20,00 e R$ 10,00

Exemplos:
Valor do Saque: R$ 30,00 – Resultado Esperado: Entregar 1 nota de R$20,00 e 1 nota de R$ 10,00.
Valor do Saque: R$ 80,00 – Resultado Esperado: Entregar 1 nota de R$50,00 1 nota de R$ 20,00 e 1 nota de R$ 10,00.

# Pedido de Abastecimento

Caso o caixa eletrônico esteja sem notas deverá ser emitido um pedido de saque para o banco responsável.

Exemplo:
Foi pedido um saque de R$ 200,00 e foram usadas as 2 ultimas notas de R$ 100,00, nesse momento deverá ser realizado um pedido
de abastecimento das notas de R$ 100,00 e assim por diante para as outras notas.

 - Os pedido de abastecimento devem ser totalmente seguro. (Utilizar Oauth2 ou JWT)
 - Cada caixa eletrônico pode realizar apenas 1 pedido de reabastecimento por vez.

No pedido de abastecimento deve se passar como paramentros os seguintes campos:
 - Valor
 - Quantidade de notas
 - Data e hora do pedido
 - Data e hora da entrega
 
Até que o abastecimento não seja finalizado o caixa eletrônico deve continuar funcionando sem problemas, ou seja 
caso seja feito um pedido de saque de R$ 100,00 e o caixa conter apenas notas de R$ 20,00 deverá ser entregue 5 notas ao cliente.


# Observações:

 - Todo pedido de saque e deve ser feito via REST.
 - O caixa eletrônico e o banco devem ser serviços/módulos diferentes.
 - No serviço/módulo do caixa eletrônico é obrigatório conter testes unitários(TDD).
 - Todos os dados devem ser guardados em um banco de dados (Postgres ou Mysql).
 - Os projetos devem ser desenvolvidos em java8 ou alguma versão superior + stack do Spring(Boot, Data, Etc...).
 - O prazo de entrega da prova é de 4 dias corridos.
 
