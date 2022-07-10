# Introdução à programação e ao pensamento computacional :computer:

Olá. Este é o espaço onde transcreverei todas as minhas anotações sobre a matéria "Introdução à programação e ao pensamento computacional". Para facilitar o entendimento eu dividi minhas anotações por tópicos. São eles:

- Pensamento computacional;
- Introdução à lógica de programação;
- Fundamentos de algoritmos;
- Linguagens de programação;

### Pensamento computacional

-> É o processo de pensamento envolvido na expressão de soluções em passos computacionais ou algoritmos que podem ser implementados no computador. 

-> É voltado para a resolução de problemas.

O pensamento computacional é baseado em 4 pilares:

1 - Decomposição (dividir o problema em subproblemas);

2 - Reconhecimento de padrões (Identificar padrões ou técnicas);

3 - Abstração (Extrapolar o conceito do problema para uma forma generalista);

4 - Design de algoritmos (Definir passo a passo da solução do problema).

O pensamento computacional é um processo contínuo, onde é necessário procurar outras soluções através de outros pontos de vista. Esse ciclo é composto por: refinamento, teste e análise.

#### Habilidades complementares

Raciocínio lógico: é uma forma de pensamento estruturado que permite encontrar a resolução ou conclusão de um problema. O raciocínio lógico classifica-se em: indução, dedução e abdução.

-> Indução: a partir de ciências experimentais desenvolve-se leis e teorias.

-> Dedução: está diretamente relacionada às ciências exatas, àquelas que precisam de comprovação a partir de leis e teorias.

-> Abdução: a partir de uma conclusão cria-se uma premissa, como por exemplo, no processo investigativo.

Após formular soluções para o problema é necessário que ela seja aperfeiçoada, determinando pontos de melhora e refinamento, esse é o método de aperfeiçoamento.

Vantagens do ato de aperfeiçoar: 

- Encontrar soluções mais eficientes;
- Otimizar processos;
- Simplificar linhas de código;
- Funções bem definidas.

Ou seja, em outras palavras pode-se dizer que há um melhor uso de recursos e melhora de códigos e algoritmos.

### Pilares do pensamento computacional

- **Decomposição**: É o primeiro passo da resolução de problemas dentro do conceito de pensamento computacional, uma definição aplicável seria: "dado um problema complexo, devemos quebra-lo em problemas menores, ou seja, mais fáceis e gerenciáveis."

  Para isso, há estratégias que podem ser seguidas: 

  O primeiro passo é a análise, que consiste no processo de quebrar e determinar partes menores e gerenciáveis. Em seguida há a síntese, que é a combinação dos elementos recompondo o problema original. A ordem de execução de tarefas menores pode ser realizada tanto de forma sequencial (com ordem de execução definida) quanto paralela (sem ordem definida).

**Padrões**: Consiste em identificar similaridades e diferenças do problema. 

-> Por que determinar padrões?

Generalizar com o objetivo de obter resoluções para problemas diferentes.

-> Como o computador reconhece padrões?

O computador reconhece padrões por comparação. Para isso, é necessário apresentar atributos à ele para que aprenda o conceito associado ao objeto e através de regras de decisão, consiga relacionar a qual grupo aquele objeto pertence e armazene os dados.

-> Algumas aplicações e áreas que utilizam o reconhecimento de padrões:

-**Aplicações**: 

- classificação de dados
- reconhecimento de imagem
- reconhecimento de fala
- análise de cenas
- classificação de documentos

-**Áreas**:

- Machine learning
- Redes neurais
- Inteligência artificial
- Ciência de dados

**Abstração**: Define-se como o processo intelectual de isolamento de um objeto da realidade.

-> Como classificar os dados? 

- Características
- Pontos essenciais
- Generalizar x Detalhar

->Representação de dados:

-  Considerar os pontos essenciais

-> Conceitos baseados em abstrações:

- Merge sort;				  Máquinas de estado infinito;		  Clusteting;				
- Busca binária ;			Linguagens de programação;   	  Comunicação;	 
- Árvore;  					  Área de rede (cliente-servidor);       Lista;
- Grafo



