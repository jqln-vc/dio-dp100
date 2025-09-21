# dio-dp100

## Prevendo Vendas de Sorvete com Machine Learning

### Cenário do Projeto: Gelato Mágico

Imagine que somos proprietários da sorveteria **Gelato Mágico**, localizada em uma cidade litorânea. Diariamente, a quantidade de sorvetes vendidos varia drasticamente, e percebemos uma forte correlação entre as vendas e a temperatura ambiente.

Para otimizar nossa produção e evitar o desperdício ou a perda de vendas, decidimos usar Machine Learning. Nosso objetivo é construir um modelo preditivo capaz de prever as vendas diárias de sorvete com base na temperatura, permitindo um planejamento de produção mais eficiente.

---

### O que foi feito neste projeto

Este projeto prático foi desenvolvido para aplicar os conceitos de **Machine Learning para Regressão Preditiva** utilizando as ferramentas e serviços da **Microsoft Azure**. A seguir, apresento os principais pontos abordados:

* **Análise Inicial dos Dados:** Utilizamos dados fictícios de temperatura e vendas para iniciar a modelagem. No arquivo `inputs/temperatura_vendas.txt`, podemos ver a base de nossas informações para a análise.
* **Treinamento do Modelo no Azure Machine Learning:** Em vez de usar bibliotecas locais, treinamos nosso modelo de regressão diretamente na plataforma **Azure Machine Learning**. Isso nos permite aproveitar o poder computacional da nuvem e gerenciar todo o ciclo de vida do modelo em um único lugar.
* **Gerenciamento de Modelos:** A funcionalidade de **Registro de Modelos do Azure Machine Learning** foi usada para versionar e gerenciar diferentes versões do nosso modelo. Isso garante a rastreabilidade e a reprodutibilidade dos nossos experimentos.
* **Implantação do Modelo como um Web Service:** O modelo treinado foi implantado como um **endpoint HTTP** usando o Azure Machine Learning. Isso nos permite criar uma API que recebe a temperatura como entrada e retorna a previsão de vendas em tempo real, pronta para ser consumida por outros aplicativos.

---

### Insights e Possibilidades de Melhoria

Após a análise inicial, alguns insights e possibilidades de melhoria já se destacam:

1.  **A Regressão é a Ferramenta Ideal:** A natureza do nosso problema, que é prever um valor contínuo (número de sorvetes), se alinha perfeitamente com os problemas de **regressão**. Modelos como Regressão Linear, Árvores de Decisão ou até Redes Neurais seriam ótimas opções, e o Azure ML oferece suporte a todos eles.
2.  **A Importância de Mais Dados:** O modelo inicial foi baseado em poucas sentenças. Para um resultado mais preciso e robusto, seria fundamental coletar mais dados históricos, incluindo outros fatores que podem influenciar as vendas, como feriados, eventos locais ou até mesmo o dia da semana.
3.  **Monitoramento e Automação:** O **Azure Machine Learning** permite automatizar o treinamento e a re-implantação do modelo (CI/CD). Também é possível monitorar o desempenho do modelo em produção e ser alertado sobre possíveis desvios, garantindo que a previsão continue precisa ao longo do tempo.
4.  **Integração com Outros Serviços Azure:** O modelo pode ser facilmente integrado com outros serviços como **Azure Functions** para processar eventos, **Azure Data Lake** para armazenar dados e **Power BI** para visualização e análise de vendas.

Este projeto demonstra como as ferramentas de nuvem da Microsoft podem ser usadas para construir e gerenciar soluções de Machine Learning de ponta a ponta. É uma excelente maneira de construir um portfólio e demonstrar habilidades práticas em MLOps e ciência de dados.
