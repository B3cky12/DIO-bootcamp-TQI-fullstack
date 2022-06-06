# Introdução a Programação e Pensamento Computacional

###### Iniciado: May 26, 2022 11:46 AM
###### Completo: Yes
###### Teacher: [Juliana Mascarenhas](https://github.com/julianazanelatto)
###### [Link da Aula](https://web.dio.me/course/introducao-a-programacao-e-pensamento-computacional/learning/285a4323-c6b0-4233-988e-4a2954065de3?back=/track/tqi-fullstack-developer&tab=undefined&moduleId=undefined)
###### [Slide da Aula](https://drive.google.com/file/d/1vemC6G790JNte1882V53DAKEawJzVIWL/view)

##

Pensamento computacional ou lógica de programação é algo aplicável a qualquer área de conhecimento, não só para programação e TI, mas pra qualquer local onde resolução de problemas é uma skill importante.

<details>
    <summary>Summary</summary>
    
     - Pensamento Coomputacional
     - Introdução a lógica de programação
     - Fundamentos de Algoritmos
     - Linguagens de Programação
     - Primeiro contato com a Programação
    
</details>

# Pensamento Computacional

// Os primeiros passos para começar a programar

## Introdução

**Definição:** O processo de pensamento envolvido na expressão de soluções em passos computacionais ou algoritmos que podem ser implementados no computador.

Olha, o pensamento computacional não se limita ao computador, o que significa que o pensamento computacional é o pensar no passo a passo que vai levar a solução para o problema em questão. Pensando assim, percebe-se que o pensamento computacional é mais uma skill do que um assunto acadêmico de um curso específico, e está presente não só dentro do mundo tecnológico, mas também na matemática, na leitura, na escrita, no planejamento, etc.

Seus pilares em que se divide são: Decomposição, reconhecimento de padrões, abstração e design de algoritmos. Não que pra todo problema seja necessário a união da força dos 4 pilares pra resolvê-lo, mas normalmente sim.

Dentre as competências adquiridas na utilização do pensamento computacional podem ser percebidos o pensamento sistemático, a colaboração dentro da equipe, a criatividade e design, e tudo isso acaba facilitando a resolução do problema.

## Habilidades complementares

As habilidades mais necessárias ao pensamento computacional é o raciocínio lógico e o aperfeiçoamento, super atreladas a resolução de problemas.

Raciocínio lógico é uma forma de pensar estruturadamente de forma que se chegue a uma conclusão, e pode ser classificado em indução, dedução e abdução. Indução é você generalizar uma teoria a partir de um fenômeno específico, a dedução, sendo o oposto, é você especificar um fenômeno a partir de uma teoria geral. A abdução é um pouco diferente, pois a indução e a dedução tratam de ideias e teorias com fenômenos e casos, mas a abdução é você definir uma suposição a partir de um fato, elaborar uma premissa a partir de uma conclusão. Então, numa inferência, a abdução e a indução se encaixam numa síntese, e a dedução se encaixa na análise.

Aperfeiçoamento também pode ser chamado de refinamento, melhoramento, aprimoramento ou ato de aperfeiçoar, basicamente é você determinar pontos de melhora e refinamento quando já se tem uma solução, mas uma solução que pode ser mais eficiente ao seu objetivo, de forma local ou global. Nisso, pode ser possível fazer um uso melhor dos recursos, como encontrar uma outra solução mais eficiente ou otimizar processos da atual, ou então melhorar os códigos e algoritmos, simplificando as linhas ou verificando que as funções estão bem definidas. Todos são opções.

## Pilares

### Decomposição

> “If you can’t solve a problem, then there is an easier problem that you can solve: find it”. George Polya.
> 

I.e. um problema complexo e grande pode ser quebrado em problemas mais simples e menores, mais fáceis de serem resolvidos. Como fazer isso? Podemos usar a estratégia de análise, que é estudar e explorar o nosso problema a fim de encontrar os conjuntos independentes e complementares que formam o todo. E então fazermos a estratégia da síntese, que é construir, no caso aqui é reconstruir as partes, os elementos de cada parte que foi separado, fundindo-os de volta de maneira coerente, alcançando a solução pro problema total. Podemos fazer isso de maneira sequencial ou paralela.

Mas isso foi só teoria aqui, pra saber mesmo o que é decomposição só decompondo. Um passo a passo simplificado(?) seria: 

- Identifica ou coleta os dados;
- Agrega os dados;
- Encontra a solução e entrega a funcionalidade.

Basicamente: segmentar, interligar, recompor.

### Padrões

