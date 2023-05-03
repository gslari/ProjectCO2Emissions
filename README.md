# Análise e Processamento de Dados Sobre Emissão de CO2
Este repositório é destinado à apresentação do primeiro MVP (Minimum Viable Product) elaborado como avaliação para a Sprint I do curso de pós-Graduação em Ciência de Dados e Analytics da Pontifícia Universidade Católica do Rio de Janeiro (PUC-RIO).

O Objetivo do trabalho é apresentar, pela base de dados, os números das emissões dos gases do efeito estufa por município, gás específico, gases totais e setor de origem. Comprovando assim a participação humana no fenômeno de aquecimento global por meio das emissões de gases poluintes, especificamente em Washington. Temos como finalidade Demonstrar por dados, os maiores setores, municípios mais poluentes e o gás mais recorrente.

![image](https://user-images.githubusercontent.com/82593529/236043176-a1658e65-a20d-4de4-8dd1-2e4617103e5f.png)


# Introdução
O efeito estufa é um fenômeno natural e possibilita a vida humana na Terra. Porém, o grande problema é que o efeito estufa está aumentando muito rapidamente neste último século, pois está havendo uma alta emissão de gases como gás carbônico, metano e óxido nitroso para a atmosfera. Assim gerando um acúmulo de calor retido na atmosfera da terra, fazendo a temperatura aumentar. Nos últimos 140 anos houve um aumento de 0,76°C, causando uma preocupação com a vida na terra. Outro aspecto distinto da mudança atual do clima é a sua origem: ao passo que as mudanças do clima no passado decorreram de fenômenos naturais, a maior parte da atual mudança do clima, particularmente nos últimos 50 anos, é atribuída às atividades humanas.
![image](https://user-images.githubusercontent.com/82593529/236043228-9f4fadbc-bd13-4f31-8f5d-38c6b4ab6ed9.png)


# Fonte da Base de Dados:
https://www.kaggle.com/ramyaparimi/greenhouse-gas-report-data-2015

#Descrição da Base de Dados:

1● Source: a origem dos gases apresentados na base de dados, a empresa responsável e afins.

2● County: os municípios envolvidos.

3● Address: os endereços das empresas responsáveis e afins.

4● Total Emissions: o número de emissões totais de gases.

5● Biogenic CO2: um dos gases a serem analisados

6● Fossil CO2: um dos gases a serem analisados

7● Methane: um dos gases a serem analisados.

8● Nitrous Oxide: um dos gases a serem analisados.

9● Hydrofluorocarbons: um dos gases a serem analisados.

10● Perfluorocarbons: um dos gases a serem analisados.

11● Sulfur Hexafluoride: um dos gases a serem analisados.

12● Other: outros gases menos dispersados. 13.Location: coordenadas geográficas.

13● Sector: setores originários dos gases.

14● Sub Sector: sub setores originários dos gases.

15● Clean Air Rule: regra de Washington que obriga empresas muito poluentes de diminuírem suas emissões de carbono.

16● Energy- Intesive: intensidade energética.

17● Point Size: tamanho relativo das emissões.

18● WAOFM: legislação.

19● Counties: condados de Washington.

# Número de Observações:
141 linhas representando as variáveis

# Metodologia:
Serão utilizados boxplots, gráfico de pizza, diagramas de dispersão, gráfico de barra.
Gráfico de pizza: utilizado para dividir em setores, exibindo uma informação relacionada.
Gráfico de Barras: é uma forma de resumir um conjunto de dados categóricos.
Gráfico de Linha: é utilizado para facilitar a identificação de tendências e anomalias.

# Bibliotecas Utilizadas:
Pandas
Matplotlib
IPython
statsmodels
scipy.stats

# Carregamento e Processamento dos dados
Nesta etapa vamos carregar o dataset da fonte ja citada e selecionar as colunas a serem utilizadas para eliminar as restantes:

![image](https://user-images.githubusercontent.com/82593529/236041431-028736df-1737-497a-92df-20b2d0856fa8.png)

# Visualização/Gráficos

1) Gráfico de Pizza

![image](https://user-images.githubusercontent.com/82593529/236041882-715fa40e-982c-4e5b-aa9a-d532613bd351.png)

Nesse gráfico pode-se ver que dentre os setores poluentes, o que mais aparece em termos de repetição e não maior poluição é a “Food Production”, mostrando que, ao menos em Washington, o setor de produção alimentícia é um setor que se repete, gerando impacto na emissão dos gases. Os outros dois setores são “Power Plants”, mostrando a poluição de usinas elétricas e “Wood Products”, que são produtos feitos de madeiras. Mostrando que esses três setores poluentes mais repetitivos , são setores de produção humana, e não naturais.

2) Gráfico de Barras

![image](https://user-images.githubusercontent.com/82593529/236042189-8bd72077-f20c-4511-b6f6-0ad5a1d3a0c0.png)

Nesse gráfico vemos a relação de emissões por setores nos municípios.Podemos perceber que,os municípios King,Pierce e Whatcom são considerados os maiores causadores da poluição,uma vez que,a liberação dos gases influencia o efeito estufa.

3) Gráfico de Linha

![image](https://user-images.githubusercontent.com/82593529/236042389-e02579b2-bd22-4c26-8e50-b59cec4ba1f7.png)

Mostra o aumento da concentração dos gases de CO2 Fóssil ao longo do crescimento das atividades:Refinaria- a utilização de combustivel é um risco para o meio ambiente pois,a extração e o transporte e até mesmo o consumo, provocam a ultilização de gases que atinge diretamente a natureza,“Wood Products” que são os produtos feitos por madeiras,“Power Plants” que apresenta a soltura dos gases poluentes por meios de usinas elétrica, e por ultimo,“Pulp and paper” celulose que é o aumento do desmatamento de árvores e ultilização de produtos químicos.

4) Boxplot

![image](https://user-images.githubusercontent.com/82593529/236042614-81889070-f54e-43a8-9d79-e24b6a294d77.png)

Boxplot mostra que os setores com as maiores emissões são o de Refinaria, uma vez que, as instalaçÕes de produção por processos e operações químicas possibilitam ainda mais as emissões,quando ocorre a degradação de certos materiais ou convertem matéria-prima em produtos de valor. O de Pulp and paper, que são os setores de celulose e papel, utilizam madeiras como forma de criar matéria prima,assim produzindo a celulose,papel,papelão e outros produtos.Desta forma,os dois maiores são causados por ação humana pois ao derrubar as árvores e usar compostos químicos contribui para o aumento do efeito estufa.

# Conclusão
Analizando as variáveis, conclui-se que os maiores setores que emitem poluição são os de Refinaria,Setor de Celulose e Papel,porém os que mais aparecem em termos de números são Produção de Comida e Usinas Elétricas, o gás mais recorrente é o CO2 Fóssil e os principais municípios que poluem são King,Pierce e Whatcom.

Assim, podemos finalizar que, BP Cherry Point Refinery - Blaine, em Whatcom, é a indústria mais poluente de Washington, se enquadrando no quesito município, setor e maior gás emitido, tendo um número de emissões totais de 2.093.437 e 2.077.888 de emissões de CO2 Fóssil.
![image](https://user-images.githubusercontent.com/82593529/236043294-fa6197c4-14cd-4828-9060-5a2e289242df.png)
