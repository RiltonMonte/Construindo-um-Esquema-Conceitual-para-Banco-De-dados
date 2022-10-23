# Construindo-um-Esquema-Conceitual-para-Banco-De-dados

Projeto de Banco de dados da D.I.O

## Objetivo:

Cria o esquema conceitual para o contexto de oficina com base na narrativa fornecida
Narrativa:

    Sistema de controle e gerenciamento de execução de ordens de serviço em uma oficina mecânica
    Clientes levam veículos à oficina mecânica para serem consertados ou para passarem por revisões  periódicas
    Cada veículo é designado a uma equipe de mecânicos que identifica os serviços a serem executados e preenche uma OS com data de entrega.
    A partir da OS, calcula-se o valor de cada serviço, consultando-se uma tabela de referência de mão-de-obra
    O valor de cada peça também irá compor a OS
    O cliente autoriza a execução dos serviços
    A mesma equipe avalia e executa os serviços
    Os mecânicos possuem código, nome, endereço e especialidade
    Cada OS possui: n°, data de emissão, um valor, status e uma data para conclusão dos trabalhos
 
 ## Resolução:
  Algumas informações não apresentadas na narrativa foram adcionadas:
	
	Nome, Telefone e E-mail do cliente
	Marca, Modelo e Ano do Veiculo
	Numero da Equipe de mecanicos
	
-----

	Foram utilizadas relações N-M da mão de Obra, Peças, e Serviços para a Ordem de Serviço
	Foram utilizadas relações 1-1 entre Veiculo e Equipe, e entre veiculo e Ordem de Serviço
	Foi utilizada relação 1-N entre cliente e veiculo  