Podemos pensar em padrões como um modelo, algo que pode ser repetido conforme um molde base, recriando infinitas vezes uma estrutura invariável. Então, para conseguir um bom reconhecimento de padrões, encontrar padrões, precisamos prestar atenção em similaridades e diferenças, e é claro que estamos falando de grupos, múltiplos, muitos ou, ao menos, pelo menos 3 elementos, pois não há padrão onde não há um comparativo.

Nós naturalmente fazemos esse processo de reconhecimento de padrões, mas a máquina não. Por isso que para o pensamento computacional voltado a programação é importante que saibamos reconhecer, descrever e determinar os padrões para poder ensinar a máquina a fazer o mesmo. Realizamos isso fazendo uso de classes e categorias, através do grau de similaridade e então classificando em categorias conhecidas ou de um objeto desconhecido. Mas para a máquina poder fazer isso também, ela irá usar de comparação. O que pode dificultar aí é a falta de dados suficientes, pois o computador é objetivo, direto, simples e burro, ele não tem os dados por si só, o programador tem que entregar pra ele primeiro.

A partir daí, após o computador ter uma boa representação dos atributos e os conceitos associados a cada objeto, armazenamos os dados e podemos definir as regras de decisão.

Então, resumindo, a abordagem para detecção de padrão envolve a extração de características e a classificação de dados, o que pode usar de diferentes métodos para aplicar em diferentes contextos. Dentre as áreas dentro da Tecnologia que utilizam bastante o reconhecimento de padrões estão machine learning, redes neurais, inteligência artifical e ciência de dados, de uma forma ou outra.

### Abstração

Sabemos que abstrair é avaliar características e propriedades a partir da observação de um ou mais elementos, já a abstração é o processo intelectual de isolamento de uma objeto da realidade, e generalizar é tornar algo geral, extenso. Abstração/Generalização como pilar do pensamento computacional será a soma dessas três coisas.

Simplificando, é definir classes gerais pra envolver objetos com base em suas características e pontos essenciais. Classificar, observando os dados importantes e desconsiderando detalhes fúteis.

Conceitos existentes baseados em abstração.. lembra de estruturas? Então… todos eles eram TAD, né? Tipos abstratos de dados..

### Algoritmos

O computador é uma ótima ferramenta, no sentido de que é eficiente, rápido e trabalha muito sem gastar muita energia, mas apesar dos seus pros, ele não opera sozin. Ele não resolve problema se ele não receber instruções detalhadas, de uma forma bem simplificada, para que ele entenda o que fazer e como. No fim, o objetivo de um computador é receber, manipular e armazenar dados.

Os programas são constituídos de instruções, que o computador vai replicar, mas essas instruções precisam conter o que precisa ser feito e a ordem de execução, um passo a passo, de forma a ser entendido pelo homem e pela máquina. O algoritmo é esse passo a passo.

Pra desenvolver um programa, é preciso analisar, entender e definir os dados de entrada e saída, formular o algoritmo usando ferramentas narrativas (utilizando a língua nativa, mas pode ficar ambíguo), de fluxograma (estrutura gráfica simples, mas requer conhecimento dos símbolos) ou de pseudocódigo (portugol, esse você já conhece), e então codificar, traduzir os passos para código na linguagem de preferência.

Mas como construir um algoritmo?

1. Compreenda o problema, os pontos mais importantes;
2. Defina os dados de entrada, os dados fornecidos pelo contexto;
3. Defina o processamento, cálculos e restrições;
4. Defina os dados de saída, após o processamento;
5. Utilize um método de construção e refinamento;
6. Realize testes e diagnósticos.

## Estudos de caso

### Conceitual: Perdido

Você está perdido numa floresta.Você olha ao redor e se pergunta:”Como que eu consigo utilizar o pensamento computacional para maximizar minhas changes de sobrevivência?”.

Primeiro podemos identificar mecanismos, recursos comuns e os detalhes mais importantes, ou seja, preciso de abrigo, comida e água. Para o abrigo eu preciso de uma boa localização que seja quente e seco e me garanta proteção. Para a comida eu posso caçar e/ou coletar. Para a água eu posso procurar uma nascente ou coletar da chuva.

Para purificar a água, cozinhar a caça, garantir a proteção e o calor é necessário que eu tenha fogo, então fogo é um padrão, e para entender a localização eu preciso de um mapa, que pode ser criado através da abstração. Até então já fizemos decomposição, reconhecimento de padrões e abstração, agora só preciso comer. Para isso eu preciso preparar a comida, seguindo as etapas:

