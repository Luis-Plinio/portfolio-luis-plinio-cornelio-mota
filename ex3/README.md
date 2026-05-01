📖 Entendendo a Lógica do Sistema
O sistema foi desenhado para seguir uma sequência linear de pensamento, dividida em três fases principais: Coleta, Processamento e Fechamento.

1. A Fase de Coleta (Entradas)
O programa começa interagindo com o usuário para obter os dados brutos. Ele solicita, um por um, o preço de três produtos diferentes. Imagine que você está no caixa de uma loja e passa três itens pelo leitor; cada um desses valores é armazenado temporariamente na memória para que possamos trabalhar com eles a seguir.

2. O Processamento Matemático
Com os três valores em mãos, o sistema realiza dois cálculos automáticos:

O Somatório (Total): Primeiro, ele junta os valores dos três produtos para descobrir quanto o cliente deve no total. É essa conta que define o valor final da nota fiscal.

A Média de Preço: O sistema divide o total por três. Isso serve para dar ao lojista uma visão do "ticket médio" daquela compra, ajudando a entender se o cliente levou produtos caros ou mais populares.

3. A Finalização e o Troco (Lógica de Decisão)
Esta é a parte "inteligente" do sistema. Após mostrar o total ao cliente, o programa pergunta quanto ele entregou em dinheiro para pagar a conta. Aqui, o sistema precisa tomar uma decisão baseada em uma condição:

Se o dinheiro for suficiente: O sistema subtrai o valor da compra do valor pago. O resultado dessa conta é o troco. O programa então confirma que o pagamento foi aprovado e informa quanto deve ser devolvido ao cliente.

Se o dinheiro for insuficiente: O sistema percebe que o valor pago é menor que o total da compra. Em vez de calcular o troco, ele exibe uma mensagem de erro ou alerta, avisando que o valor não cobre o custo dos produtos.
