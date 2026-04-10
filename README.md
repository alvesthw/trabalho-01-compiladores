# Linguagem PyC — Documentação Oficial

##  Visão Geral

A **Linguagem PyC** é uma linguagem acadêmica desenvolvida em **Java** com a ferramenta **JavaCC**, que combina características das linguagens **C** e **Python**.

Ela foi projetada para ensinar/aplicação de conceitos sobre:

- Análise léxica e sintática
- Estruturas de controle
- Tipagem de dados
- Execução estruturada de programas

---

## Principais características da Linguagem PyC

- Linguagem C
- Possui tipagem explícita. Pois é uma linguagem imperativa/procedural estruturada
- Uso do ponto e vírgula `;` é obrigatório ao final de declarações
- Uso de chaves `{}` para início e fim de blocos de função
- Estruturas como 'switch-case' e 'for'

- Linguagem Python
- Entrada dinâmica através da função `input`.
- Conversão inline de tipos
- Lógica de controle
- Expressões parecidas


##  Tecnologias Utilizadas

- Eclipe IDE
- Linguagem Java
- Ferramenta JavaCC

##  Como Executar

### 1. Pré-requisitos

- IDE que peermita a execução de código Java, como o Eclipse IDE
- Java JDK instalado
- JavaCC configurado  

### 2. Passos

- Leia este arquivo README para entender todos os outros passos necessários.
- Faça o download do arquivo .zip ou clone o repositório para sua área de trabalho.

O código principal estará no arquivo chamado 'T01.jj' que está contido toda a definição da nossa linguagem PyC.

####Os arquivos de teste estão distribuídos da seguinte forma:
- Estão nomeados na forma: testeXX.txt
- teste01.txt até teste10.txt estão os programas considerados **válidos**, que são aceitos pela linguagem PyC
- teste11.txt até teste20.txt estão os programadas considerados **inválidos**, que **não** são aceitos pela linguagem PyC
- teste21.txt até teste25.txt estão os programas cópias dos válidos, porém com certas modificações que resultam em um programa **inválido**

##  Estrutura do Projeto

```
JavaCC/src/trabalho1/
├── T01.java
├── T01.jj
├── testeXX.txt
```

###  Arquivo de entrada

Para alterar o arquivo que está sendo analisado, altere a linha da função 'main':

```
FileInputStream fis = new FileInputStream(new File("..//JavaCC//src//trabalho1//testeXX.txt"));
```

Altere o caminho, substituindo testeXX.txt pelo nome certo do seu arquivo teste

---

##  Estrutura Léxica

###  Tokens básicos
#### 1. Literais e identificadores

- NUMERO -> números inteiros
- STRING -> "texto"
- IDENTIFICADOR -> nomes de variáveis (x, valor_1)

#### 2. Tipos de dados

- int     // inteiro
- float   // ponto flutuante
- bool    // booleano
- char    // caractere

#### 3. Valores booleanos

- true
- false

#### 4. Entrada e saída

- input
- printf

#### 5. Estruturas de controle

- if
- else
- while
- do
- switch
- case
- for
- break
- default

#### 6. Operadores aritméticos

- `+`
- `-`
- `*`
- `/`
- `%`
- `++`
- `--`

#### 7. Operadores relacionais e lógicos

- `=`
- `==`
- `!=`
- `>`
- `<`
- `>=`
- `<=`

#### 8. Símbolos especiais

- Parênteses: `( )`
- Colchetes: `[ ]`
- Chaves: `{ }`
- Fim de linha: `;` (EOL)
- Dois pontos: `:`
- ' -> aspas simples
- " -> aspas duplas

#### 9. Comentários

- // comentário

#### 10. Token composto (tipo)

- int
- float
- bool
- char


###  Identificadores

```
[a-zA-Z_][a-zA-Z0-9_]*
```

---

###  Números

```
[0-9]+
```

---

###  Strings

```
"texto"
```

---

##  Estruturas da Linguagem

###  1. Declaração de Variáveis

**Simples**
```c
int x;
float y;
bool ativo;
char c;
```

**Com inicialização**
```c
int x = 10;
float y = 5;
bool ativo = true;
char c = 'a';
```

---

###  2. Atribuição

```c
x = 10;
x = y + 5;
c = 'a';
```

---

###  3. Expressões

A linguagem suporta expressões matemáticas com precedência.

**Operadores**
```
+  -  *  /  %
```

**Exemplo**
```c
x = (10 + 5) * 2;
```

---

###  4. Entrada de Dados (`input`)

**Entrada simples**
```c
input("Digite algo");
```

**Entrada com variável**
```c
input(x);
```

**Conversão de tipo**
```c
int(input("Digite um número"));
float(input("Digite um número"));
char(input("Digite um caractere"));
```

---

###  5. Saída (`printf`)

```c
printf("Hello");
printf(x);
```

---

##  Estruturas de Controle

###  1. IF / ELSE / ELSE IF

```c
if (x == 10) {
    printf("Igual");
}
else if (x > 10) {
    printf("Maior");
}
else {
    printf("Menor");
}
```

###  2. WHILE

```c
while (x < 10) {
    x++;
}
```

###  3. DO-WHILE

```c
do {
    x++;
} while (x < 10);
```

###  4. FOR

```c
for (i = 0; i < 10; i++) {
    printf(i);
}
```

```c
for (int i = 0; i < 10; i++) {
    printf(i);
}
```

###  5. SWITCH / CASE

```c
switch(x) {
    case 1:
        printf("Um");
        break;
    case 2:
        printf("Dois");
        break;
    default:
        printf("Outro");
        break;
}
```

###  6. Vetores (Arrays)

```c
int vetor[10];
float notas[5];
```

---

###  7. Blocos

```c
{
    printf("Executando bloco");
}
```

---

##  Regras Sintáticas Importantes

- Toda instrução termina com `;`  
- Blocos usam `{ }`  
- Estruturas exigem `()`  
- `break` obrigatório em `case`  
- Tipos obrigatórios  
- Strings usam `"` e `char` usa `'`  

---

##  Particularidades

### Conversão inline
```c
int(input("Digite: "));
```

### Incremento
```c
i++;
i--;
```

---

##  Debug

```java
DEBUG_PARSER = true;
DEBUG_TOKEN_MANAGER = true;
```

---


##  Objetivo Acadêmico

- Construção de linguagem com JavaCC  
- Estudo de parsing  
- Simulação de compilador  
- Integração C + Python  

---

## Autores

- Matheus Alves Bueno  
- Felipe Biava Favarin   

---

##  Licença

Uso livre para fins acadêmicos.
