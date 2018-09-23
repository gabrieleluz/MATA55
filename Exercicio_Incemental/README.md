EXERCÍCIO INCREMENTAL – ETAPA 1

A finalidade do exercício incremental deste semestre, cujas etapas vão sendo definidas e publicadas no Moodle periodicamente, é criar ao final um pequeno aplicativo para controle de movimento para consumo em bares, restaurantes e similares. A ideia é que esse aplicativo seja desenvolvido por etapas, de acordo com a evolução do conhecimento do aluno em POO. Todos os conceitos vistos até então estarão presentes no momento de cada exercício incremental.

**IMPORTANTE**: Todos os atributos das classes descritas devem ser criados como private e todos eles devem possuir métodos acessores (get e set).
Para esta primeira etapa você deve fazer o seguinte:

- Criar uma classe Produto que deve conter os seguintes atributos: codigo (int), nome (String), tipo (int), preco (double) e disponibilidade (boolean). O tipo pode conter os valores 0 (bar), 1 (cozinha) e 9 (outros). Esta classe possui dois construtores, um recebendo os valores de codigo, nome e tipo como parâmetros e outro recebendo, além destes, também disponibilidade e preco como parâmetros. Um dos métodos construtores deve referenciar o outro para instanciação.
- Criar uma classe Pedido que deve conter os seguintes atributos: numero (int), produto (objeto da classe Produto) e status (int) – se aberto (0), servido (1) ou cancelado (9). Esta classe vai possuir dois construtores, um recebendo apenas os valores de numero e produto como parâmetros e outro recebendo, além destes, também o status como parâmetro. Um dos métodos construtores deve referenciar o outro para instanciação. Considere o status padrão como 0 (aberto) quando ele não for informado. Além dos métodos acessores já mencionados, deve existir o método servir, que coloca o status em 1 e também o método cancelar, que coloca o status como 9.
- Criar uma classe Movimento que deve conter como atributo mesa (int), a dataAbertura (classe java.util.Calendar), o dataFechamento (java.util.Calendar) e o status (int), que pode assumir os seguinte valores: 0 = aberto, 1 = em pagamento e 9 = encerrada. Além desses, ela deve conter um atributo pedidos representando um array da classe Pedido. A classe Movimento possui um único método construtor recebendo apenas valores para dataAbertura e o número da mesa, deixando o atributo status com o valor ZERO. Além dos métodos acessores já mencionados, ela deve ter o método pagar, que recebe como parâmetro o valor de dataFechamento, colocando o status em 1. Deve ter também o método fechar, que recebe como parâmetro o novo valor de dataFechamento, colocando o status como 9.

Interessante conhecer um pouco mais da classe java.util.Calendar antes de criar a classe Movimento. Veja um pouco sobre ela em https://docs.oracle.com/javase/8/docs/api/java/util/Calendar.html

**ATENÇÃO**: Os nomes dos atributos e classes devem ser obedecidos conforme descritos e deve ser utilizada a convenção de nomenclatura da comunidade Java.
Mais detalhes sobre a convenção para codificação da linguagem de programação java, especialmente convenções de nomenclatura (Naming conventions), você encontra em http://www.oracle.com/technetwork/java/javase/documentation/codeconvtoc-136057.html.