#### 1° opção
1. Pescar
2. Limpar o peixe
3. Assar o filé
4. Comer

#### 2° opção

1. Pescar
2. Limpar o peixe
3. Colocar água na panela 
4. Ferver a água
5. Fazer o cozido
6. Comer

E o mesmo processo de pensamento vai para encontrar a água, construir o abrigo, etc.

### Aplicado: Soma de um intervalo

Se tivermos uma sequencia de números, digamos, inteiros entre 1 e 100, e quisermos saber a soma, podemos encontrá-la de uma forma inteligente e eficiente.

1 + 100 = 101

2 + 99 = 101

3 + 98 = 101

4 + 97 = 101

Podemos perceber um padrão nessa decomposição específica, o número 101 se repete 100/2 vezes, o que facilita nossa conta: 101 * 50 = 5050

Podemos fazer uma generalização.

Soma de n° entre x e y, o intervalo é [x, y] e o resultado_repetido_padrao = x + y e o resultado vai ser y/2 * (y + x).

Então utilizando decomposição, reconhecimento de padrões e abstração, podemos desenvolver o algoritmo:

1. Recebe os valores (x e y)
2. Resolve y/2 = total
3. Resolve y+x = resultado_repetido_padrao
4. Acha o resultado final = total * resultado_repetido_padrao
5. Imprime final

### Aplicado: Adivinhe o número

Dado que existe um número misterioso que uma pessoa escolheu dentro de um intervalo, eu faço perguntas e as únicas respostas possíveis é sim ou não. Nesse jogo, chutar números aleatoriamente é ineficiente e perde muito tempo, mas se as perguntas forem do tipo “número é maior que x?” ou “número é menor que y?” é uma estratégia bem melhor.

Esse cenário nos lembra uma busca binária em um vetor. E nesse sentido um possível algoritmo seria:

1. ordenar o vetor
2. fazer o módulo de L/2
3. acessar a estrutura
4. comparar os valores
5. repetir até encontrar o número
6. imprimir “Busca bem sucedida”

<aside>
📎 Como aprimorar essa habilidade? Desafiando-se a explicar as decisões e o processo com palavras simples.

</aside>

# Introdução à Lógica da Programação

O conceito de lógica aplicada a programação.

## O que é lógica?

**Definição:** Parte da filosofia que trata das formas do pensamento em geral (dedução, indução, hipótese, inferência, etc.) e das operações intelectuais que visam à determinação do que é verdadeiro ou não.

Então é uma forma de pensar estruturadamente, um raciocínio coeso e com sentido. Passando isso para o universo da programação, entendemos que a lógica nos códigos garante a organização e planejamento das instruções, em um algoritmo, a fim de viabilizar o nosso programa.

> “Everybody in this country should learn how to program a computer because it teaches you how to think.” Steve Jobs.
> 

## Técnicas de lógica de programação

A primeira técnica disponível é a **técnica linear:**

- É um modelo tradicional;
- Não tem vínculo;
    - Estrutura hierárquica;
    - Programação de computadores;
- Execução sequenciada;
- Recursos limitados;
- Única dimenção;

É a ordenação de elementos por uma única propriedade.

A segunda técnica é a **técnica estruturada**, que se denota na organização, disposição e ordem dos elementos essenciais que compõem um corpo, ou seja, tem-se uma estrutura disposta de tal forma que segue uma ordem lógica. Para programas, usar esse tipo de técnica facilita a escrita, o entendimento, a validação e a manutenção.

A terceira técnica é a **técnica modular**, que trata de partes independentes (os módulos) que são controlados por um conjunto de regras, mas cada um tem o seu próprio e específico. O modelo padrão para essa técnica é:

Dados de entrada → Processo de transformação → Dados de saída

Com essa técnica nós conseguimos:

- Simplificação
- Decompor o problema
- Verificação por módulo

# Fundamentos de Algoritmos

## Tipologia e variáveis

O computador processa as informações que damos pra ele, definindo dados e instruções. Os dados são tratados e processados pelo computador, e podem se encaixar em um dentre vários tipos de dados existentes: numéricos, caracteres, lógicos… Os numéricos podem ser inteiros ou reais, os caracteres são todos os símbolos, até mesmo os dos números, dentro de aspas, e o lógico está atrelado a lógica booleana, sendo ou verdadeiro ou falso.

Uma váriavel é um tipo de estrutura que possui variações. Duh. Ela pode assumir qualquer valor de qualquer tipo de dado, mas uma vez que seu tipo for definido, ela está restrita a esse tipo. Para nomear variáveis existem algumas regrinhas, mas são mais boas práticas do que regras, porque cada linguagem pode ter suas peculiaridades quanto a declaração de variáveis. São estas:

