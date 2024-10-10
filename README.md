Exercício 1:

Descrição
Você está desenvolvendo um programa para verificar o estoque de produtos, e este desafio visa aplicar o conceito de Clean Architecture para uma solução mais estruturada e modular. A Clean Architecture, desenvolvida por Robert C. Martin (também conhecido como Uncle Bob), é uma abordagem que separa as responsabilidades de um sistema em camadas distintas. Isso permite uma melhor organização do código e facilita a manutenção e a escalabilidade.

Para este desafio, seu objetivo é implementar a camada de Casos de Uso utilizando o padrão Strategy para a lógica de verificação de estoque. Você precisará garantir que o código esteja organizado conforme os princípios da Clean Architecture. Você precisará implementar uma classe chamada `VerificarEstoqueStrategy` que deve seguir uma interface denominada `EstoqueStrategy`. Esta classe será responsável por verificar o nível de estoque de um produto e gerar uma mensagem adequada com base nesse nível.

Resumindo:

Você precisa implementar a classe `VerificarEstoqueStrategy` para:

- Implementar a interface `EstoqueStrategy`.
- Usar uma constante para definir o limite mínimo de estoque.
- Verificar a quantidade de estoque do produto e retornar uma mensagem apropriada com base nesse valor.

Saiba mais sobre: Clean Architecture

Entrada
O programa deve receber as seguintes entradas:

Nome do Produto: Uma string representando o nome do produto.

Quantidade em Estoque: Um inteiro representando a quantidade atual em estoque do produto.

Saída
"Alerta: Estoque baixo de X", onde X é o nome do produto, se a quantidade em estoque for menor do que o limite mínimo pré-definido de 10 unidades.

"Estoque de X esta em nivel adequado", onde X é o nome do produto, se a quantidade em estoque for igual ou maior que o limite mínimo pré-definido de 10 unidades.




Exercício 2:

Descrição
Neste desafio, você desenvolverá uma solução que analise transações financeiras de um cliente ao longo de um mês. O programa deve receber uma lista de transações e calcular o saldo final, a maior transação de depósito e a maior transação de retirada. Além disso, o programa deve verificar se o saldo final é positivo ou negativo.

Para resolver este desafio, você aplicará os conceitos de Clean Architecture. Seu objetivo é completar a classe AnaliseTransacoesUseCase, utilizando os conceitos de Clean Architecture. Dessa forma, implemente a condição necessária para a análise das transações e construa a saída de acordo com a análise.

Saiba mais sobre: Clean Architecture

Entrada
O programa deve receber:

1. O número de transações.

2. Uma lista de números representando as transações (valores positivos para depósitos e valores negativos ( - ) para retiradas).

Saída
Saldo: X, onde X é o saldo final após todas as transações.

Deposito: Y, onde Y é o valor da maior transação de depósito.

Retirada: Z, onde Z é o valor da maior transação de retirada.

Saldo positivo ou Saldo negativo, dependendo do valor do saldo final.



Exercício 3:

Descrição
No seu desafio, você irá implementar um sistema de monitoramento de temperatura aplicando a Clean Architecture. Cada componente do sistema deve ser criado e utilizado conforme as regras da arquitetura para garantir uma separação clara de responsabilidades. Abaixo, você encontrará o detalhamento das tarefas que devem ser realizadas. Dessa forma, o objetivo é implementar o sistema de monitoramento de temperatura seguindo a Clean Architecture. Você deve focar na criação de classes e interfaces para cada parte da arquitetura, assegurando que as responsabilidades estejam bem definidas e separadas.

Detalhamento das Tarefas:

1. Criação e execução do caso de uso: Nesta parte do código, você deve instanciar a implementação do caso de uso `MonitoramentoTemperaturaUseCaseImpl`. Esta classe contém a lógica de monitoramento de temperatura e gera os alertas se alguma sala exceder o limite.

2. Criação e execução do apresentador: Aqui, você deve instanciar o apresentador que implementa a interface `MonitoramentoTemperaturaPresenter`. Esta instância será usada pelo controlador para apresentar os resultados ao usuário.

3. Criação do controlador: Nesta parte, você deve criar uma instância do controlador, passando o caso de uso (`useCase`) e o apresentador (`presenter`) como parâmetros. O controlador será responsável por orquestrar a execução do caso de uso e a apresentação dos resultados.

Saiba mais sobre: Clean Architecture

Entrada
O programa deve receber:

O número de salas no data center.

Para cada sala, a temperatura atual.

Saída
"Alerta: Sala X excedeu o limite de temperatura!" se a temperatura da sala X exceder o limite estabelecido.