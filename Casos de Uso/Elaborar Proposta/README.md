# **Especificação do Caso de Uso: Elaborar Proposta**
**Ator Primário:** Vendedor (Felipe/Gabriela) Ator Secundário: Gerente Geral (Bruna) — acionada via include

**Pré-condição:** O Vendedor recebeu uma solicitação de livros de um cliente cadastrado.

#Fluxo Principal
1. O Vendedor inicia a elaboração da proposta selecionando o pedido do cliente.

2. O Sistema executa o caso de uso incluído "Pesquisar Livros":
Nota: O vendedor busca em catálogos de editoras, distribuidoras e na internet/sebos para encontrar onde comprar, o prazo e o preço de custo.

3. O Vendedor registra os detalhes de custo (preço do fornecedor) e estimativa de frete de aquisição para cada livro encontrado.

4. O Sistema solicita a definição do preço de venda (aciona o caso de uso incluído "Definir Preço de Venda").

Nota: A lista é passada para a Gerente Geral (Bruna), que define o preço baseada em câmbio e margem de lucro.

5. O Sistema retorna os itens com os preços de venda já definidos.

6. O Vendedor calcula o frete final de envio para o cliente.

7. O Sistema consolida as informações e gera o documento preliminar da proposta.

8. O caso de uso termina com a proposta pronta para ser enviada (o envio é o próximo caso de uso no seu diagrama).

#Fluxos Alternativos

A1. Cotação Pendente (Pausa no Processo)

Cenário: Durante a pesquisa (passo 2), o vendedor não consegue o preço de custo imediatamente (precisa ligar ou mandar email para um fornecedor externo).

  1. O Vendedor marca o item como "Aguardando Cotação".

  2. O Sistema salva o estado da proposta como "Pendente" ou "Em Andamento".

  3. O caso de uso é suspenso temporariamente.

  4. Retomada: Quando a resposta chega, o Vendedor reabre a proposta, insere o valor e o fluxo retorna ao passo 3 do fluxo principal.

A2. Livro Não Encontrado

Cenário: O livro é muito raro e não foi encontrado em nenhum fornecedor.

  1. O Vendedor marca o item como "Indisponível".

  2. O fluxo segue para o próximo livro da lista.

  3. Se nenhum livro for encontrado, a proposta é gerada informando a indisponibilidade total (ou o processo é encerrado notificando o cliente).
