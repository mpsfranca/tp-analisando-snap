# Análise Estrutural de Grafos: Rede web-flickr

Este repositório contém o código-fonte e a análise topológica do grafo `web-flickr`, desenvolvidos como Trabalho Prático para a disciplina de Teoria dos Grafos.

## Sobre o Dataset

O grafo analisado representa uma rede de compartilhamento de imagens extraída do **Stanford Network Analysis Project (SNAP)**. Os vértices representam imagens e as arestas representam metadados compartilhados (mesma galeria, localização, fotógrafo, etc.).

**Atenção:** Devido ao tamanho do dataset (mais de 105 mil vértices e 2.3 milhões de arestas), o arquivo original não está hospedado neste repositório. 
Para reproduzir os testes, baixe o arquivo `flickrEdges.txt.gz` diretamente da fonte oficial:
* [Link para o dataset web-flickr no SNAP](http://snap.stanford.edu/data/web-flickr.html)

## Pré-requisitos

Para executar o Jupyter Notebook, você precisará das seguintes bibliotecas Python instaladas:

* `networkx`
* `matplotlib`
* `numpy`

Você pode instalá-las rodando o seguinte comando no seu terminal:
`pip install networkx matplotlib numpy`

## Como Executar

1. Clone este repositório para a sua máquina local.
2. Baixe o arquivo `flickrEdges.txt.gz` no link do SNAP fornecido acima e coloque-o na mesma pasta do arquivo principal.
3. Abra o arquivo `notebooks_Graph.ipynb` em um ambiente Jupyter.
4. Execute as células sequencialmente para extrair a maior componente conexa, calcular as métricas estruturais e gerar as visualizações.

## Resultados Principais

O trabalho comprova a viabilidade e os limites computacionais da aplicação empírica de algoritmos clássicos em grafos de grande escala. A análise demonstra que a rede `web-flickr` possui características de Mundo Pequeno (*Small-World*) e segue uma topologia Livre de Escala (*Scale-Free*), apresentando alta resiliência a falhas graças à sua massiva clusterização local.
