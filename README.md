# 🧠 Linguagem T01 — Documentação Oficial

## 📌 Visão Geral
A linguagem **T01** foi desenvolvida para fins acadêmicos, utilizando **JavaCC**. Seu objetivo é permitir a criação de programas simples que incluam:

- Declaração de variáveis  
- Atribuições de valores  
- Entrada (`input`) e saída (`printf`) de dados  
- Estruturas condicionais (`if`, `else`)  
- Estruturas de repetição (`while`, `do-while`, `for`)  
- Estrutura de decisão (`switch-case`)  

O parser é configurado para debug, facilitando o acompanhamento da análise léxica e sintática do código.

---

## ⚙️ Tecnologias Utilizadas
- Java  
- JavaCC  

---

## 🚀 Como Executar

### 1. Pré-requisitos
- Java JDK instalado  
- JavaCC configurado no ambiente  

### 2. Executando o projeto

1. Compile o arquivo `.jj` com JavaCC:
   ```bash
   javacc T01.jj

2. Compile os arquivos Java gerados:
    bash

    javac *.java

3. Execute o parser:
    bash

    java trabalho1.T01

Arquivo de entrada:

..//JavaCC//src//trabalho1//teste07.txt
###  3. Estrutura Léxica
🔹 Tokens Principais

    Parênteses: (, )

    Chaves: {, }

    Colchetes: [, ]

    Fim de linha: ;

    Operadores de comparação: =, ==, !=, >, <, >=, <=

🔹 Tipos de Dados
Tipo	Palavra-chave
Inteiro	int
Float	float
Booleano	bool
Caractere	char
🔹 Palavras Reservadas

    Estruturas de decisão: if, else, switch, case, default

    Estruturas de repetição: while, do, for, break

    Entrada e saída: input, printf

    Booleanos: true, false

🔹 Identificadores
regex

[a-zA-Z][a-zA-Z0-9]*

🔹 Números
regex

[0-9]+

🔹 Comentários
java

// comentário de uma linha

🧱 Estruturas da Linguagem
Declaração de Variáveis
java

int x;
int y = 10;
float z = 5;
bool ativo = true;
char c = 'a';

Atribuição de Valores
java

x = 10;
c = 'a';

Entrada de Dados
java

input("Digite algo");
int(input("Digite um número"));

Saída de Dados
java

printf("Hello");
printf(x);

Estruturas de Controle
IF / ELSE
java

if (x == 10) {
    printf("Igual");
} else {
    printf("Diferente");
}

WHILE
java

while (x < 10) {
    x++;
}

DO-WHILE
java

do {
    x++;
} while (x < 10);

FOR
java

for (i = 0; i < 10; i++) {
    printf(i);
}

SWITCH / CASE
java

switch(x) {
    case(1):
        printf("Um");
        break;
    case(2):
        printf("Dois");
        break;
    default:
        printf("Outro");
        break;
}

⚠️ Regras Importantes

    Toda instrução deve terminar com ;

    Blocos devem ser delimitados por { }

    Strings usam " ", caracteres usam ' '

    Operadores válidos para comparação: ==, !=, >, <, >=, <=

📂 Estrutura do Projeto
text

trabalho1/
 ├── T01.jj        # Arquivo da gramática JavaCC
 ├── T01.java      # Parser gerado
 ├── teste07.txt   # Arquivo de entrada de teste

🐞 Debug
java

DEBUG_PARSER = true;
DEBUG_TOKEN_MANAGER = true;

📌 Objetivo Acadêmico

    Demonstrar construção de linguagens simples usando JavaCC

    Exercitar análise léxica e sintática

    Praticar estruturas de controle e variáveis

👨‍💻 Autor

Desenvolvido para fins educacionais.
📄 Licença

Projeto de uso acadêmico livre.
Código

