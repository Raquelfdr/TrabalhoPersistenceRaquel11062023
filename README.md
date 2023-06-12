# PersistenceTrabalho

Sistema de cadastro de produtos e pedidos em um portal de e-commerce utilizando: Spring Data JPA + Cache Redis
A escolha acima foi por ser a menos complexa.

1 - Modelo Entidade Relacionamento - MER
@ManyToMany para estabelecer a relação pedidos x produtos, já que um pedido pode ter n produtos e um produto pode estar em n pedidos. 
@OneToMany para estabelecer a relação cliente x pedido, já que um cliente pode ter vários pedidos. 
@ManyToOne para estabelecer a relação cliente x pedido, já que vários clientes podem ter um número para cada pedido.

2 - Entidades criadas:
Cliente
Produto
Pedido

Foram criados os respectivos controllers e services

Fluxograma do projeto: Realizar o cadastro do cliente >>> Realizar o cadastro do produto >>> Realizar o cadastro do pedido >>> Realizar a compra e incluir os produtos em um pedido.
