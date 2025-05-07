# 🧠 Lógica de Programação com JAVA

A lógica de programação é a base para o desenvolvimento de qualquer software. Ela envolve a criação de soluções para problemas utilizando uma sequência lógica de passos. Abaixo, exploraremos os principais conceitos de lógica de programação utilizando a linguagem Java.

---
## 📋 Menu
- [Retornar para Home](homepage.md)
- [Introdução ao Java](#1-introdução-ao-java)
- [Variáveis e Tipos de Dados](#2-variáveis-e-tipos-de-dados)
- [Estruturas Condicionais](#3-estruturas-condicionais)
- [Estruturas de Repetição](#4-estruturas-de-repetição)
- [Arrays](#5-arrays)
- [Funções (Métodos)](#6-funções-métodos)
- [Entrada e Saída de Dados](#7-entrada-e-saída-de-dados)
- [Operadores](#8-operadores)
- [Boas Práticas](#9-boas-práticas)
- [String - O que é?](#10-string---o-que-é)


## 1. Introdução ao Java
Java é uma linguagem de programação amplamente utilizada, conhecida por sua portabilidade e robustez. Antes de começar, certifique-se de ter o Java Development Kit (JDK) instalado em sua máquina. Caso precise de ajuda com a instalação, consulte o guia de instalação das IDEs [aqui](tutorial_instalacao_ides.md).

### Estrutura Básica de um Programa em Java
```java
public class Main {
    public static void main(String[] args) {
        System.out.println("Olá, Mundo!");
    }
}
```
- **`public class Main`**: Define a classe principal do programa.
- **`public static void main(String[] args)`**: Método principal onde a execução do programa começa.
- **`System.out.println`**: Imprime uma mensagem no console.

---

## 2. Variáveis e Tipos de Dados
As variáveis são usadas para armazenar dados. Em Java, é necessário declarar o tipo da variável.

### Tipos de Dados Comuns
- **int**: Números inteiros.
- **double**: Números decimais.
- **char**: Um único caractere.
- **boolean**: Valores lógicos (`true` ou `false`).
- **String**: Cadeia de caracteres.

### Exemplo
```java
int idade = 25;
double altura = 1.75;
char inicial = 'J';
boolean estudante = true;
String nome = "João";
```

---

## 3. Estruturas Condicionais
Permitem que o programa tome decisões com base em condições.

### `if`, `else if` e `else`
```java
int idade = 18;

if (idade >= 18) {
    System.out.println("Você é maior de idade.");
} else {
    System.out.println("Você é menor de idade.");
}
```

### `switch`
```java
int dia = 3;

switch (dia) {
    case 1:
        System.out.println("Domingo");
        break;
    case 2:
        System.out.println("Segunda-feira");
        break;
    default:
        System.out.println("Outro dia");
}
```

---

## 4. Estruturas de Repetição
Permitem executar um bloco de código várias vezes.

### `for`
```java
for (int i = 0; i < 5; i++) {
    System.out.println("Contagem: " + i);
}
```

### `while`
```java
int i = 0;
while (i < 5) {
    System.out.println("Contagem: " + i);
    i++;
}
```

### `do-while`
```java
int i = 0;
do {
    System.out.println("Contagem: " + i);
    i++;
} while (i < 5);
```

---

## 5. Arrays
Arrays são usados para armazenar múltiplos valores em uma única variável.

### Exemplo
```java
int[] numeros = {1, 2, 3, 4, 5};

for (int numero : numeros) {
    System.out.println(numero);
}
```

---

## 6. Funções (Métodos)
Métodos são blocos de código que executam uma tarefa específica.

### Exemplo
```java
public static int soma(int a, int b) {
    return a + b;
}

public static void main(String[] args) {
    int resultado = soma(5, 3);
    System.out.println("Resultado: " + resultado);
}
```

---

## 7. Entrada e Saída de Dados
### Entrada de Dados com `Scanner`
```java
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        System.out.print("Digite seu nome: ");
        String nome = scanner.nextLine();

        System.out.println("Olá, " + nome + "!");
    }
}
```

---

## 8. Operadores
### Operadores Aritméticos
- Soma: `+`
- Subtração: `-`
- Multiplicação: `*`
- Divisão: `/`
- Módulo (resto da divisão): `%`

### Operadores Relacionais
- Igual a: `==`
- Diferente de: `!=`
- Maior que: `>`
- Menor que: `<`
- Maior ou igual a: `>=`
- Menor ou igual a: `<=`

### Operadores Lógicos
- E: `&&`
- Ou: `||`
- Não: `!`

---

## 9. Boas Práticas
- Use nomes de variáveis descritivos.
- Indente o código corretamente.
- Comente trechos importantes do código.
- Evite duplicação de código.

---

Este guia cobre os fundamentos da lógica de programação em Java. Compreender esses conceitos é essencial antes de avançar para tópicos mais avançados, como orientação a objetos.

## 10. String - O que é?
String é uma classe em Java que representa uma sequência de caracteres. Strings são imutáveis, o que significa que, uma vez criadas, não podem ser alteradas. Você pode criar strings usando aspas duplas.

```	java
    String nome = "João";
```

- **Métodos Comuns**:
    - `length()`: Retorna o comprimento da string.
    - `charAt(int index)`: Retorna o caractere na posição especificada.
    - `substring(int beginIndex, int endIndex)`: Retorna uma parte da string.
    - `toUpperCase()`: Converte a string para maiúsculas.
    - `toLowerCase()`: Converte a string para minúsculas.
    - `indexOf(String str)`: Retorna a posição da primeira ocorrência de uma substring.
    - `replace(String oldChar, String newChar)`: Substitui uma parte da string por outra.   
    - `trim()`: Remove espaços em branco do início e do fim da string.
    - `split(String regex)`: Divide a string em partes com base em um delimitador.
    - `equals(Object obj)`: Compara duas strings para verificar se são iguais.
    - `contains(CharSequence sequence)`: Verifica se a string contém uma sequência específica.
    - `isEmpty()`: Verifica se a string está vazia.
    - `startsWith(String prefix)`: Verifica se a string começa com um prefixo específico.
    - `endsWith(String suffix)`: Verifica se a string termina com um sufixo específico. 
    - `valueOf(int i)`: Converte um inteiro em uma string.
    - `compareTo(String anotherString)`: Compara duas strings lexicograficamente.
    - `concat(String str)`: Concatena duas strings.
    - `toCharArray()`: Converte a string em um array de caracteres.
    - `StringBuilder`: Para manipulação eficiente de strings mutáveis.
    - `StringBuffer`: Semelhante ao StringBuilder, mas é sincronizado e seguro para uso em múltiplas threads.
    - `String.format(String format, Object... args)`: Formata uma string com base em um formato especificado.

- **Exemplo de Uso**:
```java
String nome = "João";   

String saudacao = "Olá, " + nome + "!"; // Concatenação

System.out.println(saudacao); // Saída: Olá, João!
System.out.println("Comprimento: " + nome.length()); // Saída: Comprimento: 4

System.out.println("Primeiro caractere: " + nome.charAt(0)); // Saída: Primeiro caractere: J

System.out.println("Substring: " + nome.substring(1, 3)); // Saída: Substring: oã

System.out.println("Maiúsculas: " + nome.toUpperCase()); // Saída: Maiúsculas: JOÃO

System.out.println("Minúsculas: " + nome.toLowerCase()); // Saída: Minúsculas: joão
```

---

- [Voltar ao Menu](#menu)
- [Entenda mais sobre System.out.println ou print ou printf](utilizando_saida_dedados.md)