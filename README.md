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

---

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






-----------------



### Projeto Livre: Agenda de Contatos Simples

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