- Atribuição de um ou mais caracteres
- A primeira letra não pode ser número
- Sem espaços em branco
- Sem usar palavras reservadas
- Caracteres e números são válidos

Varíaveis podem ser criadas com duas funções principais, de ação ou de controle, aquela sendo para modificar o algoritmo e essa pra vigiar o algoritmo. Algumas vezes precisamos de variáveis que sejam fixas e invariáveis, no caso, uma constante, e podemos sim criar variáveis com o propósito de não variarem. Algumas linguagens tem uma declaração específica para essa variável constante.

## Instruções primitivas

As instruções são comandos que iram tratar os dados, no caso de dados do tipo numérico, temos operadores aritméticos, como adição, subtração, divisão, etc. 

Cada linguagem terá um vocabulário específico próprio para realizar um comando, e outra linguagem pode realizar esse mesmo comando, mas representando-o com outra notação. Então o mesmo comando pode ser representado por notações distintas, com base na sintaxe particular de cada linguagem.

É importante também entender a entrada, processamento e saída dos dados em um algoritmo. 

## Estruturas condicionais e operadores

Se quisermos utilizar se alguma verificação no algoritmo temos as estruturas condicionais, o nome é porque dado uma condição uma operação é executada, se a condição for satisfeita, ou não, se não for. Essas estruturas podem ser simples, compostas ou encadeadas. A simples somente verifica a condição, a composta define uma exceção, e a encadeada trata de uma condicional dentro de uma condicional.

Para tratar as condições, utilizamos operadores relacionais, como o igual a, diferente de, maior que, menor que, maior ou igual a, menor ou igual a. Seus símbolos são normalmente os mesmos, mas dependendo da linguagem eles podem variar. Agora os operadores lógicos tendem a não mudar muito, são eles o and, or e not, e também servem para constituir as condições, quando precisamos de respostas simplificadas de sim ou não.

## Estruturas de repetição

Quando é necessário que um mesmo grupo de comandos sejam executados repetidamente, podemos usar uma estrutura de repetição pra poder escrever esses comando uma vez só, poupando linhas, tempo, compreensão e manutenção, além de evitar erros. Laços, controle de fluxo, malhas de repetição, loop são todos sinônimos de repetição. 

Quando construímos essa estrutura, definimos também uma condição de parada, sendo um número de repetições pré-fixada ou uma condição a ser satisfeita, para que o loop pare de repetir-se e o cursor saia do laço, evitando assim o loop infinito.

Pensando em tipos, existem 3:

- Enquanto … faça
    
    Condição no início. Número de repetições indefinida.
    
- Repita … até
    
    Condição no final. Número de repetições indefinida.
    
- Para … de … até … faça
    
    Condição no início. Número de repetições definida.
    

## Vetores e matrizes

Um vetor é uma variável que representa uma sequencia unidimencional de dados com tamanho pré-fixado.

Uma matriz é uma tabela organizada em linhas e colunas, de dimensão m x n. Quase como se fosse um grupo de vetores de mesmo tamanho, um em baixo do outro, e cada um identificado por um índice.

Essas estruturas mais complexas servem para facilitar nosso entendimento do código, a otimização, manutenção e a escrita do código, quando estamos lidando com muitos dados.

## O que são funções?

As funções em programação são similares ao conceito de função em matemática; são blocos de instruções que realizam tarefas específicas. A modularização do programa. Identificados por nomes e parâmetros.

As variáveis criadas dentro de uma função pertencem ao escopo local da função, dendo desalocadas da memória uma vez que a função encerra.

## Instruções de entrada/saída

A entrada consiste na inserção e recebimento de dados do mundo real por meio de ação de alguma interface, seja teclado, mouse, arquivos, entre outros. E então, após o processamento desses dados no algoritmo, a saída consiste na impressão dos dados do mundo abstrato, digital por meio de ação de alguma interface.

Para toda saída, ela ocorre de forma bem sucedida, ou por erro no código, ou por problema com a interface.

# Linguagens de Programação

## Introdução à linguagens de programação

História da computação. 2° Guerra Mundial e Guerra Fria. Ada Lovelace, Alan Turing, Von Neuman, Claude Shannon. ENIAC, EDVAC, COLOSSUS, Intel, Microsoft, Windows, Apple, IBM.

Assembly, a “primeira linguagem de programação”, era uma linguagem de montage, de máquina. COBOL, lisp, prolog, C, Java, C#, JS, python, Ruby, …

