# Programação Orientada a Objetos - Anotações

## Mandamentos do Furgeri

1º Mandamento do Furgeri - 'Não desrespeitarás as convenções do Java'  

2º Mandamento do Furgeri - 'Não usarás valores absolutos no código'  
***SEMPRE UTILIZAR UMA CONSTANTE PARA REALIZAR OPERAÇÕES COM VALORES FIXOS NO PROGRAMA.  
DECLARE UMA CONSTANTE NO INÍCIO DO PROGRAMA, E A UTILIZE ***  

3º Mandamento do Furgeri - 'Não apresentarás valores de um array sem um laço de repetição'  

---

## Introdução

Anotações da aula de **POO (Programação Orientada a Objetos)**, baseadas no conteúdo visto em aula e materiais complementares.

Fonte de apoio: [W3Schools Java](https://www.w3schools.com/java)

---

## Saída de Dados

- `println()` → método que imprime qualquer coisa no console, como inteiros, strings, etc.

### Comentários

- `//` → comentário de linha única.  
- `/* ... */` → comentário de múltiplas linhas.  
- `/** ... */` → documentação de métodos ou funções (JavaDoc).  

---

## Variáveis

- **Tipos que começam com maiúscula** → tipos criados pelo programador (classes).  
- **Tipos que começam com minúscula** → tipos primitivos (core do Java).  

### Variáveis `final`

São **constantes**, não podem ter o valor alterado depois de atribuídos. Exemplo:

```java
final int MESES_DO_ANO = 12;
```

---

## Tipos Primitivos

Servem apenas para **armazenar e recuperar valores** (gravar e ler).  
Exemplos: `byte`, `short`, `int`, `long`, `float`, `double`, `boolean`, `char`.

### Exemplo:

```java
int idade = 20;
boolean ativo = true;
```

## Tipos Não Primitivos

- Podem armazenar valores **e também comportamentos**.  
- Incluem **Strings, Arrays, Classes e Objetos**.  
- Exemplo:

```java
String nome = "Armando";
```

---

## Números em Java

- `byte` → indicado para armazenar valores pequenos (até 127). Útil para economia de memória.  
  Exemplo: idade de uma pessoa.

---

## Java Type Casting

### Conversão de tipos

- **Widening Casting (automática)** → conversão de um tipo menor para maior.  
- **Narrowing Casting (manual)** → conversão de um tipo maior para menor, precisa de cast explícito.

### Exemplo:

```java
int num = 10;
double num2 = num; // Widening (automática)

double valor = 9.78;
int valorInt = (int) valor; // Narrowing (manual)
```

---

## Operadores de Bit

Operam diretamente com os **valores binários dos números**.

### Exemplo tabela binário-decimal:

```
000 = 0
001 = 1
010 = 2
011 = 3
100 = 4
101 = 5
110 = 6
111 = 7
```

### Operações

- **E (&)**  
```java
int x = 3 & 5; // resultado = 1
```

- **OU (|)**  
```java
int y = 3 | 5; // resultado = 7
```

---

## Operador Ternário

Forma resumida do `if/else`.

```java
int a = 40;
int b = 10;

int maior = (a > b ? a : b);
```

---

## Laço *for-each* (Iterator)

Usado para percorrer coleções e arrays:

```java
for (String s : nomes) {
    System.out.println(s);
}
```

---

## Complementos Importantes

### Pilares da POO

1. **Abstração** → representar objetos do mundo real no código.  
2. **Encapsulamento** → esconder os detalhes internos de uma classe e expor apenas o necessário.  
3. **Herança** → reutilizar código através da relação "é um".  
4. **Polimorfismo** → objetos podem assumir múltiplas formas (ex: sobrecarga e sobrescrita de métodos).  

### Classes e Objetos

- **Classe** → modelo ou molde de um objeto.  
- **Objeto** → instância de uma classe.  

Exemplo:

```java
class Pessoa {
    String nome;
    int idade;

    void falar() {
        System.out.println("Olá, meu nome é " + nome);
    }
}

public class Main {
    public static void main(String[] args) {
        Pessoa p = new Pessoa();
        p.nome = "Armando";
        p.idade = 22;
        p.falar();
    }
}
```

---

## Resumo Final

- Java diferencia **tipos primitivos** e **não primitivos**.  
- Variáveis `final` → constantes.  
- Evitar valores absolutos (mandamento do Furgeri).  
- Sempre usar laços de repetição para percorrer arrays.  
- Conhecer casting, operadores de bit e operador ternário.  
- Entender os 4 pilares da POO.  
