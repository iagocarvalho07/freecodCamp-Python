# Time Calculator

This is the boilerplate for the Time Calculator project. Instructions for building your project can be found at https://www.freecodecamp.org/learn/scientific-computing-with-python/scientific-computing-with-python-projects/time-calculator


Conclua a Categoryaula em budget.py. Ele deve ser capaz de instanciar objetos com base em diferentes categorias de orçamento, como alimentação , vestuário e entretenimento . Quando os objetos são criados, eles são passados ​​no nome da categoria. A classe deve ter uma variável de instância chamada ledgerque é uma lista. A classe também deve conter os seguintes métodos:

Um depositmétodo que aceita um valor e uma descrição. Se nenhuma descrição for fornecida, o padrão deve ser uma string vazia. O método deve anexar um objeto à lista de razão na forma de {"amount": amount, "description": description}.
Um withdrawmétodo semelhante ao depositmétodo, mas o valor passado deve ser armazenado no razão como um número negativo. Se não houver fundos suficientes, nada deve ser adicionado ao livro razão. Este método deve retornar Truese a retirada ocorreu e Falsecaso contrário.
Um get_balancemétodo que retorna o saldo atual da categoria de orçamento com base nos depósitos e saques ocorridos.
Um transfermétodo que aceita um valor e outra categoria de orçamento como argumentos. O método deve adicionar um saque com o valor e a descrição "Transferir para [Categoria de Orçamento de Destino]". O método deve então adicionar um depósito à outra categoria orçamentária com o valor e a descrição "Transferência de [Categoria Orçamentária de Origem]". Se não houver fundos suficientes, nada deve ser adicionado a nenhum dos livros contábeis. Este método deve retornar Truese a transferência ocorreu e Falsecaso contrário.
Um check_fundsmétodo que aceita um valor como argumento. Retorna Falsese o valor for maior que o saldo da categoria orçamentária e retorna Truecaso contrário. Este método deve ser usado tanto pelo withdrawmétodo quanto transferpelo método.
Quando o objeto de orçamento for impresso, ele deve exibir:

Uma linha de título de 30 caracteres onde o nome da categoria é centralizado em uma linha de *caracteres.
Uma lista dos itens no razão. Cada linha deve mostrar a descrição e o valor. Os primeiros 23 caracteres da descrição devem ser exibidos e, em seguida, o valor. A quantidade deve estar alinhada à direita, conter duas casas decimais e exibir no máximo 7 caracteres.
Uma linha exibindo o total da categoria.
Aqui está um exemplo da saída:

*************Food*************
initial deposit        1000.00
groceries               -10.15
restaurant and more foo -15.89
Transfer to Clothing    -50.00
Total: 923.96
Além da Categoryclasse, crie uma função (fora da classe) chamada create_spend_chartque receba uma lista de categorias como argumento. Ele deve retornar uma string que é um gráfico de barras.

O gráfico deve mostrar o percentual gasto em cada categoria repassado para a função. A porcentagem gasta deve ser calculada apenas com saques e não com depósitos. No lado esquerdo do gráfico, devem estar os rótulos de 0 a 100. As "barras" no gráfico de barras devem ser feitas com o caractere "o". A altura de cada barra deve ser arredondada para o 10 mais próximo. A linha horizontal abaixo das barras deve passar dois espaços após a barra final. Cada nome de categoria deve ser escrito verticalmente abaixo da barra. Deve haver um título no topo que diga "Porcentagem gasta por categoria".

Esta função será testada com até quatro categorias.

Observe a saída de exemplo abaixo com atenção e certifique-se de que o espaçamento da saída corresponda exatamente ao exemplo.

Percentage spent by category
100|          
 90|          
 80|          
 70|          
 60| o        
 50| o        
 40| o        
 30| o        
 20| o  o     
 10| o  o  o  
  0| o  o  o  
    ----------
     F  C  A  
     o  l  u  
     o  o  t  
     d  t  o  
        h     
        i     
        n     
        g     
Os testes de unidade para este projeto estão em test_module.py.

Desenvolvimento
Escreva seu código em budget.py. Para desenvolvimento, você pode usar main.pypara testar sua Categoryclasse. Clique no botão "executar" e main.pyserá executado.

teste
Importamos os testes de test_module.pypara main.pypara sua conveniência. Os testes serão executados automaticamente sempre que você clicar no botão "executar".

Enviando
Copie a URL do seu projeto e envie-a para freeCodeCamp.
