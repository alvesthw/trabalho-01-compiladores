🧠 Linguagem PYC — Documentação Oficial
📌 Visão Geral

A Linguagem PYC é uma linguagem acadêmica desenvolvida com JavaCC, que combina características das linguagens C e Python.

Ela foi projetada para ensinar conceitos de:

Análise léxica e sintática
Estruturas de controle
Tipagem de dados
Execução estruturada de programas
🔥 Principais características híbridas
Estilo C	Estilo Python
Uso de {} para blocos	Entrada dinâmica (input)
; obrigatório	Sintaxe simples e direta
Tipagem explícita	Conversão inline de tipos
switch-case, for	Flexibilidade de entrada
⚙️ Tecnologias Utilizadas
Java
JavaCC
🚀 Como Executar
1. Pré-requisitos
Java JDK instalado
JavaCC configurado
2. Passos
javacc T01.jj
javac *.java
java trabalho1.T01
📂 Arquivo de entrada
../JavaCC/src/trabalho1/teste18.txt
🔤 Estrutura Léxica
🔹 Tokens básicos
Parênteses: ( )
Chaves: { }
Colchetes: [ ]
Fim de linha: ;
Dois pontos: :
🔹 Operadores

Atribuição e comparação

=   ==   !=
>   <    >=   <=

Aritméticos

+   -   *   /   %
++  --
🔹 Tipos de dados
int     // inteiro
float   // ponto flutuante
bool    // booleano
char    // caractere
🔹 Valores booleanos
true
false
🔹 Identificadores
[a-zA-Z_][a-zA-Z0-9_]*
🔹 Números
[0-9]+
🔹 Strings
"texto"
🔹 Comentários
// comentário de uma linha
🧱 Estruturas da Linguagem
🔹 1. Declaração de Variáveis

Simples

int x;
float y;
bool ativo;
char c;

Com inicialização

int x = 10;
float y = 5;
bool ativo = true;
char c = 'a';
🔹 2. Atribuição
x = 10;
x = y + 5;
c = 'a';
🔹 3. Expressões

A linguagem suporta expressões matemáticas com precedência.

Operadores

+  -  *  /  %

Exemplo

x = (10 + 5) * 2;
🔹 4. Entrada de Dados (input)

Entrada simples

input("Digite algo");

Entrada com variável

input(x);

Conversão de tipo (híbrido C + Python)

int(input("Digite um número"));
float(input("Digite um número"));
char(input("Digite um caractere"));

👉 Destaque:

Entrada dinâmica (Python)
Conversão explícita (C)
🔹 5. Saída (printf)
printf("Hello");
printf(x);
🔄 Estruturas de Controle
🔹 6. IF / ELSE / ELSE IF
if (x == 10) {
    printf("Igual");
}
else if (x > 10) {
    printf("Maior");
}
else {
    printf("Menor");
}
🔹 7. WHILE
while (x < 10) {
    x++;
}
🔹 8. DO-WHILE
do {
    x++;
} while (x < 10);
🔹 9. FOR

Estilo C

for (i = 0; i < 10; i++) {
    printf(i);
}

Com declaração

for (int i = 0; i < 10; i++) {
    printf(i);
}
🔹 10. SWITCH / CASE
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
🔹 11. Vetores (Arrays)
int vetor[10];
float notas[5];

👉 Apenas declaração (sem acesso implementado)

🔹 12. Blocos (Funções simplificadas)
{
    printf("Executando bloco");
}

Limitações:

Sem nome
Sem parâmetros
Sem retorno
🧠 Regras Sintáticas Importantes
Toda instrução termina com ;
Blocos usam { }
Estruturas exigem ()
break obrigatório em case
Tipos obrigatórios
Strings usam " e char usa '
⚠️ Particularidades da Linguagem
🔥 Mistura de paradigmas
Sintaxe rígida (C)
Entrada dinâmica (Python)
Conversão inline
🔥 Conversão embutida
int(input("Digite: "));
🔥 Expressões completas
Parênteses ()
Colchetes [] como agrupadores
🔥 Incremento / Decremento
i++;
i--;
🔥 Condições

Formato padrão:

variavel operador valor
🐞 Debug
DEBUG_PARSER = true;
DEBUG_TOKEN_MANAGER = true;

Mostra:

Tokens reconhecidos
Regras sintáticas
📂 Estrutura do Projeto
trabalho1/
├── T01.jj
├── T01.java
├── teste18.txt
📌 Objetivo Acadêmico
Construção de linguagem com JavaCC
Estudo de parsing
Simulação de compilador
Integração C + Python
👨‍💻 Autor

Projeto desenvolvido para fins educacionais.

📄 Licença

Uso livre para fins acadêmicos.
