# lnpg-cap9-subprogramas-JAMES-HOFMANN
ATIVIDADE 7 - Cap. 09

James Tavares Hofmann
LNPG-BSI-2026.1


### Tarefa 1 — Modularização em Java

O objetivo da atividade foi desenvolver um sistema de controle acadêmico em Java utilizando subprogramas.

O sistema:
- lê o nome de 5 alunos;
- lê 3 notas para cada aluno;
- calcula a média;
- determina a situação do aluno;
- exibe um relatório final.



Versão Monolítica:

Na primeira versão, todo o sistema foi desenvolvido dentro do método main.

Características:
- código concentrado em um único bloco;
- pouca separação de responsabilidades;
- maior repetição de lógica;
- difícil manutenção.

Versão Modularizada:

Na segunda versão, o sistema foi dividido em subprogramas.

Métodos criados:
- lerAluno() # Responsável apenas por ler o nome. Retorna uma String.
- lerNotas() # Responsável apenas por ler as notas. Retorna um vetor de notas.
- calcularMedia() # Recebe notas por parâmetro. Retorna a média.
- determinarSituacao() #Recebe a média e retorna a situação do aluno.
- imprimirRelatorio() # Responsável apenas pela saída final do sistema.


Objetivo da modularização:
- melhorar organização;
- facilitar manutenção;
- evitar repetição de código;
- aumentar legibilidade.

-----------------



# Tarefa 2: Sistema de Vendas

Objetivo

Desenvolver um sistema de vendas em Python utilizando modularização e funções.



Versão monolítica

A primeira versão foi criada utilizando apenas um bloco principal.

Problemas encontrados:
- código grande;
- pouca organização;
- difícil manutenção;
- responsabilidades misturadas.



Versão modularizada

Na segunda versão, o sistema foi dividido em funções menores.

Funções criadas:
- ler_produto()
- ler_quantidade()
- ler_preco()
- calcular_subtotal()
- calcular_desconto()
- calcular_total()
- imprimir_cupom()



Partes repetitivas

As partes relacionadas aos cálculos e impressão poderiam gerar repetição caso o sistema aumentasse.

A modularização ajudou a separar essas responsabilidades.



Partes mais reutilizáveis

As funções de cálculo ficaram reutilizáveis:
- calcular_subtotal()
- calcular_desconto()
- calcular_total()




Impacto da modularização na legibilidade

A modularização melhorou:
- organização do código;
- clareza do fluxo;
- entendimento das responsabilidades;
- facilidade de manutenção.

O programa ficou mais simples de ler e compreender.

-----------------



# Tarefa 3 — Passagem de Parâmetros por Valor em Java

Objetivo:

Compreender como funciona a passagem de parâmetros por valor em Java utilizando tipos primitivos.


Por que o valor original não mudou?

O valor original não mudou porque o método recebeu apenas uma cópia do valor da variável.


No programa, a variável original é:

int numero = 10;



Quando ela foi enviada para o método:

alterarNumero(numero);

o Java copiou o valor 10 para a variável local x.


Dentro do método:

x = 100;

somente a cópia foi alterada.

A variável numero do main continuou armazenando o valor original.


O que significa “passagem por valor”?

Passagem por valor significa que o método recebe uma cópia do valor da variável.

Em tipos primitivos do Java:

int
double
char
boolean

o valor é copiado para o parâmetro do método.

Isso significa que:
- alterações feitas dentro do método;
- não modificam a variável original.


Qual valor realmente foi copiado?

O valor copiado foi 10. Esse valor saiu da variável numero e foi copiado para x.


Mudança local

A mudança aconteceu apenas dentro do método:

x = 100;

O valor de x mudou localmente para 100.


Ausência de mudança externa


Após a execução do método, o valor original permaneceu igual:

numero = 10


Isso demonstra que a alteração ocorreu apenas localmente.

Assi, aprendi que Java utiliza passagem por valor para tipos primitivos.

O método recebe apenas uma cópia do valor, e não a variável original.

Por isso:

- a variável local pode ser alterada;
- a variável externa permanece inalterada.

--------------------






------------------

# Projeto Livre: Agenda de Contatos Simples

Objetivo
Criar um sistema simples de agenda utilizando subprogramas.

---

Diagrama simples das chamadas

main()
 ├── mostrarMenu()
 ├── adicionarContato()
 ├── listarContatos()
 ├── buscarContato()
 │     ├── atualizarContato()
 │     └── removerContato()

---

---
Justificativa da divisão dos subprogramas

O programa foi dividido em funções menores para:
- melhorar organização;
- facilitar manutenção;
- evitar repetição de código;
- melhorar legibilidade.

Cada função possui apenas uma responsabilidade.

---

Dificuldades encontradas

- Entender passagem de parâmetros;
- Trabalhar com retorno de funções;
- Organizar responsabilidades do programa;
- Reutilizar funções corretamente.

---

Vantagens da modularização

- Código mais organizado;
- Mais fácil de entender;
- Facilita manutenção;
- Permite reutilização;
- Reduz repetição de código.