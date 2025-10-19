# Programação Orientada a Objetos com Java

## 📜Mandamentos do Furgeri📜

🗿 1º Mandamento - 'Não desrespeitarás as convenções do Java'  
🗿 2º Mandamento - 'Não usarás valores absolutos no código'  
🗿 3º Mandamento - 'Não apresentarás valores de um array sem um laço de repetição'  
🗿 4º Mandamento - 'Nomearás seus métodos com a semântica adequada'  
🗿 5º Mandamento - 'Documentarás todos os métodos'

---

## ☕ Introdução ao Java

O **Java** é uma linguagem de programação orientada a objetos, multiplataforma e fortemente tipada, desenvolvida pela Sun Microsystems (hoje Oracle).  
Ela é amplamente utilizada em aplicações desktop, web, mobile e sistemas embarcados.

A principal filosofia do Java é o conceito de **“Write Once, Run Anywhere”** — ou seja, escreva uma vez e execute em qualquer lugar, graças à **Java Virtual Machine (JVM)**.

---

## 🔧 JDK, JRE e JVM

### **JDK (Java Development Kit)**
É o kit de desenvolvimento que contém todas as ferramentas necessárias para criar, compilar e executar programas Java.

**Principais componentes do JDK:**
- **Compilador (`javac`)** – converte o código-fonte `.java` em bytecode `.class`  
- **Interpretador (`java`)** – executa o bytecode na JVM  
- **Gerador de documentação (`javadoc`)** – cria documentação automática a partir de comentários JavaDoc  
- **Visualizador de Applets (`appletviewer`)** – usado para testar applets (obsoleto nas versões modernas)

### **JRE (Java Runtime Environment)**
É o ambiente de execução do Java, necessário apenas para rodar programas, não para desenvolvê-los.

### **JVM (Java Virtual Machine)**
É a máquina virtual responsável por interpretar o bytecode e executar o programa em qualquer sistema operacional.

---

## 🔁 Ciclo de Desenvolvimento em Java

1. **Escrever** o código-fonte (`.java`).
2. **Compilar** usando o `javac`, que gera o arquivo `.class`.
3. **Executar** o programa com o comando `java`, que roda o bytecode na JVM.

```bash
javac Programa.java
java Programa
```

Esse processo garante portabilidade e segurança, uma das principais vantagens da linguagem.

---

## ✍️ Convenções de Código em Java

As convenções servem para **padronizar e melhorar a legibilidade do código**.

| Elemento | Convenção | Exemplo |
|-----------|------------|----------|
| Arquivos e Classes | CamelCase, com letra maiúscula | `Cliente.java`, `PedidoOnline.java` |
| Métodos | camelCase, com letra minúscula | `getNome()`, `calcularTotal()` |
| Variáveis | camelCase | `valorFinal`, `nomeUsuario` |
| Constantes | MAIÚSCULAS | `MAX_VALOR`, `TAXA_DESCONTO` |
| Pacotes | minúsculo e separados por ponto | `pacote1`, `br.com.empresa.app` |

> 💡 **Dica:** Seguir as convenções evita confusão entre desenvolvedores e melhora a manutenção do código.

---

## 🧱 Estrutura Básica de uma Aplicação Java

```java
public class HelloWorld {
    public static void main(String[] args) {
        System.out.println("Olá, mundo!");
    }
}
```

- O arquivo deve ter o mesmo nome da classe principal.  
- O método `main` é o ponto de entrada da aplicação.  
- `System.out.println()` é usado para imprimir saídas no console.

---

## 📦 Packages (Pacotes)

Um **package** é o local onde as classes de um projeto são **agrupadas e organizadas**.  
Ele serve para **estruturar o código**, **evitar conflitos de nomes** e **facilitar a reutilização** de classes.  

Os pacotes podem ser **importados** em outros arquivos, permitindo o uso das classes neles contidas — de forma semelhante a **bibliotecas**.

```java
package br.com.fatec.exemploanterior; // declarando o pacote da classe atual

public class Principal {
    public static void main(String[] args) {
        Exemplo ex = new Exemplo(); // criando um objeto da classe Exemplo, que está no mesmo pacote
        ex.olaMundo(); // chamando o método da classe Exemplo
    }
}
```
E se a classe Exemplo estivesse em outro pacote, seria necessário importá-la explicitamente:

```java
package br.com.fatec.exemplonovo // declarando o pacote da classe atual (não possui a classe Exemplo)
import br.com.fatec.exemploanterior.Exemplo; // importando a classe Exemplo de outro pacote que possui a classe Exemplo

public class Principal {
    public static void main(String[] args) {
        Exemplo ex = new Exemplo();
        ex.olaMundo();
    }
}
```
Sem a importação adequada, a classe Exemplo não seria reconhecida pela aplicação,
pois cada arquivo Java só “enxerga” as classes dentro do seu próprio pacote (ou as que são importadas).

---

## 📚 Arrays em Java

Um **array** é uma estrutura que armazena vários valores do mesmo tipo.

### Declaração e uso:

```java
String[] nomes = {"Ana", "Bruno", "Carlos"}; // Declarando e já inserindo valores
int[] numeros = new int[3]; // Apenas declarando e definindo o tamanho
numeros[0] = 10;
numeros[1] = 20;
numeros[2] = 30;
```