Os problemas computacionais são recorrentes. A necessidade de uma era gera espaço para inovação, e o que era inovação, depois de sua era, não é mais, e novas necessidades são a regra.

Uma linguagem de programação vai ser um método, um conjunto de regras que ao serem combinadas e movidas, podem alcançar um resultado esperado e, quem sabe, nunca visto antes.

## Como um computador entende o programa?

O código fonte é traduzido ou interpretado pelo computador para o computador, pois o computador não fala inglês, português, mandarim, etc.., o computador não fala linguagens humanas. Mas codamos com palavras humanas, então, pra que o computador entenda os dados e instruções do programa é necessário que o programa fonte passe por uma compilador gerando um programa objeto que está na linguagem de máquina. Esse processo se chama de compilação ou tradução.

Já a interpretação, o programa fonte é executado diretamente, o que pode ter suas vantagens e desvantagens em comparação com a compilação. Python é uma linguagem interpretada e C é uma linguagem compilada.

Mais recente, surgiu a técnica da transpilação, que seria o programa fonte ser escrito em uma linguagem de altíssimo nível e então ser transpilada para uma linguagem de nível um pouco mais baixo, mas ainda não de baixo nível, o que é muito interessante pois garante a flexibilidade do código de alto nível mas com uma execução um pouco mais rápida. Typescript é transpilado com JavaScript.

## Características de um programa

Na hora de pensar em desenvolver um programa, é bom pensar nos pontos:

- Legibilidade - ser legível;
    
    Facilidade de leitura, compreensão, ortogonalidade, definição adequada das estruturas.
    
- Redigibilidade - ser de facil escrita;
    
    Ortogonalidade, simplicidade da escrita, coerência nas instruções, suporte à abstração, reuso do código, expressividade.
    
- Confiabilidade - faz o que foi programado pra fazer;
    
    Verifique os tipos, trata das exceções, usa bem o recurso dos ponteiros, compatibilidade entre compiladores.
    
- Custo - anáçise de impacto;
    
    Treinamento, codificação, compilação, execução, infra-estrutura.
    
- Atualizações;
- Iso para IA;
- Disponibilidade de ferramentas;
- Comunidade ativa;
- Adoção pelo mercado.

## Análises de código

Durante a leitura de um código, algumas análises acontecem lá dentro.

- Análise léxica
    
    Ela é a primeira fase. Lê caractere por caractere e agrupa os caracteres por símbolos léxicos. Ela particiona o código, classifica os elementos (tokens) e eliminar as maquiagens (espaços em branco, comentários).
    
- Análise sintática
    
    A sintaxe é a forma, e a análise sintática é a corretude do programa. Extremamente dependente da linguagem específica utilizada.
    
- Análise semântica
    
    Está ligada ao estudo do significado e da lógica do programa; um erro de semântica seria quando o código não faz o que é esperado, mas eles são mais dificeis de se encontrar.
    

## Paradigmas de programação

Paradigma seria um exemplo de um padrão, um modelo complexo, uma estrutura, conceito ou procedimento que serve para instruir os movimentos e facilitar a resolução de um problema específico. Em programação podem ser classificados como paradigmas:

- Orientação à objeto;
- Procedural;
- Funcional;
- Estruturado;
- Computação distribuída;
- Lógico;

Os mais utilizados nas linguagens são a orientação à objetos e o estruturado.

# Primeiro contato com a Programação

## Algoritmos em pseudocódigo

    programa {

        funcao inicio() {
            inteiro x, y
    
            escreva(”Digite os números para executar a soma do intervalo: “)

            leia(x)

            leia(y)

            escreva(soma_intervalo(x,y))
        }

        funcao inteiro soma_intervalo(inteiro x, inteiro y) {

            inteiro total, resultado_parcial

            total = y/2

            resultado_parcial = y+x

            inteiro resultado = total * resultado_parcial

            retorne resultado

        }

    }

;;;;

    programa {

        funcao inicio() {

            real a1, a2, b1, b2

            escreva (”Digite a nota p1 e p2 do aluno A: “)

            leia(a1)

            leia(a2)

            escreva(”Digite as notas da p1 e p2 do aluno B: “)

            leia(b1)

            leia(b2)

            escreva(’Média do aluno A: “, media_aluno(a1, a2))

            escreva(”\nMédia do aluno B: “, media_aluno(b1, b2))

        }

        funcao real media_aluno(real nota_a, real nota_b) {

            retorne (nota_a + nota_b)/2

        }

    }
