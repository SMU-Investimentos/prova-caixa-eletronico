# Cadastro de Investidores

# Introdução:
Este teste tem como objetivo a criação de uma API de cadastro de investidores com conta. Os investidores pode fazer operações como saque e depósito e pra isso, o mesmo precisa de uma conta para contabilizar os saques, depósitos e transferências.


# Cadastro
Antes das operações, o investidor precisa fazer um cadastro, pode ser ele, tanto pessoa física como jurídica. É muito importante ter validações para os cadastros.
No momento do cadastro, o investidor também precisa receber uma conta para fazer as operações.
Em caso de anormalidade com os investidores, deve ser possível bloquear ou desbloquear os mesmos, via endpoint administrativo com segurança oauth.


# Conta
A conta terá as seguintes operações: Saque, Depósito, Transferência e extrato.
É importante ter as validações principais para que o investidor sempre transfira valores que são dele e para que a conta não fique negativa.
O investidor não pode transferir para ele mesmo.
O investidor precisa realizar autenticação via Oauth para fazer alguma operação e comprovar que é ele mesmo que está fazendo a operação.


# Observações:

 - Toda a construção deve ser em Java e de preferência a mais recente.
 - A API de autenticação e do investidor ser construídas em módulos diferentes.
 - Fazer testes unitários
 - Usar o H2 para subir a base de dados em memória.
 - Os projetos devem ser desenvolvidos com a stack do Spring(Boot, Data, Etc...).
 - O prazo de entrega da prova é de 5 dias corridos.
 -	Usar o H2 para subir a base de dados em memória.
 - Subir o fonte num github + jar pronto para ser executado
 