**Algoritmos**: Processo de resolução de problemas "step by step" (passo a passo) utilizando instruções. Os algoritmos não operam sozinhos. 

- Processamento de dados: o computador recebe, manipula e armazena os dados.

  -> O algoritmo precisa ser entendido por um humano ou uma máquina.

Desenvolvimento do programa

-> Análise: Estudo e definição dos dados de entrada e saída.

-> Algoritmo: Descreve o problema por meio de ferramentas narrativas, fluxograma ou pseudocódigo.

-> Codificação: O algoritmo é codificado de acordo com a linguagem de programação escolhida.

Como construir um algoritmo?

- Compreensão do problema (pontos mais importantes);
- Definição dados de entrada (dados fornecidos e cenários);
- Definir processamento (cálculos e restrições);
- Definir dados de saída (após o processamento);
- Utilizar um método de construção;
- Teste e diagnóstico (construção e refinamento do algoritmo).

Tipos de algoritmos:

-> Narrativa: usa a linguagem natural e pode ter vários sentidos;

-> Fluxograma: estrutura gráfica com símbolos pré-definidos que definem qual tipo de ação que está sendo executada. Simples entendimento.

->Pseudocódigo (ou portugol): possui passos a serem seguidos e é o mais próximo de uma codificação.

# Lógica de programação

O que é lógica?

Surge para solucionar problemas. É uma forma de pensamento estruturado que ajuda a determinar o que é verdadeiro ou não. 

#### Técnicas de lógica de programação

-**Técnica Linear**: É uma ordenação de elementos por uma única propriedade. 

- modelo tradicional
- não tem vínculo
- estrutura hierárquica
- programação de computadores
- execução sequenciada

-**Técnica estruturada**: Organização, disposição e ordem dos elementos essenciais que compõem um corpo (concreto ou abstrato). Não é linear, ou seja, não segue  uma sequência.

No processamento de dados seus objetivos são: escrita, entendimento, validação e manutenção.

-**Técnica modular**: São partes independentes controladas por um conjunto de regras. Ela possui dados de entrada, processo de transformação e dados de saída e seus objetivos são simplificação, decompor o problema e verificação de cada módulo independentemente.

# Fundamentos de algoritmos

Tipologia e variáveis

-> A função do computador é processar as informações que passamos a ele. Estas informações são compostas de dados e instruções.

   ->Instruções: são normativas usadas pelo computador para executar determinadas ações que irão processar os dados.

 ->Dados: são objetos de manipulação e processamento de um computador. Eles são tratados e processados. Os dados podem ser dos tipos numéricos, caracteres e lógico.

- Numéricos: São os números inteiros (int) = positivos e negativos sem casas decimas e os números reais (float) = positivos, negativos e esses podem ter casas decimasi.
- Caracteres: É tudo aquilo que não é representado como número, eles possuem um limite de tamanho e as letras precisam estar entre aspas duplas.
- Lógico: Aqueles que resultam em verdadeiro (1) ou falso (0). Diretamente relacionado à lógica booleana.

#### O que é uma variável?

-> É uma estrutura mutável que possui variações. Ela recebe um dado e seu tipo.

-> Pode assumir qualquer valor de um conjunto de valores, porém, restrita ao tipo de dados.

Para nomear uma variável há um conjunto de regras a serem seguidas:

​	-Atribuição de um ou mais caracteres

​	-A primeira letra não pode ser um número

​	-Sem espaços em branco

​	-Não pode utilizar palavras reservadas da linguagem de programação em questão

​	-Caracteres e números

Papéis da variável:

​	-Ação: modifica o estado do algoritmo.

​	-Controle: vigia de algum programa, equação.

**Constante**: Tudo aquilo que é fixo ou estável.

#### Instruções primitivas

As instruções determinam as ações que serão executadas em cima dos dados, geralmente são cálculos matemáticos e para isso, utiliza-se operadores. Esses cálculos possuem como input as variáveis e as constantes, e eles podem ser binário ou unário. 

