# solution_sprintG
sprint 1 - MBA ED - FIAP

Passos:

1 - preparar o ambiente seguindo os passos => https://github.com/fabiogjardim/bigdata_docker.git .

2 - na web, abrir: localhost:8888 (HUE), ir em files e criar o diretório "dataset", para que os futuro arquivos sejam carregados no HDFS.

3 - no google drive, crie uma pasta "Dataset" e suba o arquivo "olist_geolocation_dataset.csv" presente no diretório "solution_sprintG\Projeto\datasetKaggle".

4 - usando o google colab, execute o arquivo "Geolocalização.ipynb" (local: solution_sprintG\Projeto\Python) para que a API seja executada e atualizar a latitude e longitude presentes no dataset "olist_geolocation_dataset.csv". Ao fim um novo arquivo será salvo no diretório criado no google Drive.
Obs.: a execução da API leva quase 6hrs.

5 - Após finalizar a API, execute o arquivo "Merge_dataset.ipynb" (local: solution_sprintG\Projeto\Python), também no google colab, para que seja realizado o merge entre os datasets.

6 - Baixe os dois arquivos após finalizar a execução. Obs.: os arquivos já estão presentes no diretório "solution_sprintG\Projeto\datasetUpdate"

7 - Voltando ao 2 passo, dentro do diretório "dataset", carregar os diretórios presentes em "solution_sprintG\Projeto\datasetKaggle" para o HDFS.

8 - No diretório "geolocation", dentro do HUE, excluir o arquivo existente e importar o arquivo "olist_geolocation_dataset_updt.csv" do diretório "solution_sprintG\Projeto\datasetUpdate", que contém a geolocalização atualizada.

9 - Ainda no HUE, localize "Documents" e clique. No ícone com três pontos em vertical, escolher a opção import. Abrirá uma caixinha para escolher o Json. Carregue o Json presente no diretório "solution_sprintG\DDLs". Você terá todas as DDLs das para criar no HIVE e queries para extração de dados conforme previsto na solution sprint.
