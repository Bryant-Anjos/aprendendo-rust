## Guessing Game

Programa desenvolvido em Rust com o propósito de estudo da linguagem.
O programa é um jogo de adivinha, aonde é gerado um número aleatório entre 1 e 100 e o usuário tem que acertar qual é.
Conforme o usuário vai digitando números, o programa diz se o número é menor, ou maior que o esperado, e caso o usuário acerte, o programa termina a execução com a mensagem "You win!".

O guia para desenvolver o programa pode ser encontrado em: (https://doc.rust-lang.org/book/ch02-00-guessing-game-tutorial.html).

### Aprendizados

O que foi aprendido nesse capítulo e nos anteriores foi:

- Criar um novo projeto em Rust usando o `Cargo`;
- Declaração de uma função usando `fn`;
- O `main` é a função que é executada quando executa o programa;
- O `println!` é uma macro usada para escrever no terminal;
- O que termina com `!` são macros e não funções;
- Declaração de variável com `let`;
- As variáveis no Rust por padrão são imutáveis, sendo necessário adicionar `mut` para permitir alterá-las ao longo do programa;
- O compilador do Rust possui inferência de tipos, então não é necessário sempre declarar o tipo da variável;
- Utilizar o `stdin` para receber o valor digitado pelo usuário;
- Utilizar o `match` para decidir o que o programa vai fazer dependendo do resultado recebido;
- Adicionar uma dependência no arquivo `Cargo.toml`;
- Usar o `loop` para fazer uma repetição infinita;
- Usar o `break` para parar o `loop` e o `continue` para pular para a pŕoxima iteração.
