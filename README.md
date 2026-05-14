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

# Tarefa 4 — Objetos e Referência em Java

Objetivo:

Compreender o comportamento de objetos em chamadas de métodos em Java.



Java possui passagem por referência verdadeira?

Não. Java sempre utiliza passagem por valor.



O que é copiado na chamada?

No caso de objetos, o valor copiado é a referência do objeto.

Isso significa que o método recebe uma cópia da referência que aponta para o objeto original.



Por que alterações no objeto permanecem?

As alterações permanecem porque:
- o parâmetro do método;
- e a variável original;

apontam para o mesmo objeto na memória.


Quando o método altera:

p.preco = p.preco - 50;

o objeto original também é modificado.


Assim, aprendi que Java sempre usa passagem por valor e que em objetos, a referência é copiada. As alterações no objeto permanecem após a chamada do método.


------------------

# Projeto Livre: Agenda de Contatos Simples

Objetivo
Criar um sistema simples de agenda utilizando subprogramas.



Diagrama simples das chamadas

main()
 ├── mostrarMenu()
 ├── adicionarContato()
 ├── listarContatos()
 ├── buscarContato()
 │     ├── atualizarContato()
 │     └── removerContato()



Justificativa da divisão dos subprogramas

O programa foi dividido em funções menores para deixar o código mais organizado e menos confuso. Em vez de fazer tudo em um único bloco grande, cada função ficou responsável por uma parte específica do sistema, como adicionar contatos, buscar informações ou mostrar os dados na tela, tudo isso de forma bem organizada, o que ajuda muito no entendimento do código, especialmente para quem está começando ou não tem muita experiência. Dessa forma, ficou mais fácil entender o que cada parte do programa faz e também mais simples de mexer no código caso seja necessário fazer alguma alteração depois.

Dificuldades encontradas

Uma das maiores dificuldades foi entender melhor como os parâmetros funcionam nas funções e como retornar valores corretamente. Essa parte precisa de muita atenção e fazer muuuitos testes. Também foi um pouco complicado decidir o que cada função deveria fazer, principalmente para evitar repetir código. Em alguns momentos foi necessário organizar várias vezes partes do programa para deixar as funções mais separadas e com tarefas mais claras. Dá mais trabalho, mas compensa com código mais claro de entender.

Vantagens da modularização

Depois de dividir o programa em funções, o código ficou muito mais organizado e fácil de entender. Também ficou mais simples encontrar erros e fazer alterações sem precisar mexer em todo o sistema. Outro ponto positivo foi a reutilização de funções, já que algumas partes do código puderam ser usadas várias vezes sem precisar escrever tudo novamente. Isso ajudou a reduzir repetição e deixou o programa mais limpo.

Dessa forma, aprendi que enquanto estudante de programação tenho que me preocupar com a clareza do código para que futuramente eu ainda continue entendendo cada parte dele. E quando utilizo a modulação o processo fica mais transparente e mais simples de entender. Mas vi que é mais trabalho porque tenho que organizar o código e deixar ele enxuto. É preciso mais lógica e atenção, especialmente fazer mais testes para testar se as funções estão sendo chamadas e retornando valores corretamente. Achei uma experiência legal em fazer a comparação entre o código em bloco completo e o código com modularização.