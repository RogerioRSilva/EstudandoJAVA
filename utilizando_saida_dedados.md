## Métodos de Saída de Dados em Java: `System.out.print`, `System.out.println` e `System.out.printf`

Em Java, os métodos `System.out.print`, `System.out.println` e `System.out.printf` são utilizados para exibir informações no console. Cada um deles possui características específicas que os tornam adequados para diferentes situações.

---

### Diferença entre `print`, `println` e `printf`

- **`print`**: Exibe o texto no console sem pular para a próxima linha.
- **`println`**: Exibe o texto no console e pula automaticamente para a próxima linha.
- **`printf`**: Exibe o texto com formatação personalizada, sem pular para a próxima linha automaticamente.

---

### Estrutura de Cada Método

#### `System.out.print`
Exibe o texto ou valor diretamente no console, sem quebra de linha.

```java
System.out.print("Olá, ");
System.out.print("mundo!");
```

**Saída:**
```
Olá, mundo!
```

---

#### `System.out.println`
Exibe o texto ou valor no console e adiciona uma quebra de linha ao final.

```java
System.out.println("Olá,");
System.out.println("mundo!");
```

**Saída:**
```
Olá,
mundo!
```

---

#### `System.out.printf`
Permite exibir textos formatados no console, utilizando marcadores para inserir valores.

```java
String nome = "João";
int idade = 25;
System.out.printf("Nome: %s, Idade: %d%n", nome, idade);
```

**Saída:**
```
Nome: João, Idade: 25
```

---

### Marcadores de Formatação no `printf`

Dentro das aspas do `printf`, utilizamos marcadores para definir como os valores serão exibidos. Aqui estão alguns exemplos:

| Marcador | Tipo de Dados       | Exemplo                                    |
|----------|---------------------|--------------------------------------------|
| `%d`     | Número inteiro      | `System.out.printf("Valor: %d", 10);`      |
| `%f`     | Número decimal      | `System.out.printf("Preço: %.2f", 9.99);`  |
| `%s`     | Texto (String)      | `System.out.printf("Nome: %s", "João");`   |
| `%c`     | Caractere único     | `System.out.printf("Letra: %c", 'A');`     |
| `%n`     | Nova linha          | `System.out.printf("Linha 1%nLinha 2");`   |

---

### Exemplos Práticos

#### 1. Exibir um nome e uma idade com `printf`

```java
String nome = "Ana";
int idade = 28;
System.out.printf("Nome: %s, Idade: %d%n", nome, idade);
```

**Saída:**
```
Nome: Ana, Idade: 28
```

---

#### 2. Exibir um número decimal com duas casas decimais

```java
double preco = 19.987;
System.out.printf("Preço: R$ %.2f%n", preco);
```

**Saída:**
```
Preço: R$ 19.99
```

---

#### 3. Ajustar largura mínima de um número com `printf`

```java
int quantidade = 7;
System.out.printf("Quantidade: %5d%n", quantidade);
```

**Saída:**
```
Quantidade:     7
```

---

#### 4. Alinhar texto à direita e à esquerda com `printf`

```java
System.out.printf("|%-10s|%10s|%n", "Esquerda", "Direita");
```

**Saída:**
```
|Esquerda  |   Direita|
```

---

### Conclusão

Os métodos `System.out.print`, `System.out.println` e `System.out.printf` são ferramentas essenciais para exibir informações no console em Java. Enquanto `print` e `println` são mais simples e diretos, o `printf` oferece maior flexibilidade e controle sobre a formatação da saída. Escolha o método mais adequado para suas necessidades e aproveite o poder da personalização na exibição de dados!

