# lnpg-cap9-subprogramas-JAMES-HOFMANN
ATIVIDADE 7 - Cap. 09

James Tavares Hofmann
LNPG-BSI-2026.1


### Tarefa 1 — Modularização em Java
Objetivo: Dividir um programa grande em subprogramas.

O porquê da modulação utilizada

---
lerAluno()

Responsável apenas por ler o nome.

public static String lerAluno()

Retorna uma String.

---

lerNotas()

Responsável apenas por ler as notas.

public static double[] lerNotas()

Retorna um vetor de notas.

---

calcularMedia()

Recebe notas por parâmetro.

calcularMedia(double[] notas)

Retorna a média.
---



determinarSituacao()

Recebe a média e retorna a situação do aluno.

determinarSituacao(double media)

---

imprimirRelatorio()

Responsável apenas pela saída final do sistema.




-----------------
Agenda de Contatos

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