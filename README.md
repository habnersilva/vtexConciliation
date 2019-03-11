# vtexConciliation
######  O proposito do Marketplace Conciliation e facilitar a gestão e repasse dos pagamento recebido dos marketplaces para o seller.

### Dos Recursos ###

## ##

> Cadastrar Usuario

> Editar Usuario  

> Deletar Usuario

> Efetuar Login  

> Efetuar logoff

##### Obs: #####
*Gerenciamento de usuario com ACL (Access control list)*

## ##

> Cadastro Função do Usuario (Role)

> Editar Função do Usuario

> Deletar Função do Usuario

## ##


> Importar Pedido

> Atualizar Pedido

> Deletar pedido

> Filtrar pedido

##### Obs: #####

*- Gereciamento dos pedidos dos marketplaces*

  *- Importação dos dados dos pedidos*

  *- Filtros para dados relevante, tais como: "Seller, status, data, entre outro"*

  *- Paginação*

  *- Inserção de novos dados com "Observação"*

##### Regras: #####
- Trazer o campo de Identificação da Vtex 
- Trazer quem é o seller
- Trazer qual é o marketplace
- Trazer quem é o cliente
- Trazer a data do pedido
- Trazer a data do faturamento (data de autorização)
- Calcular a data de vencimento que o marketplace irá pagar o pedido
- Trazer o valor total do pedido
- Trazer o valor apenas do produtos
- Adicionar a informação se o marketplace já pagou o pedido
- Calcular o comissão do Marketplace
- Calcular a comissão da Vtex
- Calcular a comissão da Look Lovers
- Calcular a comissão da YMI
- Calcular a comissão da Moip
- Calcular o imposto
- Soma o custos de comissionamento
- Soma o custo da Operação (Custos de comissionamento + imposto)
- Calcular o valor do repasse ( Valor dos produtos + custo da Operação )
- Trazer valor do frete
- Adiconar a valor do frete real
- Calulcar diferente do frete (frete - frete real)
- Valor da NF a tirar para Seller (valor apenas do produtos - valor do repasse)
- Adicionar a informação se o pedido é de um unico seller ou foi splitado
- Caso o pedido seja splitado será necessário o fracionamento do mesmo

## ##

> Cadastrar Marketplace

> Editar Marketplace

> Deletar Marketplace

##### Obs: #####

*- Marketplaces deverão ser cadastros com as seguinte dados:*

*- Sigla do Marketplace (para relacionamento com pedidos)*

*- Comissão do Marketplace percentual*

*- Comissão do Marketplace fixo*

*- Prazo de pagamento do Marketplace em dias*

## ##

> Cadastrar Comissionantes

> Editar Comissionantes

> Deletar Comissionantes

##### Obs: #####

*- Vtex, deverá armazenar a aliquota de comissionamento sendo o valor percentual*

*- Look Lovers, deverá armazenar a aliquota de comissionamento sendo o valor percentual*

*- YMI, deverá armazenar a aliquota de comissionamento sem o valor fixo*

*- MOIP, deverá armazenar as aliquota de comissionamento, sendo fixo e percentual*

*- Imposto, deverá armazenar a aliquota para calculo do imposto*

## ##

> Emitir relatório por Seller no periodo

> Emitir relatório Logistico por periodo

##### Obs: #####

*- Relatorios com os pdidos a serem e pagos e devoluções a serem estornadas*

*- Relatorio com saldo dos frete e amostra do frete pagos confortados com os frete simulados* 

##### Regras #####
- Fechamento por periodo do Pagamento aos Seller
  - Relatar pedidos pagos com valores
	- Relatar devoluções realiza como valores
	- Ao final trazer o saldo do periodo
- Fechamento por periodo da Logistica
	- Valor de entrada e saida dos frete por pedido
	- Saldo do frete
	- Percentual de diferença entre frente real e simulado
