## **Projeto Lógico de um Banco de Dados para um cenário de E-commerce**

<br>

**Objetivo**

 <br>

  O objetivo do banco de dados Ecommerce é fornecer uma estrutura para gerenciar e analisar dados relacionados a uma plataforma de comércio eletrônico. O esquema foi projetado para suportar operações básicas de um e-commerce, incluindo o gerenciamento de clientes, produtos, pedidos, pagamentos, entregas, fornecedores e vendedores terceirizados.

  <br>

**Esquema do Banco de Dados**

<br>

  Tabela TipoCliente: Armazena os diferentes tipos de clientes, como Regular, Premium e VIP.

  Tabela Cliente: Contém informações sobre os clientes da loja.

  Tabela Produto: Armazena informações sobre os produtos disponíveis na loja.

  Tabela Pedido: Registra os pedidos feitos pelos clientes.

  Tabela RelacaoDePedidoProduto: Relaciona produtos aos pedidos, especificando a quantidade e o status de cada item.

  Tabela Pagamento: Contém informações sobre os pagamentos dos pedidos.

  Tabela Entrega: Registra as informações de entrega dos pedidos.

  Tabela Fornecedor: Armazena informações sobre os fornecedores de produtos.

  Tabela Estoque: Contém informações sobre os locais de armazenamento dos produtos.

  Tabela ProdutoEmEstoque: Relaciona produtos aos locais de estoque, especificando a quantidade disponível.

  Tabela ForneceuProduto: Relaciona fornecedores aos produtos que fornecem.

  Tabela TerceiroVendedor: Armazena informações sobre os vendedores terceirizados.

  Tabela TerceiroVendedorProduto: Relaciona vendedores terceirizados aos produtos que vendem.

  <br>

**Relacionamentos**

<br>
  
  Cliente e Pedido: Um cliente pode fazer vários pedidos (1:N).
  
  Pedido e RelacaoDePedidoProduto: Um pedido pode conter vários produtos (1:N).
  
  Produto e RelacaoDePedidoProduto: Um produto pode estar em vários pedidos (1:N).
  
  Pedido e Pagamento: Um pedido pode ter um ou mais pagamentos (1:N).

  Pedido e Entrega: Um pedido pode ter uma ou mais entregas (1:1).
  
  Fornecedor e ForneceuProduto: Um fornecedor pode fornecer vários produtos (1:N).
  
  Produto e ForneceuProduto: Um produto pode ser fornecido por vários fornecedores (1:N).
  
  Produto e ProdutoEmEstoque: Um produto pode estar em vários estoques (1:N).
  
  Estoque e ProdutoEmEstoque: Um estoque pode conter vários produtos (1:N).
  
  TerceiroVendedor e TerceiroVendedorProduto: Um vendedor pode vender vários produtos (1:N).
  
  Produto e TerceiroVendedorProduto: Um produto pode ser vendido por vários vendedores (1:N).

  <br>

**Considerações**

 <br>

  O esquema do banco de dados foi projetado para suportar a gestão eficiente de um e-commerce, facilitando a recuperação de informações detalhadas sobre clientes, produtos, pedidos e fornecedores. A estrutura permite consultas complexas para análise de vendas, gerenciamento de estoque, e relacionamento entre produtos e fornecedores, garantindo uma visão abrangente das operações comerciais.
