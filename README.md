# __*RNA-Perceptron-java*__


[![Badge](https://img.shields.io/static/v1?label=Samuel&message=Ricardo&color=green&style=for-the-badge&logo=GITHUB)](https://github.com/Samuel-Ricardo)
[![Badge](https://img.shields.io/static/v1?label=License&message=MIT&color=green&style=for-the-badge&logo=GITHUB)](https://github.com/git/git-scm.com/blob/master/MIT-LICENSE.txt)

[![Badge](https://img.shields.io/static/v1?label=Made%20Whit&message=Java&color=red&style=for-the-badge&logo=JAVA)](https://www.java.com/pt-BR/about/whatis_java.jsp)
[![Badge](https://img.shields.io/static/v1?label=Made%20Whit&message=NetBeans&color=red&style=for-the-badge&logo=JAVA)](https://netbeans.apache.org/)
[![Badge](https://img.shields.io/static/v1?label=JDK&message=8&color=red&style=for-the-badge&logo=JAVA)](https://www.oracle.com/java/technologies/javase/javase-jdk8-downloads.html)

[![Badge](https://img.shields.io/static/v1?label=Artificial&message=Intelligence&color=green&style=for-the-badge&logo=GITHUB)](https://github.com/search?q=Artificial+Intelligence)
[![Badge](https://img.shields.io/static/v1?label=Neural&message=Network&color=green&style=for-the-badge&logo=GITHUB)](https://github.com/search?q=Neural+Network)
[![Badge](https://img.shields.io/static/v1?label=Perceptron&message=Project&color=green&style=for-the-badge&logo=GITHUB)](https://github.com/search?q=Perceptron)

[![Badge](https://img.shields.io/static/v1?label=Version&message=1.0.2&color=green&style=for-the-badge&logo=GITHUB)](https://github.com/Samuel-Ricardo/IA-Perceptron-java)
[![Badge](https://img.shields.io/static/v1?label=State&message=Finalized&color=green&style=for-the-badge&logo=GITHUB)](https://github.com/Samuel-Ricardo/IA-Perceptron-java)

/* As Tags São clicáveis ;) */
 
## __*Versão Atual (Finalizado):*__
- __*Notas da Versão 1.0.2*__
  
# __*Informações Gerais:*__
- __*Autor:*__ [Samuel Ricardo Cabral de Barros](https://github.com/Samuel-Ricardo)

- __*Estado:*__ Finalizado

- __*Versão Atual:*__ 1.0.2

## __*O que foi Usado*__
- __*[Java](https://www.java.com/pt-BR/about/whatis_java.jsp)*__,
- __*[NetBeans](https://netbeans.apache.org/)*__
 
## __*O que é necessário para rodar:*__
- __*[JDK](https://www.oracle.com/java/technologies/javase-downloads.html)*__,
- __*alguma IDE*__,
	- __*Recomendado:*__ [Eclipse](https://www.eclipse.org/) ou [NetBeans](https://netbeans.apache.org/download/index.html)

## __*Fontes:*__ 

- __*Vídeo*__ -
[Redes Neurais Artificiais, Perceptron Simples (Parte 1): Problema, Arquitetura e Componentes](https://youtu.be/PMfarAZdNSA) 
	- __*do Canal:*__ [Serafim Nascimento](https://www.youtube.com/channel/UC4nbGdTDlcNrbZGVt732lmQ)
    
> [![Redes Neurais Artificiais, Perceptron Simples,Parte 1: Problema, Arquitetura e Componentes](http://img.youtube.com/vi/PMfarAZdNSA/0.jpg)](http://www.youtube.com/watch?v=PMfarAZdNSA "Redes Neurais Artificiais, Perceptron Simples, Parte 1: Problema, Arquitetura e Componentes")



# __*RNA-Perceptron-java*__


Nesse Projeto é realizada a **criação de uma [Rede Neural](https://pt.wikipedia.org/wiki/Rede_neural_artificial#:~:text=Em%20ci%C3%AAncia%20da%20computa%C3%A7%C3%A3o%20e,como%20o%20reconhecimento%20de%20padr%C3%B5es.) [Perceptron](https://en.wikipedia.org/wiki/Perceptron)** utilizando a linguagem Java, sua função é **descobrir se os dados enviados para ele representa um ser vivo ou não.**

É o meu **primeiro projeto**, foi feito inicialmente em algoritmos com [VisualG](https://visualg3.com.br/) posteriormente passado para Java, sendo assim meu primeiro projeto Java após finalizar os estudos em algoritmos, é também **o projeto que deu início ao meu github.**

Este projeto não usa nenhuma **interface gráfica**, a interação ocorre a partir do **terminal** da IDE, utilizando o comando 
```java
System.out.print(“”);
``` 
e a 
```java
java.util.Scanner
``` 
para obter os dados de input (Entrada de dados).
 
Os procedimentos são baseados em lógica, ou seja, ele **não depende da linguagem de programação**, a mesma lógica pode ser aplicada a **qualquer** outra linguagem, incluindo algoritmos como o VisualG.
 

## __*Conversão de dados*__
 
As **redes neurais entendem apenas [bits](https://pt.wikipedia.org/wiki/Bit#:~:text=O%20bit%20(simplifica%C3%A7%C3%A3o%20para%20d%C3%ADgito,ou%20passagem%20de%20energia%2C%20respectivamente. )**, por isso, de alguma forma, deve ser feita uma conversão dos dados para bits fazendo com que a rede neural seja capaz de compreender e processar os dados, um exemplo simples seria utilizar  1 (Verdadeiro) ou 0 (falso) para indicar se um funcionário está empregado ou desempregado.
 
No caso desta atividade os dados são **letras** (nomes de seres vivos e de objetos) porém, como visto, redes neurais não entendem letras, então foi necessário realizar a **conversão das palavras para bits.**

Possuímos **8 valores (palavras)**, então foi preciso descobrir com **quantos bits se consegue representar até 8 valores**, sabendo que:

 **1 bit**  consegue representar a **2 valores (0 / 1)**

 temos 2 (**número de valores possíveis para 1 bit**) ^ N (**quantidade de bits**)
 
 logo:

#
 - 1 bit **->** 2^1 = 2 valores  

   - 0 e 1
#
 
 - 2 bits **->** 2^2 = 4 valores 
 
   - 00, 01, 10, 11
# 
 
 - 3 bits **->** 2^3 = 8 valores 

   - 000, 001, 010, 011, 100, 101, 110, 111
#   
   
   
> ![Conversao de dados](https://github.com/Samuel-Ricardo/IA-Perceptron-java/blob/master/Readme/Conversao_de_dados.jpeg)
   
   
   
   
após chegar no resultado, resta escolher qual palavra (valor) cada bit vai representar, 

__*Nomes*__ | __*Bits*__
------|-----
Peixe | 000
Colher | 001
sapo | 010
cachorro | 100
aquario | 011
pessoa | 110
agulha | 101
feijao | 111
 
 
- como é mostrado neste trecho do código.
 
 ```java
 
 System.out.println("----------------------------");  
        System.out.println("//Descubra se é Ser Vivo: //");
        System.out.println("----------------------------");
        System.out.println("+(1)-peixe                 +");
        System.out.println("+(2)-colher                +");
        System.out.println("+(3)-sapo                  +");  
        System.out.println("+(4)-cachorro              +");
        System.out.println("+(5)-aquario               +");
        System.out.println("+(6)-pessoa                +");
        System.out.println("+(7)-agulha                +");
        System.out.println("+(8)-feijao                +");
        System.out.println("----------------------------");
        
        option = tec.nextInt();

        switch (option) {  //converte nome escolhido para bits
              
        case 1:
           x[1] = 0;
           x[2] = 0;
           x[3] = 0;
         
        break;
        
        case 2:
           x[1] = 0;
           x[2] = 0;
           x[3] = 1;
           
        break;
        
        case 3:
           x[1] = 0;
           x[2] = 1;
           x[3] = 0;
           
        break;
        
        case 4:
           x[1] = 1;
           x[2] = 0;
           x[3] = 0;
           
        break;
        
        case 5:
           x[1] = 0;
           x[2] = 1;
           x[3] = 1;
           
        break;
        
        case 6:
           x[1] = 1;
           x[2] = 1;
           x[3] = 0;
           
        break;
        
        case 7:
           x[1] = 1;
           x[2] = 0;
           x[3] = 1;
          
        break;
        
        case 8:
           x[1] = 1;
           x[2] = 1;
           x[3] = 1;
           
        break;
    }
 ```
 
O mesmo vale para o resultado, como os resultados possíveis são apenas 2 ( **é um ser vivo ou nao**), podemos representar com:

- 1 bit -> 2^1 

  - 1 (verdadeiro) e 0 (falso)


## __*Arquitetura Perceptron Simples*__

> ![arquitetura de uma perceptron](https://github.com/Samuel-Ricardo/IA-Perceptron-java/blob/master/Readme/Arquitetura_Perceptron.jpeg)

- __*Essa imagem é uma demonstração visual de como a RNA (Rede Neural) trabalha.*__


- **X** = Dados de entrada -> bit (1 / 0)
  - [tipo int, pois só são aceitos os valores 1 e 0]

- **W** = Pesos Sinápticos que serão usados nas operações matemáticas para obter o resultado
  -  [Tipo float, pois o peso pode ter qualquer valor]

- **Bias** = Um termo constante que não depende de qualquer valor de entrada. 
  - [tipo int, pois só são aceitos os valores 1 e 0]

- **Wb** = Peso do Bias
  - [Tipo float, pois o peso pode ter qualquer valor]

- **U** = Resultado da Função Combinadora / Somadora
  -  [Tipo float, pois o pode ter qualquer valor]
  
- **g(u)** = Função de Transferência (Função Degrau) que resume o resultado em 1 ou 0 

- **Y** = resultado final (1 ou 0)
  - [tipo int, pois só são aceitos os valores 1 e 0]
  
- **N** =   Taxa de Aprendizado, é uma constante e seu valor é aleatório, mas para este código foi escolhido o valor 1.

> ![Componentes do Perceptron](https://github.com/Samuel-Ricardo/IA-Perceptron-java/blob/master/Readme/Componemtes_Perceptron.jpeg)




## __*Dados de Entrada*__

Para os dados de entrada (**X**) será necessário um vetor com o tamanho **equivalente a quantidade de bits**, que nesse caso são **3 bits por palavra**, então precisamos de um vetor com **3 posições.**

```java
int[] x = new int [4];


```



> ![treinamento 01](https://github.com/Samuel-Ricardo/IA-Perceptron-java/blob/master/Readme/Treinamento_01.jpeg)

- __*Modelo de Um neurônio*__



## __*Pesos Sinápticos*__

Para os pesos (**W**) será necessário um vetor com o **tamanho equivalente aos dados de entrada (X)**, ou seja, **para cada bit (posição) do vetor X será necessário um peso (posição) do vetor W**, neste caso como  vetor X tem 3 posições, o vetor W terá **3 posições**.

```Java
float [] w =  new float [4];
```

Um detalhe a se destacar, é que o peso **inicia com um valor aleatório**, neste caso foi decidido que todos os pesos iniciariam com o **valor 0** e o mesmo vale para o **peso do bias**, como mostrado na imagem acima e neste trecho de código onde “c” é o contador :

```java
	for (int c = 1; c == 3; c++){
            w[c]= 0;
        }
```



> ![Treinamento 02](https://github.com/Samuel-Ricardo/IA-Perceptron-java/blob/master/Readme/Treinamento_02.jpeg)

- __*Foi Selecionado o primeiro exemplo (000) e o modelo foi preenchido*__


## __*Função Combinadora / Somadora*__

O primeiro cálculo será feito utilizando a **Função Combinadora / Somadora**, que realiza uma soma ponderada entre o produto de cada entrada e seu peso sináptico **equivalente** e somaremos com o produto entre o bias e seu peso sináptico:

#

 - produto de cada entrada e seu peso sináptico
   - X[1] * W[1]

#

- soma ponderada 
   - ( X[1] * W[1]  +  X[2] * W[2] ...)

#

- somaremos com o produto entre o bias e seu peso sináptico.
  -  + ( Bias * WBias)

#

- como resultado temos:

  -  **U** = (**X**[**i**] * **W**[**i**]) + **Bias** * **Wb**

#

- Como é representado no código:

```java
  u = ( x[1] * w[1] + x[2] * w[2] + x[3] * w[3] ) + b * wB;
```

#

> ![Treinamento 03](https://github.com/Samuel-Ricardo/IA-Perceptron-java/blob/master/Readme/Treinamento_03.jpeg)

- __*Após os dados serem preenchidos, agora eles começam a ser processados passando pela **Função Combinadora / Somadora***__




## __*Função de Transferência (Função Degrau)*__

Para obtermos o resultado final (1 ou 0) utilizaremos uma **Função de Transferência**, existem várias, porém será usada a **Função Degrau**, que basicamente funciona assim:

#

 Se o “U” (resultado) for **MENOR** que 0 o resultado final (**Y**) será **0**
	-> se **U** < **0** então **Y** será = **0**

 Já se o “U” (resultado) for **IGUAL OU MAIOR** que 0 o resultado final (**Y**) será **1**
	-> se **U** >= **0** então **Y** será = **1**
#

Como é representado neste trecho do código:


```java
  if (u<0){            

            y = 0;
            
        }else{
        
            y = 1;
            
   }
```


> ![Treinamento 04](https://github.com/Samuel-Ricardo/IA-Perceptron-java/blob/master/Readme/Treinamento_04.jpeg)

- __*Função de Transferência sendo aplicada.*__



## __*Algoritmo de Aprendizado (Correção de Erro)*__

O método de aprendizagem trabalhado, é o método de **Aprendizagem Supervisionada**, onde nos é dado um conjunto de dados rotulados que já sabemos qual é a nossa saída correta e que deve ser semelhante ao conjunto, tendo a ideia de que existe uma relação entre a entrada e a saída (Fonte: [Opensanca](https://medium.com/opensanca/aprendizagem-de-maquina-supervisionada-ou-n%C3%A3o-supervisionada-7d01f78cd80a) ([Pedro Barros](https://pedro-barros.medium.com/?source=post_page-----7d01f78cd80a--------------------------------)))

Sendo assim o cálculo do  erro será feito da seguinte forma:


## __*Cálculo do Erro*__

A função deste cálculo é **verificar se a rede neural acertou ou não.** 

O cálculo do Erro (**Et**) será dado pela diferença entre o resultado correto (**Yc**) e o resultado da Rede Neural (**Y**):

   - **Et** = **Yc** - **Y**

Como mostra o trecho do código:


```java
	 er = e - y;
```


se **Et** for igual a **0** significa que a rede neural **acertou**, porém o algoritmo de aprendizagem ainda **deve ser executado**, pois se tudo estiver correto o algoritmo irá manter o mesmo valor para os pesos..




> ![Treinamento 05](https://github.com/Samuel-Ricardo/IA-Perceptron-java/blob/master/Readme/Treinamento_05.jpeg)

- __*Aplicando o cálculo de erro, para verificar se a rede neural acertou*__




> ![Treinamento 06](https://github.com/Samuel-Ricardo/IA-Perceptron-java/blob/master/Readme/Treinamento_06.jpeg)

- __*Neste caso a Rede Neural errou*__




## __*Algoritmo de Aprendizado(Regra Delta)*__
	
A função deste cálculo é **reajustar os pesos sinápticos de acordo com cálculo do Erro (Et)**, para isso existem vários algoritmos, mas, para este código foi usado a **Regra delta**, o mesmo vale para o peso do Bias:

-  **W**[**i**] = **W**[**i**] + **N** * **Et** * **X**[**i*]


Onde **“N”**  é a taxa de Aprendizado.


Veja o Exemplo a seguir:

-  **W**[**1**] = **W** [**1**] + **1** * **Et** * **X**[**1**]


Nó código está escrito desta forma:

```java
	for (int c = 1; c == 3; c++){      
                w[c] = w[c]+n*er*x[c];
                System.out.println(w[c]);
            }
        
        wB = wB+n*er*b;
```




> ![](https://github.com/Samuel-Ricardo/IA-Perceptron-java/blob/master/Readme/Treinamento_07.jpeg)

- __*Reajustando o primeiro Peso Sináptico*__


> ![](https://github.com/Samuel-Ricardo/IA-Perceptron-java/blob/master/Readme/Treinamento_08.jpeg)

- __*Reajustando o Segundo Peso Sináptico*__


> ![](https://github.com/Samuel-Ricardo/IA-Perceptron-java/blob/master/Readme/Treinamento_09.jpeg)

- __*Reajustando o terceiroPeso Sináptico*__


> ![](https://github.com/Samuel-Ricardo/IA-Perceptron-java/blob/master/Readme/Treinamento_10.jpeg)

- __*Reajustando o Peso Sináptico do Bias*__



> ![](https://github.com/Samuel-Ricardo/IA-Perceptron-java/blob/master/Readme/Treinamento_11.jpeg)

- __*Reajustando o Peso Sináptico do Bias*__



##

- Agora é só repetir o algoritmo até que a Rede Neural consiga acertar



