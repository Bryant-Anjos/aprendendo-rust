## Rectangles

Programa desenvolvido em Rust com o propósito de estudo da linguagem.
O programa é a implementação de retângulos através da estrutura de dados `struct`.
São adicionados métodos à estrutura para calcular a área, verificar se um retângulo encaixa em outro e uma função associada para criar um quadrado, que nada mais é que um retângulo com ambas as dimensões iguais.

O guia para desenvolver o programa pode ser encontrado em: (https://doc.rust-lang.org/book/ch05-02-example-structs.html) e a continuação em (https://doc.rust-lang.org/book/ch05-03-method-syntax.html).

### Aprendizados

O que foi aprendido nesse capítulo foi:

- Criar uma estrutura usando `struct`;
- A struct pode ser feita como em forma de dicionário (chave -> valor), ou de tuplas (uma estrutura de dados do Rust);
- Acessar os atributos, métodos e funções da struct;
- Adicionar métodos às structs através do `impl`;
- Os métodos recebem o `self` como argumento e são acessados com o `.` na instância do objeto;
- As funções associadas não recebem o `self` e são acessadas com `::` direto na própria struct;
- Como imprimir a struct com a macro `println!` usando o `{:?}` e o `{:#?}` para uma formatação melhor. É necessário adicionar a annotation `#[derive(Debug)]` na declaração da struct.

E nos capítulos anteriores:

- Estudado mais a fundo as variáveis do Rust, que podem ser declaradas com `let`, com `mut` na frente caso deseje que a variável seja mutável, e `const` para criar constantes;
- A `const` precisa ter seu tipo especificado na declaração e precisa ser um valor que seja sabido qual é durante a etapa de compilação;
- Os tipos de dados primitivos, como inteiros, floats, booleanos, a string (str) e os tipos de dados compostos como tuplas e array. Esses todos possuem tamanho fixo e são armazenados na stack;
- As funções, que são bem semelhantes às de outras linguagens. podem receber argumentos ou não e são divididas em `statement` quando não retornam nada e `expression` quando retornam um valor. Uma diferença notável é que caso não adicione o `;` na última linha, essa linha se torna o valor a ser retornado da função, não sendo necessário adicionar um `return`;
- Comentários que sao adicionados com `//`;
- Estruturas de controle como o `if`, `else` e `elseif`, `loop` para loops infinitos, `while` e o `for`;
- Como as variáveis são alocadas na memória `stack` ou `heap`. Variáveis que se saibam o tamanho durante a etapa de compilação são alocadas na stack, enquanto aquelas de valores que podem variar são alocadas na heap e são acessadas através de um ponteiro, é nisso que se diferenciam os textos do tipo `str` e `String` do Rust;
- Os conceitos de `ownership`, `references` e `borrowing`. Variáveis com valores apontados para a memória `heap` mudam de dono quando são passadas para outras variáveis ou funções e são limpadas da memória quando termina o contexto a qual ela pertence. É possivel passa-las por referencia usando o `&` que quando for somente para leitura é passado uma cópia, mas quando é para alteração a referência muda o ownership;
- Sobre `shadowing`. É possível redeclarar a variável, mudando os seus valores e até mesmo o tipo. Todavia, o valor anterior não pode mais ser acessado;
- O `slice type ([..])`, que é utizado para acessar parte de valores da memória. Sua estrutura consiste em armazenar o índice inicial e o tamanho;
- O compilador do Rust sempre auxilia sobre como proceder com esses conceitos, nos mostrando o que não pode fazer, onde estão os erros e as possíveis soluções para resolve-los;
