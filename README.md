# Criando-seu-Primeiro-Reposit-rio-no-GitHub-Para-Compartilhar-Seu-Progresso
Desafio
Faça um programa que peça para 3 pessoas a sua idade, ao final o programa deverá verificar se a média de idade da turma varia entre 0 e 25, 26 e 60 e maior que 60; e então, dizer se a turma é jovem, adulta ou idosa, conforme a média calculada.

Entrada
A entrada consiste em três números inteiros que representam a idade das pessoas.

Saída
A saída imprimirá a média de idade da turma, conforme o exemplo abaixo:

Entrada	Saída
70  Idosa!   7     Jovem!
60  Idosa!   14    Jovem!
61	Idosa!   22    Jovem!

// IMPORTANTE: Para ler os dados de entrada do usuário, utilize a classe Scanner, 
// instanciando seu leitor da seguinte forma: "Scanner leitor = new Scanner(System.in);". 
// Por outro lado, para imprimir suas saídas, utilize System.out.print ou System.out.println.  

import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner leitor = new Scanner(System.in);

        int idade1 = leitor.nextInt();
        int idade2 = leitor.nextInt();
        int idade3 = leitor.nextInt();
        int media = (idade1 + idade2 + idade3)/3;

 //TODO: Implemente um condição de verifique a média de idade da turma conforme a descrição do desafio:
  if( media >= 0 && media <= 25){
          System.out.println("Jovem!");
       } else if (media >= 26 && media <= 60){
          System.out.println("Adulta!");
        } else {
          System.out.println("Idosa!") ;
         }
       
    }
}


//////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////



Desafio
Faça um Programa que pergunte em que turno você estuda. Peça para digitar M-matutino ou V-Vespertino ou N- Noturno. Imprima a mensagem "Bom Dia!", "Boa Tarde!" ou "Boa Noite!" ou "Valor Inválido!", conforme o caso.

Entrada
A entrada consiste em um caractere(char) M , N ou V que informará o turno em que você estuda.

Saída
A saída mostrará uma mensagem que informa conforme o seu turno. Veja o exemplo:

Entrada	Saída
M	Bom Dia!
N	Boa Noite!
T	Valor Inválido!

// IMPORTANTE: Para ler os dados de entrada do usuário, utilize a classe Scanner, 
// instanciando seu leitor da seguinte forma: "Scanner leitor = new Scanner(System.in);". 
// Por outro lado, para imprimir suas saídas, utilize System.out.print ou System.out.println.

import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner leitor = new Scanner(System.in);

        char turno = leitor.next().toUpperCase().charAt(0);

//TODO: Implemente uma solução para que seja impresso a saída correto do seu turno:      

    switch (turno){

     case 'M': {System.out.println("Bom Dia!"); break;}

     case 'V': {System.out.println("Boa Tarde!"); break;}

     case 'N': {System.out.println("Boa Noite!"); break;}

     default : {System.out.println("Valor Inválido!"); break;}

    }

   }

  }


///////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////



Desafio
Elabore um programa que simule uma fila de atendimento bancário. O programa deve ler o nome de 3 pessoas (clientes do banco), armazenando-os em uma fila.

Entrada
A entrada será o nome de três pessoas (clientes do banco).

Saída
O programa deve imprimir como saída na tela o nome da pessoa e sua posição na fila.

Entrada	Saída
Ana       Ana - esta na posicao: 1

Sofia    Sofia - esta na posicao: 2

Lucas    Lucas - esta na posicao: 3



// IMPORTANTE: Para ler os dados de entrada do usuário, utilize a classe Scanner, 
// instanciando seu leitor da seguinte forma: "Scanner leitor = new Scanner(System.in);". 
// Por outro lado, para imprimir suas saídas, utilize System.out.print ou System.out.println.

import java.util.Scanner; 
 
public class Main { 
 
    public static void main(String[] args) { 
 
    String[] nomesFila = new String[3]; 
    Scanner nome = new Scanner(System.in); 

 //TODO: Implemente uma condição que simule uma fila bancaria, gerando o nome a posição do cliente na fila:
 
  for (int i = 0; i < nomesFila.length; i++) {

    nomesFila[i] = nome.next();

     

    System.out.format("%s - esta na posicao: %d%n", nomesFila[i], (i + 1));

  }

  

 } 

}
  
   
  //////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////
  
  
  
  
  
  
  Desafio
O gerente de uma loja resolveu aplicar descontos em todos os seus produtos! A tarefa é calcular a Porcentagem de Desconto aplicada a esses produtos. 

Entrada
A entrada deverá ser feita por dois valores M e D, onde a primeira linha deverá receber o valor marcado do produto, e na segunda linha o valor do produto com o desconto já aplicado.

Saída
A saída deverá retornar o percentual de desconto que foi aplicado no produto, conforme exemplo abaixo.

Exemplo 1

Entrada	Saída
40
30	O desconto foi de 25%
 

Exemplo 2

Entrada	Saída
500
195	O desconto foi de 61%
 

Exemplo 2

Entrada	Saída
100
50	O desconto foi de 50%



// IMPORTANTE: Para ler os dados de entrada do usuário, utilize a classe Scanner, 
// instanciando seu leitor da seguinte forma: "Scanner leitor = new Scanner(System.in);". 
// Por outro lado, para imprimir suas saídas, utilize System.out.print ou System.out.println.  

import java.util.*;
 
public class Main{

public static void main(String args[]) {
    Scanner input = new Scanner(System.in);
		
   
double M = input.nextDouble();
double D = input.nextDouble();
double desconto = ((M - D) / M) * 100;
    
    //TODO:  Retorne o percentual de desconto que foi aplicado no produto

System.out.println("O desconto foi de " + String.format("%.0f", desconto)+ "%");

}

  

}


///////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////



Descrição
Dado um inteiro positivo n , retorne o menor inteiro positivo que é um múltiplo 2 de e n .

Entrada
A entrada consiste em um int, do qual podemos calcular seu menor multiplo.

Saída
A entrada consiste em um retorno, que será o menor multiplo digitado e 2.

Exemplo 1

Entrada	Saída
5	
O resultado eh:10




// IMPORTANTE: Para ler os dados de entrada do usuário, utilize a classe Scanner,
// instanciando seu leitor da seguinte forma: "Scanner leitor = new Scanner(System.in);".
// Por outro lado, para imprimir suas saídas, utilize System.out.print ou System.out.println.

import java.util.Scanner;

public class Main {
  public static void main(String[] args) {
    Scanner scanner = new Scanner(System.in);
    int numero = scanner.nextInt();

//TODO: Crie as outras condições necessárias para a resolução do desafio.
    int minimoMultiplo = 0;
    if (numero % 2 == 0) {
      minimoMultiplo = numero;
    } else {
      minimoMultiplo = numero * 2;
    }

    System.out.println("O resultado eh:" + minimoMultiplo);
  }

}
