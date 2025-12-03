# EEL873-LivrariaResolve
Repositório do trabalho da disciplina EEL873 (Engenharia de Software) do Grupo P (Thiago Motta, Pedro Mangrich, Pedro Rodrigues e Davi da Costa). Trabalho tem como base um sistema de atendimento a clientes da Livraria Resolve, uma livraria especializada em livros raros e de alto valor agregado, os quais, geralmente, já saíram de catálago.

# Tarefa 1: Relatório de Entrevista com Proprietário (5W2H)

Foi realizada uma entrevista na empresa com o proprietário da Livraria Resolve, Arnaldo Américo, da qual foram obtidas as seguintes informações.

## Descrição do Negócio

A Livraria Resolve atua no mercao de venda de livros de arte e livros raros, de colecionadores, sob encomenda. A livraria recebe dos clientes pedidos de livros, os quais são adquiridos via editoras, distribuidoras e vendedores pelo mundo todo. Tais pedidos são encaminhados para as fontes com os livros correspondentes semanalmente (toda sexta-feira). Quando recebidos, um pedido de pagamento é enviado aos clientes. Assim que pagos, os livros são enviados junto de uma nota fiscal (cópiasde notas fiscais e boletos são encaminhadas para o contador terceirizado da empresa). 

- Clientes devem estar cadastrados antes de enviarem pedidos, e são avisados caso tentem um pedido sem cadastro pelo mesmo meio de contato usado pelo cliente (Ex: e-mail).
- O cadastro requer certas informações pessoais e de contato já estabelecidas.
- Cadastros são autorizados por Arnaldo Américo (proprietário) ou Armando Américo (diretor).
- Pedidos são cancelados após 30 dias se a fonte não enviou o livro requisitado. O cliente é avisado por correio com o restante dos livros pedidos, se houverem, ou apenas o aviso é enviado.
- Alguns livros acabam em um estoque (sem manutenção) por problemas de venda.

## Objetivo

A prioridade atual do sistema é apoiar a equipe de vendas a realizar pedidos e manter clientes, com possibilidade de estender as funções para permitir vendas pela internet e auxiliar outras tarefas na empresa. A importância do apoio a vendas se dá pela perda de clientes por conta dos atrasos no processo de atendimento. 'Atendimento' é entendido na empresa como o pagamento e a entrega do livro solicitado pelo cliente, mas a experiência do mesmo com o negócio abrange também o cadastro e a solicitação de livros.

Antes de refinar o conceito do sistema, uma entrevista com o restante das partes interessadas (PIs) deve ser realizada.

# Tarefa 2: Identificação de Partes Interessadas

Uma planilha foi criada para registrar as partes interessadas, seus objetivos e os diferentes meios pelos quais estas podem impactar o projeto.
[Link da planilha](https://docs.google.com/spreadsheets/d/1DUdSgmw2rfjZduCucBqQiNxWH2wCIFqd32IC56AAFic/edit?usp=sharing)

# Tarefa 3: Identificação de Desejos

Foram coletados 5 funções desejadas pelas partes interessadas.
-  **(Must)** Venda de livros pela internet (Apoiadores: Proprietário, Diretor)(Resistentes: Gerente Geral)
-  **(Must)** Acompanhamento de pedidos  (Apoiadores: Gerente Geral, Vendedores)
-  **(Must)** Integração com sistema de contabilidade (Apoiadores: Gerente Geral, Vendedores, Gerente de TI)
-  **(Should)** Dados e fichas de clientes (Apoiadores: Diretor, Gerente Geral, Vendedores)
-  **(Should)** Relatório de compra/venda mensal (Apoiadores: Diretor)

# Tarefa 4 : Registro de Processos (BPMN)

A partir das entrevistas realizadas, os processos vigentes (_As-Is_) foram mapeados em forma de diagramas de linguagem BPMN. Os diagramas se encontram na pasta de **Processos** do repositório, com subdiretórios dedicados para cada processo identificado. Cada subdiretório contém um arquivo que pode ser acessado e modificado pelo site **bpmn.io**.

# Tarefa 5 : Histórias do Usuário

As histórias do usuário são representações sucintas dos requisitos funcionais que o sistema a ser desenvolvido precisa acatar para resolver os problemas do usuário e facilitar o alcance dos seus objetivos. As histórias do usuário do sistema atendendo a Livraria Resolve foram organizadas na mesma planilha da tarefa 2 (Partes Interessadas), em uma aba diferente.
[Link da planilha](https://docs.google.com/spreadsheets/d/1DUdSgmw2rfjZduCucBqQiNxWH2wCIFqd32IC56AAFic/edit?usp=sharing)

# Tarefa 6 : Casos de Uso

Os casos de uso são especificações dos requisitos funcionais expressas em formas de narrativas, que possuem o fim de apresentar de forma clara o que o sistema deve ser capaz de realizar em cenários normais e alternativos de operação. Os casos de uso identificados do sistema idealizado para a Livraria Resolve estão representado no Diagrama de Casos de Uso na pasta **Casos de Uso**, e alguns casos de uso em si estão descritos em subdiretórios da mesma pasta.

# Tarefa 7: Pontos de Função

Para a análise dos pontos de função do sistema idealizado da Livraria Resolve, foi primeiro realizado um modelo ER do mesmo. A partir deste modelo, forma inferidos os arquivos lógicos e as funções transacionais com base no modelo e nos requisitos funcionais representados pelas histórias do usuário e dos casos de uso. O modelo, o raciocínio para a contagem dos PFs e o resultado se encontram no diretório **Pontos de Função**.
