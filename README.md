# Autoencoder: Detecção de anomalias

  Este projeto é uma implementação de um autoencoder com o objetivo de detectar possíveis transações ilegais.
  Essa arquitetura de rede neural tem como objetivo dar uma saída mais semelhante possível á entrada, de modo que
  seu aprendizado tenha comportamento igual a aproximação da função identidade hW,b(x)≈x
  
  Uma transação será classificada como legal ou ilegal com base no erro de reconstrução do algoritmo, calculado pela equação de erro quadrático médio.
  MSE é resultado da média do somátório da diferença entre os valores reais e preditos, elevados ao quadrado, conforme demonstra a seguinte equação. Esse valor deve ser minimizado ao máximo durante o treinamento.
  
  ![MSEformula](https://user-images.githubusercontent.com/51008104/88002656-6639cf00-cad9-11ea-98a9-fbceab93cb14.png)


  O algoritmo foi treinado apenas em dados de classificação positiva, de modo que o erro de reconstrução para a classe de transações legais seja a menor possível, assim,
  se receber um input onde possa haver uma probabilidade de ser uma transação ilegal, o erro de reconstrução será alto e consequentemente, classificado como ilegal.
 
  Os dados usados nesse proejto foi retirado de kaggle.com
