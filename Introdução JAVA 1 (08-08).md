# Programação Orientada a Objetos com Java

## 📜Mandamentos do Furgeri📜

🗿 1º Mandamento - 'Não desrespeitarás as convenções do Java'  
🗿 2º Mandamento - 'Não usarás valores absolutos no código'  
🗿 3º Mandamento - 'Não apresentarás valores de um array sem um laço de repetição'  
🗿 4º Mandamento - 'Nomearás seus métodos com a semântica adequada'  
🗿 5º Mandamento - 'Documentarás todos os métodos'

---

## Conteúdo Original Convertido

INTRODUÇÃO A JAVA

O que é o JDK (Java Development Kit)?
R: É o kit de ferramentas mínimo para desenvolvimento de aplicações em java. As ferramentas abaixo são parte do JDK:

Compilador (javac)
Interpretador de bytecode (java)
Visualizador de applets (appletviewer)
Gerador de documentação (javadoc)

Ciclo de Desenvolvimento em Java:

O Java é uma linguagem compilada, no ciclo de desenvolvimento o arquivo em Java é primeiro compilado, após isso caso esteja tudo certo o sistema gera um arquivo "executável" que é o arquivo interpretado para o funcionamento do programa.

---

CONVENÇÕES EM JAVA

São padrões que auxiliam na identificação dos componentes e itens do desenvolvimento de uma aplicação.

Nomes de arquivos (Camel Case com letra maiúscula no início)
• Customer.java, RentalItem.java

Nomes de Classes (Camel Case com letra maiúscula no início)
• Customer, RentalItem, InventorItem [Uma classe sempre começa com letras maiúsculas]

Nomes de Pacotes (Snake Case)
• semana01, br.com.fatec.poo

Nomes de Métodos (Camel Case)
• getCustomerName(), setRentalItemPrice()

Standard para variáveis (Camel Case)
• customerName, customerCreditLimit

Standard para constantes (Upper Case)
• MIN_WIDTH, MAX_NUMBER_OF_ITEMS
---

Criando uma aplicação em java
 
1. Criar um arquivo .java com o código da aplicação.

Diferença entre uma classe e uma aplicação - uma aplicação é algo executável, uma classe é um modelo que é consumido/utilizado por uma aplicação (uma aplicação consome classes). 

- Uma classe pode ser criada, mas também existem classes fixas das próprias aplicações (comandos)

- Uma classe está dentro do arquivo, e o nome do arquivo sempre precisa ser igual ao nome da classe.

2. Usando as ferramentas da linguagem para compilar e executar o arquivo .java criado:
- Primeiro, na pasta do JDK, chamamos o javac para compilar o arquivo .java indicando seu caminho;(javac caminho_do_arquivo);
* Após isso, o javac que é o compilador do JDK vai criar um arquivo "executável"
* A JVM (Java Virtual Machine) é responsável por interpretar o arquivo .class gerado pelo compilador para que a aplicação funcione. É a maquina virtual que conversa com o sistema operacional.

- Rodar o arquivo.class com o java para executá-lo (java caminho arquivo);

CTRL+A e CTRL+I aplica a identação em todo o arquivo.

---

Package - é uma pasta onde as classes estão sendo armazenadas.

Maneiras de declarar um Array em java
String [] vetor = {"10","20"};
String [] v = new String[2];
v[0]="30";
v[1]="40";




