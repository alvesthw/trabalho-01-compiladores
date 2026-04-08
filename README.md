# README da Linguagem T01 — versão comentada em Python

"""
# 🧠 Linguagem T01 — Documentação Oficial
# Cabeçalho do projeto mostrando o nome da linguagem

## 📌 Visão Geral
# Breve descrição do objetivo da linguagem T01
# Desenvolvida para fins acadêmicos usando JavaCC
# Permite criar programas simples com:
# - Declaração de variáveis
# - Atribuições
# - Entrada e saída de dados
# - Estruturas condicionais e de repetição
# - Estruturas de decisão switch-case
# O parser possui configuração de debug para acompanhar análise léxica e sintática

---

## ⚙️ Tecnologias Utilizadas
# Linguagens e ferramentas usadas no projeto
# - Java
# - JavaCC

---

## 🚀 Como Executar

### 1. Pré-requisitos
# Antes de executar, é necessário:
# - Java JDK instalado
# - JavaCC configurado no ambiente

### 2. Executando o projeto
# Passos para compilar e executar o parser

# 1. Compile o arquivo .jj com JavaCC
# bash command:
# javacc T01.jj

# 2. Compile os arquivos Java gerados
# bash command:
# javac *.java

# 3. Execute o parser
# bash command:
# java trabalho1.T01

# Arquivo de entrada usado no parser:
# ..//JavaCC//src//trabalho1//teste07.txt

### 3. Estrutura Léxica
# Definição dos tokens, tipos de dados e palavras reservadas da linguagem

# 🔹 Tokens Principais
# Parênteses: (, )
# Chaves: {, }
# Colchetes: [, ]
# Fim de linha: ;
# Operadores de comparação: =, ==, !=, >, <, >=, <=

# 🔹 Tipos de Dados
# Inteiro: int
# Float: float
# Booleano: bool
# Caractere: char

# 🔹 Palavras Reservadas
# Estruturas de decisão: if, else, switch, case, default
# Estruturas de repetição: while, do, for, break
# Entrada e saída: input, printf
# Booleanos: true, false

# 🔹 Identificadores
# regex: [a-zA-Z][a-zA-Z0-9]*

# 🔹 Números
# regex: [0-9]+

# 🔹 Comentários
# Exemplo de comentário de linha:
# // comentário de uma linha

# 🧱 Estruturas da Linguagem

# Declaração de Variáveis
# Exemplo:
# int x;
# int y = 10;
# float z = 5;
# bool ativo = true;
# char c = 'a';

# Atribuição de Valores
# Exemplo:
# x = 10;
# c = 'a';

# Entrada de Dados
# Exemplo:
# input("Digite algo");
# int(input("Digite um número"));

# Saída de Dados
# Exemplo:
# printf("Hello");
# printf(x);

# Estruturas de Controle

# IF / ELSE
# Exemplo:
# if (x == 10) {
#     printf("Igual");
# } else {
#     printf("Diferente");
# }

# WHILE
# Exemplo:
# while (x < 10) {
#     x++;
# }

# DO-WHILE
# Exemplo:
# do {
#     x++;
# } while (x < 10);

# FOR
# Exemplo:
# for (i = 0; i < 10; i++) {
#     printf(i);
# }

# SWITCH / CASE
# Exemplo:
# switch(x) {
#     case(1):
#         printf("Um");
#         break;
#     case(2):
#         printf("Dois");
#         break;
#     default:
#         printf("Outro");
#         break;
# }

# ⚠️ Regras Importantes
# - Toda instrução termina com ;
# - Blocos delimitados por { }
# - Strings usam " ", caracteres usam ' '
# - Operadores válidos: ==, !=, >, <, >=, <=

# 📂 Estrutura do Projeto
# trabalho1/
#  ├── T01.jj        # Arquivo da gramática JavaCC
#  ├── T01.java      # Parser gerado
#  ├── teste07.txt   # Arquivo de entrada de teste

# 🐞 Debug
# DEBUG_PARSER = true;
# DEBUG_TOKEN_MANAGER = true;

# 📌 Objetivo Acadêmico
# - Demonstrar construção de linguagens simples usando JavaCC
# - Exercitar análise léxica e sintática
# - Praticar estruturas de controle e variáveis

# 👨‍💻 Autor
# Desenvolvido para fins educacionais

# 📄 Licença
# Projeto de uso acadêmico livre
"""
