# **Atividade de Programação 02**
## **Um Agente Inteligente para Classificação de Pedestres**

IA  2021.1e

Prof. Herman Gomes

---

A detecção da presença de pedestres em cenas de trânsito com vistas a [evitar atropelamentos](https://www.youtube.com/watch?v=vI9EIjUx20I) é uma tarefa crítica para o desenvolvimento de veículos autônomos e  sistemas avançados de assistência ao motorista - preservar a vida humana deve ser uma diretiva ética fundamental na concepção de tais sistemas. 

Inserido neste contexto, o propósito da Atividade de Programação 02 é desenvolver um agente inteligente para uma instância mais simples da tarefa, em que regiões candidatas da imagem já foram segmentadas e o objetivo do agente inteligente é decidir se uma determinada região contém ou não contém um pedestre. Em outras palavras, o seu agente irá receber um recorte de imagem em tons de cinza do ambiente e retornar uma classificação binária (contém ou não contém um pedestre). O agente deverá aprender de forma supervisionada na modalidade offline (o treinamento ocorre por completo antes do agente entrar em operação). 

Para o desenvolvimento desta atividade, deve-se utilizar a base de dados “[Daimler Pedestrian Classification Benchmark Dataset](http://www.gavrila.net/Datasets/Daimler_Pedestrian_Benchmark_D/Daimler_Mono_Ped__Class__Bench/daimler_mono_ped__class__bench.html)”. Mais especificamente, o “[Base pedestrian classification data set](http://www.lookingatpeople.com/data/Daimler/pami06-munder-gavrila/DC-ped-dataset_base.tar.gz)”. 

Além disso, considerar uma técnica de aprendizagem de máquina como base para funcionamento do seu agente. Algumas possibilidades:

* Uma rede Neural Convolucional operando diretamente sobre as imagens.
* Uma rede neural MultiLayer Perceptron operando sobre versões reduzidas (redimensionadas) das imagens de entrada
* Uma árvore de decisão (ou RandomForest) operando sobre vetores de características extraídos das imagens  (.e.g. histogramas de cores, bordas, texturas). As características podem também ser obtidas a partir de um autocodificador neural. 
* Um classificador Bayesiano (NaïveBayes) operando sobre características extraídas das imagens
* Rede Bayesiana operando sobre características extraídas das imagens

As equipes podem testar os exemplos de códigos python vistos em aula e buscar adaptá-los para esta tarefa, escolhendo (para constar na resposta da equipe) a solução que produzir os melhores resultados. 

Alternativamente, para acelerar o tempo de treinamento, as equipes podem também adaptar um modelo de rede neural pré-treinado (como VGG16), como discutido neste [post](https://machinelearningmastery.com/how-to-use-transfer-learning-when-developing-convolutional-neural-network-models/),  e refinar o treinamento para o caso de classificação de pedestres.

***Roteiro da atividade:***
1.   Criem uma cópia do notebook da atividade, para edição pelos componentes da equipe. Ao concluir a atividade, façam download do notebook (.ipynb) acrescentem a extensão .txt e faça o upload do arquivo do notebook (.ipynb.txt) como resposta da tarefa.
2.   Completem as partes faltantes da implementação do Agente PedestrianClassifier
3. Realizem o treinamento do agente, conforme a seção correspondente no notebook da atividade. 
4. Implementem os códigos faltantes para uso e avaliação do desempenho do agente, façam o experimento final, sempre respondendo às questões formuladas no notebook. 

Boa sorte e bom trabalho!

---
