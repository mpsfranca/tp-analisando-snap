# Análise Estrutural de Grafos: Rede web-flickr

Este repositório contém o código-fonte, o dataset principal e a análise topológica do grafo `web-flickr`, desenvolvidos como Trabalho Prático para a disciplina de Teoria dos Grafos.

## Sobre o Dataset

O grafo analisado representa uma rede de compartilhamento de imagens extraída do **Stanford Network Analysis Project (SNAP)**. Os vértices representam imagens e as arestas representam metadados compartilhados (mesma galeria, localização, fotógrafo, etc.).

O arquivo principal contendo as conexões do grafo (`flickrEdges.txt.gz`) **está disponibilizado neste repositório** para facilitar a reprodução do código. No entanto, os arquivos complementares com atributos de nós, atributos de arestas e metadados XML detalhados (`nodeFeatures.tar.gz`, `edgeFeatures.tar.gz`, `flickrXml.tar.gz`) não foram incluídos. Eles podem ser baixados diretamente da fonte oficial:
* [Dataset web-flickr no site oficial do SNAP](http://snap.stanford.edu/data/web-flickr.html)

## Pré-requisitos

Para executar o Jupyter Notebook, você precisará das seguintes bibliotecas Python instaladas:

* `networkx`
* `matplotlib`
* `numpy`

Você pode instalá-las rodando o seguinte comando no seu terminal:
```bash
pip install networkx matplotlib numpy
