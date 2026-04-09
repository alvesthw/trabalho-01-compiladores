# 🧠 Linguagem PYC — Documentação Oficial

## 📌 Visão Geral

Linguagem desenvolvida para fins acadêmicos utilizando **JavaCC**.

Permite criar programas simples com:

* Declaração de variáveis
* Atribuições
* Entrada e saída de dados
* Estruturas condicionais e de repetição
* Estruturas de decisão (`switch-case`)

O parser possui configuração de debug para acompanhar a análise léxica e sintática.

---

## ⚙️ Tecnologias Utilizadas

* Java
* JavaCC

---

## 🚀 Como Executar

### 1. Pré-requisitos

* Java JDK instalado
* JavaCC configurado no ambiente

### 2. Passo a passo

#### 1. Gerar o parser com JavaCC

```bash
javacc T01.jj
```

#### 2. Compilar os arquivos Java

```bash
javac *.java
```

#### 3. Executar o parser

```bash
java trabalho1.T01
```

#### 4. Arquivo de entrada

```
../JavaCC/src/trabalho1/teste07.txt
```

---

## 🔤 Estrutura Léxica

### 🔹 Tokens

* Parênteses: `(` `)`
* Chaves: `{` `}`
* Colchetes: `[` `]`
* Fim de linha: `;`
* Operadores: `=`, `==`, `!=`, `>`, `<`, `>=`, `<=`

### 🔹 Tipos de Dados

* `int`
* `float`
* `bool`
* `char`

### 🔹 Palavras Reservadas

* Decisão: `if`, `else`, `switch`, `case`, `default`
* Repetição: `while`, `do`, `for`, `break`
* Entrada/Saída: `input`, `printf`
* Booleanos: `true`, `false`

### 🔹 Identificadores

```regex
[a-zA-Z][a-zA-Z0-9]*
```

### 🔹 Números

```regex
[0-9]+
```

### 🔹 Comentários

```c
// comentário de uma linha
```

---

## 🧱 Estruturas da Linguagem

### 🔹 Declaração de Variáveis

```c
int x;
int y = 10;
float z = 5;
bool ativo = true;
char c = 'a';
```

### 🔹 Atribuição

```c
x = 10;
c = 'a';
```

### 🔹 Entrada de Dados

```c
input("Digite algo");
int(input("Digite um número"));
```

### 🔹 Saída de Dados

```c
printf("Hello");
printf(x);
```

---

## 🔄 Estruturas de Controle

### IF / ELSE

```c
if (x == 10) {
    printf("Igual");
} else {
    printf("Diferente");
}
```

### WHILE

```c
while (x < 10) {
    x++;
}
```

### DO-WHILE

```c
do {
    x++;
} while (x < 10);
```

### FOR

```c
for (i = 0; i < 10; i++) {
    printf(i);
}
```

### SWITCH / CASE

```c
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
```

---

## ⚠️ Regras Importantes

* Toda instrução termina com `;`
* Blocos delimitados por `{ }`
* Strings usam `" "` e caracteres usam `' '`
* Operadores válidos: `==`, `!=`, `>`, `<`, `>=`, `<=`

---

## 📂 Estrutura do Projeto

```
trabalho1/
├── T01.jj
├── T01.java
├── teste07.txt
```

---

## 🐞 Debug

```java
DEBUG_PARSER = true;
DEBUG_TOKEN_MANAGER = true;
```

---

## 📌 Objetivo Acadêmico

* Demonstrar construção de linguagens com JavaCC
* Exercitar análise léxica e sintática
* Praticar estruturas de controle e variáveis

---

## 👨‍💻 Autor

Projeto desenvolvido para fins educacionais.

---

## 📄 Licença

Uso livre para fins acadêmicos.
