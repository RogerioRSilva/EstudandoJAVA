# Guia de Nomenclatura no Java

A linguagem Java segue convenções de nomenclatura bem definidas que ajudam os programadores a criar códigos mais claros e organizados. Essas convenções não são obrigatórias, mas são altamente recomendadas para manter a legibilidade e padronização do código.

## 1. Identificadores no Java

Identificadores são nomes usados para identificar classes, métodos, variáveis e outros elementos no código. Algumas regras básicas para criar identificadores:

- Devem começar com uma letra (a–z, A–Z), um símbolo de sublinhado (`_`) ou um cifrão (`$`).
- Podem conter números, mas nunca começar com eles.
- Não podem usar palavras reservadas do Java como `class`, `public`, `static`, etc.
- São sensíveis a maiúsculas e minúsculas.

---

## 2. Convenções de Nomenclatura

As convenções ajudam a distinguir diferentes elementos no código. Veja como aplicá-las:

### Classes e Interfaces
- Use a convenção **PascalCase**, em que cada palavra no nome começa com letra maiúscula.  
    **Exemplos:** `ClienteCadastro`, `GerenciadorDeProdutos`, `Runnable`.
- Escolha nomes que representem objetos ou conceitos (geralmente substantivos).

### Métodos
- Use a convenção **camelCase**, em que a primeira palavra começa com letra minúscula, e as seguintes com maiúscula.  
    **Exemplos:** `calcularTotal`, `imprimirFatura`, `verificarDisponibilidade`.
- Métodos geralmente representam ações, por isso seus nomes começam com verbos.

### Variáveis
- Também seguem a convenção **camelCase** e devem ter nomes curtos, porém descritivos.  
    **Exemplos:** `nomeUsuario`, `quantidadePedido`, `precoComDesconto`.

### Constantes
- Devem ser escritas em letras maiúsculas, com palavras separadas por sublinhado (`_`).  
    **Exemplos:** `MAX_VELOCIDADE`, `TEMPO_PADRAO`.

### Pacotes
- Os nomes dos pacotes devem estar em letras minúsculas, geralmente representando o domínio da empresa seguido pelo nome do projeto ou módulo.  
    **Exemplos:** `br.com.exemplo.meuprojeto`.

---

## 3. Boas Práticas

- Use nomes descritivos que façam sentido no contexto do código.
- Seja consistente nas convenções em todo o projeto.
- Evite abreviações, salvo aquelas universalmente conhecidas.
- Não use caracteres especiais nem espaços nos identificadores.

---

## 4. Exemplo Prático

### Código em Java:
```java
package br.com.exemplo.meuprojeto;

public class Calculadora {
        private double resultado;

        public double somarNumeros(double primeiroNumero, double segundoNumero) {
                return primeiroNumero + segundoNumero;
        }

        public void imprimirResultado() {
                System.out.println("O resultado é: " + resultado);
        }
}
```

### Explicação:
- `Calculadora` é o nome da classe, seguindo o padrão **PascalCase**.
- `somarNumeros` e `imprimirResultado` são métodos, seguindo o padrão **camelCase**.
- `resultado`, `primeiroNumero` e `segundoNumero` são variáveis, também em **camelCase**.
- O pacote `br.com.exemplo.meuprojeto` está em letras minúsculas, conforme a convenção.

---

## 5. Conclusão

Seguir as convenções de nomenclatura ajuda a criar códigos mais legíveis, organizados e fáceis de manter. Além disso, essas práticas facilitam a colaboração em equipe e a evolução dos projetos.
