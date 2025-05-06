# Exercícios de Lógica de Programação em Java

[Voltar para a Página Inicial](homepage.md)

## Menu de Etapas

Escolha uma das etapas abaixo para explorar os exercícios:

1. [Etapa 1: Estruturas Sequenciais](#etapa-1-estruturas-sequenciais)
2. [Etapa 2: Estruturas Condicionais](#etapa-2-estruturas-condicionais)
3. [Etapa 3: Estruturas de Repetição](#etapa-3-estruturas-de-repetição)
4. [Etapa 4: Estruturas de Repetição com `do-while`](#etapa-4-estruturas-de-repetição-com-do-while)
5. [Etapa 5: Estruturas de Repetição com `for-each`](#etapa-5-estruturas-de-repetição-com-for-each)
6. [Etapa 6: Exercícios com Listas](#etapa-6-exercícios-com-listas)
7. [Etapa 7: Exercícios com Métodos](#etapa-7-exercícios-com-métodos)

## Etapa 1: Estruturas Sequenciais
1. **Soma de Dois Números**  
    Escreva um programa que leia dois números inteiros e exiba a soma deles.  
    **Exemplo de Código:**
    ```java
    import java.util.Scanner;

    public class Soma {
         public static void main(String[] args) {
              Scanner scanner = new Scanner(System.in);
              System.out.print("Digite o primeiro número: ");
              int num1 = scanner.nextInt();
              System.out.print("Digite o segundo número: ");
              int num2 = scanner.nextInt();
              int soma = num1 + num2;
              System.out.println("A soma é: " + soma);
         }
    }
    ```
    **Saída Esperada:**
    ```
    Digite o primeiro número: 5
    Digite o segundo número: 3
    A soma é: 8
    ```

2. **Cálculo de Área de um Retângulo**  
    Leia a largura e altura de um retângulo e calcule sua área.  
    **Exemplo de Código:**
    ```java
    import java.util.Scanner;

    public class AreaRetangulo {
         public static void main(String[] args) {
              Scanner scanner = new Scanner(System.in);
              System.out.print("Digite a largura: ");
              double largura = scanner.nextDouble();
              System.out.print("Digite a altura: ");
              double altura = scanner.nextDouble();
              double area = largura * altura;
              System.out.println("A área do retângulo é: " + area);
         }
    }
    ```
    **Saída Esperada:**
    ```
    Digite a largura: 4
    Digite a altura: 5
    A área do retângulo é: 20.0
    ```

3. **Conversão de Temperatura**  
    Converta uma temperatura de Celsius para Fahrenheit.  
    Fórmula: `F = C * 9/5 + 32`.  
    **Exemplo de Código:**
    ```java
    import java.util.Scanner;

    public class ConversaoTemperatura {
         public static void main(String[] args) {
              Scanner scanner = new Scanner(System.in);
              System.out.print("Digite a temperatura em Celsius: ");
              double celsius = scanner.nextDouble();
              double fahrenheit = celsius * 9 / 5 + 32;
              System.out.println("A temperatura em Fahrenheit é: " + fahrenheit);
         }
    }
    ```
    **Saída Esperada:**
    ```
    Digite a temperatura em Celsius: 25
    A temperatura em Fahrenheit é: 77.0
    ```

4. **Cálculo de Média Aritmética**  
    Leia três números e calcule a média aritmética deles.  
    **Exemplo de Código:**
    ```java
    import java.util.Scanner;

    public class MediaAritmetica {
         public static void main(String[] args) {
              Scanner scanner = new Scanner(System.in);
              System.out.print("Digite o primeiro número: ");
              double num1 = scanner.nextDouble();
              System.out.print("Digite o segundo número: ");
              double num2 = scanner.nextDouble();
              System.out.print("Digite o terceiro número: ");
              double num3 = scanner.nextDouble();
              double media = (num1 + num2 + num3) / 3;
              System.out.println("A média é: " + media);
         }
    }
    ```
    **Saída Esperada:**
    ```
    Digite o primeiro número: 4
    Digite o segundo número: 6
    Digite o terceiro número: 8
    A média é: 6.0
    ```

5. **Cálculo de IMC**  
    Leia o peso e a altura de uma pessoa e calcule o Índice de Massa Corporal (IMC).  
    Fórmula: `IMC = peso / (altura * altura)`.  
    **Exemplo de Código:**
    ```java
    import java.util.Scanner;

    public class CalculoIMC {
         public static void main(String[] args) {
              Scanner scanner = new Scanner(System.in);
              System.out.print("Digite o peso (kg): ");
              double peso = scanner.nextDouble();
              System.out.print("Digite a altura (m): ");
              double altura = scanner.nextDouble();
              double imc = peso / (altura * altura);
              System.out.println("O IMC é: " + imc);
         }
    }
    ```
    **Saída Esperada:**
    ```
    Digite o peso (kg): 70
    Digite a altura (m): 1.75
    O IMC é: 22.857142857142858
    ```

## Etapa 2: Estruturas Condicionais
1. **Número Par ou Ímpar**  
    Escreva um programa que leia um número inteiro e determine se ele é par ou ímpar.  
    **Exemplo de Código:**
    ```java
    import java.util.Scanner;

    public class ParOuImpar {
         public static void main(String[] args) {
              Scanner scanner = new Scanner(System.in);
              System.out.print("Digite um número: ");
              int numero = scanner.nextInt();
              if (numero % 2 == 0) {
                    System.out.println("O número é par.");
              } else {
                    System.out.println("O número é ímpar.");
              }
         }
    }
    ```
    **Saída Esperada:**
    ```
    Digite um número: 7
    O número é ímpar.
    ```

2. **Maior de Dois Números**  
    Leia dois números e exiba o maior deles.  
    **Exemplo de Código:**
    ```java
    import java.util.Scanner;

    public class MaiorNumero {
         public static void main(String[] args) {
              Scanner scanner = new Scanner(System.in);
              System.out.print("Digite o primeiro número: ");
              int num1 = scanner.nextInt();
              System.out.print("Digite o segundo número: ");
              int num2 = scanner.nextInt();
              if (num1 > num2) {
                    System.out.println("O maior número é: " + num1);
              } else {
                    System.out.println("O maior número é: " + num2);
              }
         }
    }
    ```
    **Saída Esperada:**
    ```
    Digite o primeiro número: 10
    Digite o segundo número: 20
    O maior número é: 20
    ```
3. **Classificação de Idade**  
    Escreva um programa que leia a idade de uma pessoa e determine se ela é criança (0-12 anos), adolescente (13-17 anos), adulta (18-64 anos) ou idosa (65 anos ou mais).  
    **Exemplo de Código:**
    ```java
    import java.util.Scanner;

    public class ClassificacaoIdade {
            public static void main(String[] args) {
                Scanner scanner = new Scanner(System.in);
                System.out.print("Digite a idade: ");
                int idade = scanner.nextInt();
                if (idade >= 0 && idade <= 12) {
                    System.out.println("Criança");
                } else if (idade >= 13 && idade <= 17) {
                    System.out.println("Adolescente");
                } else if (idade >= 18 && idade <= 64) {
                    System.out.println("Adulto");
                } else if (idade >= 65) {
                    System.out.println("Idoso");
                } else {
                    System.out.println("Idade inválida.");
                }
            }
    }
    ```
    **Saída Esperada:**
    ```
    Digite a idade: 30
    Adulto
    ```

4. **Verificação de Nota**  
    Leia uma nota de 0 a 10 e exiba se ela é válida ou inválida.  
    **Exemplo de Código:**
    ```java
    import java.util.Scanner;

    public class VerificacaoNota {
            public static void main(String[] args) {
                Scanner scanner = new Scanner(System.in);
                System.out.print("Digite uma nota (0 a 10): ");
                double nota = scanner.nextDouble();
                if (nota >= 0 && nota <= 10) {
                    System.out.println("Nota válida.");
                } else {
                    System.out.println("Nota inválida.");
                }
            }
    }
    ```
    **Saída Esperada:**
    ```
    Digite uma nota (0 a 10): 8.5
    Nota válida.
    ```

5. **Cálculo de Salário com Bônus**  
    Leia o salário fixo de um vendedor e o total de vendas realizadas. Se o total de vendas for maior que R$ 10.000,00, adicione um bônus de 10% ao salário. Caso contrário, adicione um bônus de 5%.  
    **Exemplo de Código:**
    ```java
    import java.util.Scanner;

    public class CalculoSalario {
            public static void main(String[] args) {
                Scanner scanner = new Scanner(System.in);
                System.out.print("Digite o salário fixo: ");
                double salarioFixo = scanner.nextDouble();
                System.out.print("Digite o total de vendas: ");
                double totalVendas = scanner.nextDouble();
                double salarioFinal;
                if (totalVendas > 10000) {
                    salarioFinal = salarioFixo + (totalVendas * 0.10);
                } else {
                    salarioFinal = salarioFixo + (totalVendas * 0.05);
                }
                System.out.println("O salário final é: " + salarioFinal);
            }
    }
    ```
    **Saída Esperada:**
    ```
    Digite o salário fixo: 2000
    Digite o total de vendas: 12000
    O salário final é: 3200.0
    ```

## Etapa 3: Estruturas de Repetição

1. **Tabuada de um Número**  
    Leia um número inteiro e exiba a tabuada dele (de 1 a 10).  
    **Exemplo de Código:**
    ```java
    import java.util.Scanner;

    public class Tabuada {
            public static void main(String[] args) {
                    Scanner scanner = new Scanner(System.in);
                    System.out.print("Digite um número: ");
                    int numero = scanner.nextInt();
                    for (int i = 1; i <= 10; i++) {
                        System.out.println(numero + " x " + i + " = " + (numero * i));
                    }
            }
    }
    ```
    **Saída Esperada:**
    ```
    Digite um número: 5
    5 x 1 = 5
    5 x 2 = 10
    ...
    5 x 10 = 50
    ```

2. **Soma de Números Positivos**  
    Leia números inteiros até que um número negativo seja digitado. Exiba a soma dos números positivos.  
    **Exemplo de Código:**
    ```java
    import java.util.Scanner;

    public class SomaPositivos {
            public static void main(String[] args) {
                    Scanner scanner = new Scanner(System.in);
                    int soma = 0;
                    while (true) {
                        System.out.print("Digite um número (negativo para sair): ");
                        int numero = scanner.nextInt();
                        if (numero < 0) {
                            break;
                        }
                        soma += numero;
                    }
                    System.out.println("A soma dos números positivos é: " + soma);
            }
    }
    ```
    **Saída Esperada:**
    ```
    Digite um número (negativo para sair): 10
    Digite um número (negativo para sair): 20
    Digite um número (negativo para sair): -5
    A soma dos números positivos é: 30
    ```

3. **Contagem Regressiva**  
    Exiba uma contagem regressiva de 10 a 0 e, ao final, exiba "FIM!".  
    **Exemplo de Código:**
    ```java
    public class ContagemRegressiva {
            public static void main(String[] args) {
                    for (int i = 10; i >= 0; i--) {
                        System.out.println(i);
                    }
                    System.out.println("FIM!");
            }
    }
    ```
    **Saída Esperada:**
    ```
    10
    9
    ...
    0
    FIM!
    ```

4. **Números Ímpares em um Intervalo**  
    Leia dois números inteiros e exiba todos os números ímpares entre eles.  
    **Exemplo de Código:**
    ```java
    import java.util.Scanner;

    public class NumerosImpares {
            public static void main(String[] args) {
                    Scanner scanner = new Scanner(System.in);
                    System.out.print("Digite o primeiro número: ");
                    int inicio = scanner.nextInt();
                    System.out.print("Digite o segundo número: ");
                    int fim = scanner.nextInt();
                    for (int i = inicio; i <= fim; i++) {
                        if (i % 2 != 0) {
                            System.out.println(i);
                        }
                    }
            }
    }
    ```
    **Saída Esperada:**
    ```
    Digite o primeiro número: 3
    Digite o segundo número: 9
    3
    5
    7
    9
    ```

5. **Fatorial de um Número**  
    Leia um número inteiro e calcule o fatorial dele.  
    **Exemplo de Código:**
    ```java
    import java.util.Scanner;

    public class Fatorial {
            public static void main(String[] args) {
                    Scanner scanner = new Scanner(System.in);
                    System.out.print("Digite um número: ");
                    int numero = scanner.nextInt();
                    int fatorial = 1;
                    for (int i = 1; i <= numero; i++) {
                        fatorial *= i;
                    }
                    System.out.println("O fatorial de " + numero + " é: " + fatorial);
            }
    }
    ```
    **Saída Esperada:**
    ```
    Digite um número: 5
    O fatorial de 5 é: 120
    ```

## Etapa 4: Estruturas de Repetição com `do-while`
1. **Soma de Números Positivos**  
    Leia números inteiros até que um número negativo seja digitado. Exiba a soma dos números positivos.  
    **Exemplo de Código:**
    ```java
    import java.util.Scanner;

    public class SomaPositivosDoWhile {
            public static void main(String[] args) {
                    Scanner scanner = new Scanner(System.in);
                    int soma = 0;
                    int numero;
                    do {
                        System.out.print("Digite um número (negativo para sair): ");
                        numero = scanner.nextInt();
                        if (numero >= 0) {
                            soma += numero;
                        }
                    } while (numero >= 0);
                    System.out.println("A soma dos números positivos é: " + soma);
            }
    }
    ```
    **Saída Esperada:**
    ```
    Digite um número (negativo para sair): 10
    Digite um número (negativo para sair): 20
    Digite um número (negativo para sair): -5
    A soma dos números positivos é: 30
    ```
2. **Contagem Regressiva**  
    Exiba uma contagem regressiva de 10 a 0 e, ao final, exiba "FIM!".  
    **Exemplo de Código:**  
    ```java
    public class ContagemRegressiva {
            public static void main(String[] args) {
                    for (int i = 10; i >= 0; i--) {
                        System.out.println(i);
                    }
                    System.out.println("FIM!");
            }
    }
    ```
    **Saída Esperada:**  
    ```
    10
    9
    8
    7
    6
    5
    4
    3
    2
    1
    0
    FIM!
    ```
3. **Números Ímpares em um Intervalo**  
    Leia dois números inteiros e exiba todos os números ímpares entre eles.  
    **Exemplo de Código:**  
    ```java
    import java.util.Scanner;

    public class NumerosImparesDoWhile {
            public static void main(String[] args) {
                    Scanner scanner = new Scanner(System.in);
                    System.out.print("Digite o primeiro número: ");
                    int inicio = scanner.nextInt();
                    System.out.print("Digite o segundo número: ");
                    int fim = scanner.nextInt();
                    int i = inicio;
                    do {
                        if (i % 2 != 0) {
                            System.out.println(i);
                        }
                        i++;
                    } while (i <= fim);
            }
    }
    ```
    **Saída Esperada:**  
    ```
    Digite o primeiro número: 3
    Digite o segundo número: 9
    3
    5
    7
    9
    ```

4. **Fatorial de um Número**  
    Leia um número inteiro e calcule o fatorial dele.  
    **Exemplo de Código:**  
    ```java
    import java.util.Scanner;

    public class FatorialDoWhile {
            public static void main(String[] args) {
                    Scanner scanner = new Scanner(System.in);
                    System.out.print("Digite um número: ");
                    int numero = scanner.nextInt();
                    int fatorial = 1;
                    int i = 1;
                    do {
                        fatorial *= i;
                        i++;
                    } while (i <= numero);
                    System.out.println("O fatorial de " + numero + " é: " + fatorial);
            }
    }
    ```
    **Saída Esperada:**  
    ```
    Digite um número: 5
    O fatorial de 5 é: 120
    ```

5. **Soma de Quadrados**  
    Leia números inteiros até que um número negativo seja digitado. Exiba a soma dos quadrados dos números positivos.  
    **Exemplo de Código:**  
    ```java
    import java.util.Scanner;

    public class SomaQuadradosDoWhile {
            public static void main(String[] args) {
                    Scanner scanner = new Scanner(System.in);
                    int soma = 0;
                    int numero;
                    do {
                        System.out.print("Digite um número (negativo para sair): ");
                        numero = scanner.nextInt();
                        if (numero >= 0) {
                            soma += numero * numero;
                        }
                    } while (numero >= 0);
                    System.out.println("A soma dos quadrados dos números positivos é: " + soma);
            }
    }
    ```
    **Saída Esperada:**  
    ```
    Digite um número (negativo para sair): 3
    Digite um número (negativo para sair): 4
    Digite um número (negativo para sair): -1
    A soma dos quadrados dos números positivos é: 25
    ```

## Etapa 5: Estruturas de Repetição com `for-each`
1. **Soma de Elementos de um Array**  
    Leia um array de números inteiros e exiba a soma de seus elementos.  
    **Exemplo de Código:**  
    ```java
    public class SomaArray {
            public static void main(String[] args) {
                int[] numeros = {1, 2, 3, 4, 5};
                int soma = 0;
                for (int numero : numeros) {
                    soma += numero;
                }
                System.out.println("A soma dos elementos do array é: " + soma);
            }
    }
    ```  
    **Saída Esperada:**  
    ```
    A soma dos elementos do array é: 15
    ```

2. **Números Pares em um Array**  
    Leia um array de números inteiros e exiba apenas os números pares.  
    **Exemplo de Código:**  
    ```java
    public class NumerosPares {
            public static void main(String[] args) {
                int[] numeros = {1, 2, 3, 4, 5, 6};
                System.out.println("Números pares:");
                for (int numero : numeros) {
                    if (numero % 2 == 0) {
                            System.out.println(numero);
                    }
                }
            }
    }
    ```  
    **Saída Esperada:**  
    ```
    Números pares:
    2
    4
    6
    ```

3. **Concatenação de Strings em um Array**  
    Leia um array de strings e exiba todas as strings concatenadas em uma única linha.  
    **Exemplo de Código:**  
    ```java
    public class ConcatenaStrings {
            public static void main(String[] args) {
                String[] palavras = {"Olá", "mundo", "Java"};
                StringBuilder resultado = new StringBuilder();
                for (String palavra : palavras) {
                    resultado.append(palavra).append(" ");
                }
                System.out.println("Resultado: " + resultado.toString().trim());
            }
    }
    ```  
    **Saída Esperada:**  
    ```
    Resultado: Olá mundo Java
    ```

4. **Maior Número em um Array**  
    Leia um array de números inteiros e determine o maior número.  
    **Exemplo de Código:**  
    ```java
    public class MaiorNumeroArray {
            public static void main(String[] args) {
                int[] numeros = {10, 20, 5, 30, 15};
                int maior = numeros[0];
                for (int numero : numeros) {
                    if (numero > maior) {
                            maior = numero;
                    }
                }
                System.out.println("O maior número é: " + maior);
            }
    }
    ```  
    **Saída Esperada:**  
    ```
    O maior número é: 30
    ```

5. **Contagem de Vogais em um Array de Caracteres**  
    Leia um array de caracteres e conte quantas vogais ele contém.  
    **Exemplo de Código:**  
    ```java
    public class ContagemVogais {
            public static void main(String[] args) {
                char[] caracteres = {'a', 'b', 'c', 'e', 'i', 'o', 'u', 'x'};
                int contadorVogais = 0;
                for (char caractere : caracteres) {
                    if ("aeiou".indexOf(caractere) != -1) {
                            contadorVogais++;
                    }
                }
                System.out.println("O número de vogais é: " + contadorVogais);
            }
    }
    ```  
    **Saída Esperada:**  
    ```
    O número de vogais é: 5
    ```
## Etapa 6: Exercícios com Listas

1. **Soma de Elementos de uma Lista**  
    Leia uma lista de números inteiros e exiba a soma de seus elementos.  
    **Exemplo de Código:**  
    ```java
    import java.util.ArrayList;
    import java.util.Scanner;

    public class SomaLista {
            public static void main(String[] args) {
                    Scanner scanner = new Scanner(System.in);
                    ArrayList<Integer> numeros = new ArrayList<>();
                    System.out.println("Digite números inteiros (digite -1 para encerrar):");
                    while (true) {
                        int numero = scanner.nextInt();
                        if (numero == -1) {
                                break;
                        }
                        numeros.add(numero);
                    }
                    int soma = 0;
                    for (int numero : numeros) {
                        soma += numero;
                    }
                    System.out.println("A soma dos elementos da lista é: " + soma);
            }
    }
    ```  
    **Saída Esperada:**  
    ```
    Digite números inteiros (digite -1 para encerrar):
    10
    20
    30
    -1
    A soma dos elementos da lista é: 60
    ```

2. **Números Pares em uma Lista**  
    Leia uma lista de números inteiros e exiba apenas os números pares.  
    **Exemplo de Código:**  
    ```java
    import java.util.ArrayList;
    import java.util.Scanner;

    public class NumerosParesLista {
            public static void main(String[] args) {
                    Scanner scanner = new Scanner(System.in);
                    ArrayList<Integer> numeros = new ArrayList<>();
                    System.out.println("Digite números inteiros (digite -1 para encerrar):");
                    while (true) {
                        int numero = scanner.nextInt();
                        if (numero == -1) {
                                break;
                        }
                        numeros.add(numero);
                    }
                    System.out.println("Números pares:");
                    for (int numero : numeros) {
                        if (numero % 2 == 0) {
                                System.out.println(numero);
                        }
                    }
            }
    }
    ```  
    **Saída Esperada:**  
    ```
    Digite números inteiros (digite -1 para encerrar):
    1
    2
    3
    4
    -1
    Números pares:
    2
    4
    ```

3. **Ordenação de uma Lista**  
    Leia uma lista de números inteiros e exiba os números em ordem crescente.  
    **Exemplo de Código:**  
    ```java
    import java.util.ArrayList;
    import java.util.Collections;
    import java.util.Scanner;

    public class OrdenacaoLista {
            public static void main(String[] args) {
                    Scanner scanner = new Scanner(System.in);
                    ArrayList<Integer> numeros = new ArrayList<>();
                    System.out.println("Digite números inteiros (digite -1 para encerrar):");
                    while (true) {
                        int numero = scanner.nextInt();
                        if (numero == -1) {
                                break;
                        }
                        numeros.add(numero);
                    }
                    Collections.sort(numeros);
                    System.out.println("Números em ordem crescente: " + numeros);
            }
    }
    ```  
    **Saída Esperada:**  
    ```
    Digite números inteiros (digite -1 para encerrar):
    5
    2
    8
    1
    -1
    Números em ordem crescente: [1, 2, 5, 8]
    ```

4. **Remoção de Elementos Duplicados**  
    Leia uma lista de números inteiros e remova os elementos duplicados.  
    **Exemplo de Código:**  
    ```java
    import java.util.ArrayList;
    import java.util.HashSet;
    import java.util.Scanner;

    public class RemoveDuplicados {
            public static void main(String[] args) {
                    Scanner scanner = new Scanner(System.in);
                    ArrayList<Integer> numeros = new ArrayList<>();
                    System.out.println("Digite números inteiros (digite -1 para encerrar):");
                    while (true) {
                        int numero = scanner.nextInt();
                        if (numero == -1) {
                                break;
                        }
                        numeros.add(numero);
                    }
                    HashSet<Integer> unicos = new HashSet<>(numeros);
                    System.out.println("Lista sem duplicados: " + unicos);
            }
    }
    ```  
    **Saída Esperada:**  
    ```
    Digite números inteiros (digite -1 para encerrar):
    1
    2
    2
    3
    -1
    Lista sem duplicados: [1, 2, 3]
    ```

5. **Média dos Elementos de uma Lista**  
    Leia uma lista de números inteiros e calcule a média dos elementos.  
    **Exemplo de Código:**  
    ```java
    import java.util.ArrayList;
    import java.util.Scanner;

    public class MediaLista {
            public static void main(String[] args) {
                    Scanner scanner = new Scanner(System.in);
                    ArrayList<Integer> numeros = new ArrayList<>();
                    System.out.println("Digite números inteiros (digite -1 para encerrar):");
                    while (true) {
                        int numero = scanner.nextInt();
                        if (numero == -1) {
                                break;
                        }
                        numeros.add(numero);
                    }
                    int soma = 0;
                    for (int numero : numeros) {
                        soma += numero;
                    }
                    double media = numeros.isEmpty() ? 0 : (double) soma / numeros.size();
                    System.out.println("A média dos elementos da lista é: " + media);
            }
    }
    ```  
    **Saída Esperada:**  
    ```
    Digite números inteiros (digite -1 para encerrar):
    10
    20
    30
    -1
    A média dos elementos da lista é: 20.0
    ```
## Etapa 7: Exercícios com Métodos

1. **Cálculo de Potência**  
    Crie um método que receba dois números inteiros, base e expoente, e retorne o resultado da base elevada ao expoente.  
    **Exemplo de Código:**  
    ```java
    public class CalculaPotencia {
        public static void main(String[] args) {
            int base = 2;
            int expoente = 3;
            System.out.println("Resultado: " + potencia(base, expoente));
        }

        public static int potencia(int base, int expoente) {
            int resultado = 1;
            for (int i = 0; i < expoente; i++) {
                resultado *= base;
            }
            return resultado;
        }
    }
    ```  
    **Saída Esperada:**  
    ```
    Resultado: 8
    ```

2. **Verificação de Número Primo**  
    Crie um método que receba um número inteiro e retorne `true` se ele for primo, ou `false` caso contrário.  
    **Exemplo de Código:**  
    ```java
    public class VerificaPrimo {
        public static void main(String[] args) {
            int numero = 7;
            System.out.println("O número " + numero + " é primo? " + ehPrimo(numero));
        }

        public static boolean ehPrimo(int numero) {
            if (numero <= 1) return false;
            for (int i = 2; i <= Math.sqrt(numero); i++) {
                if (numero % i == 0) return false;
            }
            return true;
        }
    }
    ```  
    **Saída Esperada:**  
    ```
    O número 7 é primo? true
    ```

3. **Cálculo de Fatorial com Método**  
    Crie um método que receba um número inteiro e retorne o fatorial dele.  
    **Exemplo de Código:**  
    ```java
    public class CalculaFatorial {
        public static void main(String[] args) {
            int numero = 5;
            System.out.println("O fatorial de " + numero + " é: " + fatorial(numero));
        }

        public static int fatorial(int numero) {
            int resultado = 1;
            for (int i = 1; i <= numero; i++) {
                resultado *= i;
            }
            return resultado;
        }
    }
    ```  
    **Saída Esperada:**  
    ```
    O fatorial de 5 é: 120
    ```

4. **Cálculo de Média com Método**  
    Crie um método que receba um array de números inteiros e retorne a média dos elementos.  
    **Exemplo de Código:**  
    ```java
    public class CalculaMedia {
        public static void main(String[] args) {
            int[] numeros = {10, 20, 30};
            System.out.println("A média é: " + media(numeros));
        }

        public static double media(int[] numeros) {
            int soma = 0;
            for (int numero : numeros) {
                soma += numero;
            }
            return numeros.length == 0 ? 0 : (double) soma / numeros.length;
        }
    }
    ```  
    **Saída Esperada:**  
    ```
    A média é: 20.0
    ```

5. **Inversão de String**  
    Crie um método que receba uma string e retorne a string invertida.  
    **Exemplo de Código:**  
    ```java
    public class InverteString {
        public static void main(String[] args) {
            String texto = "Java";
            System.out.println("Texto invertido: " + inverte(texto));
        }

        public static String inverte(String texto) {
            StringBuilder invertida = new StringBuilder(texto);
            return invertida.reverse().toString();
        }
    }
    ```  
    **Saída Esperada:**  
    ```
    Texto invertido: avaJ
    ```