# **Especificação do Caso de Uso: Solicitar Livro**
**Ator Primário:** Cliente (Felipe/Gabriela)

**Pré-condição:** -

# Fluxo Principal
1. Cliente faz o login no sistema

2. Sistema identifica o cliente e apresenta a tela principal da aplicação

3. Cliente seleciona a opção de solicitar livros

4. Sistema apresenta a tela de solicitação com os campos de especificação 

5. Cliente informa o nome do livro que deseja e outros dados de especificação (edição, tradução por Fulano, assinado pelo autor, etc)

6. Sistema confirma especificação do livro ao cliente.

7. Cliente pede o registro da solicitação

8. Sistema cria um novo pedido de livro(s) ligado à conta do cliente.

9. Sistema informa a criação do novo pedido com sucesso ao cliente.

10. Cliente faz logout.

# Fluxos Alternativos

1A. Cliente não cadastrado

Cenário: Cliente ainda não possui cadastro

  1A.1 Sistema informa cliente e o redireciona para a página de cadastro.

  1A.2 Executar Cadastrar Cliente

  1A.3 Voltar para o passo 1. 

3B. Cliente Inadimplente

Cenário: Cliente foi marcado como inadimplente e precisa quitar os pedidos ainda à pagar para realizar um novo pedido.

   1B.1 Sistema informa cliente de inadimplência e o redireciona para a página do respectivo pedido
   
   1B.2 Cliente paga a dívida pelo meio disponível

   1B.3 Sistema confirma pagamento

   1B.4 Continuar do passo 4.

7A. Múltiplos livros

Cenário: Pedido consiste de mais de um livro

   7A.1 Voltar para o passo 5

8A. Erro ao criar novo pedido

Cenário: Um erro do sistema impede a criação do pedido

    8A.1 Sistema informa cliente do erro e pede para tentar novamente mais tarde

    8A.2 Sistema encerra pedido e volta à tela inicial da aplicação.