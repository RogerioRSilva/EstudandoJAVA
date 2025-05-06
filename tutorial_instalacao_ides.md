# Tutorial de Instalação de IDEs

[Retornar para a homepage](homepage.md)

Este tutorial irá guiá-lo na instalação das seguintes IDEs: **VS Code**, **IntelliJ IDEA**, **Eclipse** e **NetBeans**. Clique no nome da IDE para ir diretamente à seção correspondente.

## Índice
1. [Visual Studio Code (VS Code)](#visual-studio-code-vs-code)
2. [IntelliJ IDEA](#intellij-idea)
3. [Eclipse](#eclipse)
4. [NetBeans](#netbeans)

---

## Instalação da JDK (Java Development Kit)

### Passo 1: Download
- Acesse o site oficial da Oracle: [https://www.oracle.com/java/technologies/javase-downloads.html](https://www.oracle.com/java/technologies/javase-downloads.html).
- Escolha a versão mais recente do JDK compatível com o seu sistema operacional e faça o download.

### Passo 2: Instalação
- Execute o instalador baixado.
- Siga as instruções na tela para concluir a instalação.
- Durante a instalação, anote o diretório onde o JDK será instalado (exemplo: `C:\Program Files\Java\jdk-XX`).

### Passo 3: Configuração de Variáveis de Ambiente
1. Abra as configurações do sistema e acesse as variáveis de ambiente.
2. Adicione uma nova variável de sistema chamada `JAVA_HOME` apontando para o diretório de instalação do JDK.
3. Edite a variável `Path` e adicione o caminho para o diretório `bin` do JDK (exemplo: `C:\Program Files\Java\jdk-XX\bin`).

### Passo 4: Verificação
- Abra o terminal ou prompt de comando e execute o comando `java -version`.
- Certifique-se de que a versão instalada do JDK é exibida corretamente.

---

## Visual Studio Code (VS Code)

### Passo 1: Download
- Acesse o site oficial: [https://code.visualstudio.com/](https://code.visualstudio.com/).
- Clique no botão de download para o seu sistema operacional.

### Passo 2: Instalação
- Execute o instalador baixado.
- Siga as instruções na tela, marcando as opções desejadas (como adicionar ao PATH).

### Passo 3: Configuração Inicial
- Abra o VS Code e instale extensões úteis, como:
    - **Java Extension Pack** (para desenvolvimento em Java).

---

## IntelliJ IDEA

### Passo 1: Download
- Acesse o site oficial: [https://www.jetbrains.com/idea/](https://www.jetbrains.com/idea/).
- Escolha entre as versões **Community** (gratuita) ou **Ultimate** (paga) e faça o download.

### Passo 2: Instalação
- Execute o instalador e siga as instruções.
- Configure o IntelliJ para o desenvolvimento em Java durante o primeiro uso.

### Passo 3: Configuração Inicial
- Instale plugins adicionais, se necessário, como suporte para frameworks específicos.

---

## Eclipse

### Passo 1: Download
- Acesse o site oficial: [https://www.eclipse.org/downloads/](https://www.eclipse.org/downloads/).
- Baixe o instalador para a versão **Eclipse IDE for Java Developers**.

### Passo 2: Instalação
- Execute o instalador e selecione o pacote desejado.
- Siga as instruções para concluir a instalação.

### Passo 3: Configuração Inicial
- Configure o workspace e importe projetos existentes, se necessário.

---

## NetBeans

### Passo 1: Download
- Acesse o site oficial: [https://netbeans.apache.org/](https://netbeans.apache.org/).
- Baixe a versão mais recente para o seu sistema operacional.

### Passo 2: Instalação
- Execute o instalador e siga as instruções.
- Certifique-se de que o JDK está instalado antes de iniciar o NetBeans.

### Passo 3: Configuração Inicial
- Configure o ambiente para o desenvolvimento em Java e instale plugins adicionais, se necessário.

---

## Conclusão
Agora você está pronto para usar a IDE de sua escolha para desenvolver seus projetos em Java. Caso tenha dúvidas, consulte a documentação oficial de cada ferramenta.