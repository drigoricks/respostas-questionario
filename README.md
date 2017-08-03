# respostas-questionario

  4)  O que é Deadlock? Detalhe um pouco sobre o caso e como você poderia resolver isso.
      
      Deadlock é o bloqueio de execução devido a interdependência entre processos em um dado momento, ou seja, 
      quando um processo A depende do processo B e B também depende A em um mesmo instante, ocorre um bloqueio 
      pois tanto A como B são interdependentes.
      
      Para evitar devemos sempre liberar recursos e os acessos aos recursos quando não mais utilizados.
      
      
  5)	Uma das grandes inclusões no Java 8 foi a API Stream. Com ela podemos fazer diversas operações de loop, filtros, maps, etc. 
      Porém, existe uma variação bem interessante do Stream que é ParallelStreams. 
      Descreva com suas palavras qual é a diferença entre os dois e quando devemos utilizar cada um deles.
      
      Principal diferença esta na forma de processamento a primeira variação, utiliza uma única Thread para efetuar o processando, 
      enquanto a segunda subdivide em uma ou mais Thread, o que em grande parte explica a melhor performance da ParrarelStream.
      
      Devemos usar a ParallelStreams quando for necessario filtrar um grande volume de dados, pois ganhamos em desempenho 
      pois a filtragem é feita de forma paralela todo o poder de processamento disponibilizado pelo hardware, usando o mesmo
      somente com operações paralelizadas.
