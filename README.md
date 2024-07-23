# IGORS_PIZZARIA

A “Igor’s Pizzaria” necessita de um sistema para gerenciar pedidos das pizzas. Utilizando o design pattern Builder
para criar diferentes tipos de pizza, permite-se a customização dos atributos de cada pizza. 

De acordo como o diagrama de classes abaixo, implemente um sistema que permita criação de pizzas com várias
configurações.

![Captura de tela de 2024-07-23 20-25-37](https://github.com/user-attachments/assets/f9964343-3abb-4c88-a1f5-13f309b4c117)

Após a implementação, explique porque o objeto builder, destacado no exemplo acima, precisou seu instanciado
duas vezes. Contemple na explicação como é o comportamento em memória dos objetos Pizza.Builder e Pizza.

R: No exemplo acima, o objeto Builder precisou ser instanciado duas vezes, pois caso não fosse, os dados da primeira Pizza criada atravez do Builder, seria replicado para os demais objtos de Pizza que vierao a seguir.
Ambos as classes guardam seus atributos, porém, a classe Builder é exclusivamente feita para "alimentar" a classe Pizza, que por sua vez, depende da classe Builder para receber valores para seus atributos.
