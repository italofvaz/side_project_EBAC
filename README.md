# side_project_EBAC
projeto de machine leraning para prever boas gorgetas

o dataset utilizado foi o tips, importado da biblioteca Seaborn

COLETA DE DADOS: 
O conjunto de dados tips contém informações sobre gorjetas recebidas por garçons em um restaurante, registradas ao longo de vários atendimentos. 

elemntos do dataset:

total_bill:O valor total da conta do cliente (em dólares).
tip: O valor da gorjeta deixada pelo cliente (em dólares).
sex: O gênero do cliente que pagou a conta. 'Male' (homem) e 'Female' (mulher).
smoker: Indica se o cliente era fumante ou não. 'Yes' (fumante) e 'No' (não fumante).
day: O dia da semana em que o atendimento ocorreu. 'Thur' (quinta-feira), 'Fri' (sexta-feira), 'Sat' (sábado) e 'Sun' (domingo).
time: O período do dia em que ocorreu o atendimento. 'Lunch' (almoço) e 'Dinner' (jantar).
size: O número de pessoas na mesa (tamanho do grupo).

o codigo tem como objetivo prever se a gorjeta é boa ou não (probabilidade de boas gorjetas), entáo o problema é de classificação.

MODELAGEM:
para a previsao de probabilidades das classes (no caso, boas gorjetas) foi utilizado o modelo de arvore de decisáo. O método para isso foi o scikit-learn é predict_proba().

CONCLUSAO:
utilizamos tambem o XGBoost para treinar um modelo como o XGBClassifier, que nos permite a interpretação da importância das variáveis (features) utilizadas no modelo. A função plot_importance() do XGBoost nos ajudou a visualizar graficamente essa importância.

A importância das variáveis mede o quanto cada variável contribui para a decisão final do modelo.

