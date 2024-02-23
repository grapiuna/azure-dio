# azure-dio
Bootcamp Microsoft Azure AI Fundamentals da Dio.me

Tutorial de como criar um modelo de previsão com seus devidos pontos de extremidade configurados no Azure.

1 - Crie sua conta no Azure se não tiver: https://portal.azure.com;

2 - Clique em Novo repositório e digite um nome;

3 - Inicie o Studio do Azure Machine Learning;

4 - No Studio clique em ML Automatizado;

4 - Insira os seguintes dados: nome, descrição e tipo de tarefa;

5 - Escolha o banco dados da web e indique o url https://aka.ms/bike-rentals;

6 - Escolha Regressão e conclua;

7 - Clique em "Melhor resumo de modelo";

8 - Insira o nome do algoritmo e em métricas escolha residuos e predicted_true;

9 - Selecione o menu modelo e depois implantar (Deploy);

10 - No menu "Pontos de Extremidade" selecione o modelo anteriro;

11 - No menu teste, insira os seguintes dados:
```
{
   "Inputs": { 
     "data": [
       {
         "day": 1,
         "mnth": 1,   
         "year": 2022,
         "season": 2,
         "holiday": 0,
         "weekday": 1,
         "workingday": 1,
         "weathersit": 2, 
         "temp": 0.3, 
         "atemp": 0.3,
         "hum": 0.3,
         "windspeed": 0.3 
       }
     ]    
   },   
   "GlobalParameters": 1.0
 } 
 ```

12- Ele mostrará o seguinte resultado:
 ```
 {
  "Results": [
    345.35071706753126
  ]
}
```
