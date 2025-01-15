# Pipeline-Similarity

## Descrição do Projeto
Este projeto consiste em um pipeline de similaridade molecular baseado em SMILES canônicos. Ele processa dados químicos, calcula fingerprints moleculares utilizando o algoritmo Morgan (baseado em Tanimoto) e gera uma matriz de similaridade. Além disso, cria visualizações gráficas, como heatmaps, para facilitar a análise da similaridade entre moléculas.

## Requisitos
As bibliotecas necessárias para executar o pipeline são:

- Python 3.8 ou superior
- pandas
- numpy
- matplotlib
- seaborn
- rdkit
- scikit-learn

Para instalar todas as dependências, execute:
```bash
pip install pandas numpy matplotlib seaborn rdkit scikit-learn
```

## Instruções de Uso

1. Certifique-se de que o arquivo de dados de entrada no formato Excel (.xlsx) contém a coluna Canonical SMILES.
   
2. Substitua o caminho do arquivo na linha:

```python
file_path = "data-with-SMILES.xlsx"
```
pelo caminho do seu arquivo de dados.

3. Execute o script para gerar:
-Matriz de similaridade baseada na distância de Tanimoto.
-Heatmap de similaridade entre as moléculas.

4. O heatmap final será salvo como heatmap_similaridade2.png na mesma pasta do script.

## Estrutura do Repositório
Sugerimos que a estrutura do repositório seja organizada da seguinte forma:

```bash

root/
├── data/
│   └── full-smiles.xlsx           # Conjunto de dados de entrada
├── output/
│   └── heatmap_similaridade2.png  # Heatmap de similaridade gerado
├── src/
│   └── pipeline_similarity.py     # Script principal do pipeline
├── README.md                      # Documentação do projeto
└── requirements.txt               # Lista de dependências do projeto
```

## Licença
Este projeto está licenciado sob a licença MIT. Consulte o arquivo `LICENSE` para obter mais detalhes.

## Contribuições
Contribuições são bem-vindas! Sinta-se à vontade para abrir uma issue ou enviar um pull request.