| Operador | Operação         | Tipo    | Prioridade matemática | Retorno         |
| -------- | ---------------- | ------- | --------------------- | --------------- |
| +        | manutenção sinal | unário  | 1                     | positivo        |
| -        | inversão sinal   | unário  | 1                     | negativo        |
| ↑        | exponencial      | binário | 2                     | inteiro ou real |
| /        | divisão          | binário | 3                     | real            |
| div      | divisão          | binário | 4                     | inteiro         |
| *        | multiplicação    | binário | 3                     | inteiro ou real |
| +        | adição           | binário | 4                     | inteiro ou real |
| -        | subtração        | binário | 4                     | inteiro ou real |

**Estruturas condicionais e operadores**

-> Há uma condição que se for satisfeita a operação será executada, se for insatisfeita, a operação é exceção.

E.C.Simples: verifica se a condição foi satisfeita.

E.C.Composta: verifica se a condição foi satisfeita e se não foi é exceção.

E.C.Encadeada: sucessão de estruturas condicionais.

**Operadores relacionais:** 

| =    | igual            |
| ---- | ---------------- |
| <>   | diferente        |
| >    | maior que        |
| <    | menor que        |
| >=   | maior ou igual à |
| <=   | menor ou igual à |

**Operadores lógicos:**

AND -> é verdadeiro quando todas as condições são satisfeitas.

OR -> é verdadeiro se uma ou ambas forem satisfeitas.

NOT -> verdadeiro quando a condição falsa for insatisfeita.

**Estruturas de repetição**: irá repetir um determinado trecho de código a partir de parâmetros estabelecidos.

**Condições de parada**: Número de repetições pré-fixada

**Por que usar estruturas de repetição?**

- Redução de linhas

- Compreensão facilitada

- Redução de erro

  Alguns tipos: -> Enquanto ... faça

  ​						-> Repita ... até

​								-> Para ... de ... até ... faça

# Vetores e Matrizes

- Um vetor é caracterizado por uma variável dimensionada com tamanho pré-fixado.
- Uma matriz é uma tabela organizada em linhas e colunas (mxn), m = n° de linhas (horizontal), n = n° de colunas (vertical).

# Funções

- São blocos de instruções (códigos) que realizam tarefas especificas; modularização do problema.

Vantagens de usar: 

- Modularização do problema;
- Código mais simples e conciso;
- Reutilização de instruções;

# Instruções de entrada/saída

**Entrada**: Inserção e recebimento de dados do mundo real por meio de ação de alguma interface, seja teclado, mouse, arquivos, etc.

**Saída**: Impressão dos dados do mundo abstrato, digital, por meio de alguma interface. As saídas podem ser programadas (condicional ou não) ou por interrupção.

​	Casos de saída: 

​	-bem sucedida

​	-erro de sintaxe ou outro

​	-erros de programação

​	-problemas com a interface

# Como o computador entende o programa?

Pelo processo de tradução: uma linguagem de alto nível passa pelo compilador e é transformada em uma linguagem de baixo nível, que o computador entenda.

**Interpretação**: o programa fonte é executado diretamente.

**Diretrizes para desenvolver programas**: 

- Legibilidade
- Redigibilidade
- Confiabilidade
- Custo

## Análises de código

-> **Análise léxica**: É a primeira fase do processo de compilação. Sua função é fazer a leitura do programa fonte e agrupar os caracteres em sequências léxicas (tokens).

-> **Análise sintática**: É a forma que define através de palavras reservadas, indexação, qual é a estrutura relacionada para a codificação, dentro daquela linguagem específica.

-> **Análise semântica**: Estuda o significado. Incide sobre a relação entre significantes, como: palavras, frases, sinais e símbolos.

### Paradigmas de programação

-> **Estruturado**: sequência, decisão (teste lógico), iteração (funções, laços, condições). 

​	->Problemas específicos e diretos.

-> **Orientação a objetos**: baseado na utilização de objetos e suas iterações; análogo ao mundo real; um objeto possui atributo, comportamento e métodos.

​	->Reuso de código.

Pilares da orientação a objetos:

- Herança
- Encapsulamento
- Polimorfismo
- Abstração
