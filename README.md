# Redes Neurais Convolucionais

Exercícios e notebooks de estudo do curso **Convolutional Neural Networks**, o quarto curso da [Deep Learning Specialization](https://www.coursera.org/specializations/deep-learning), da DeepLearning.AI no Coursera. O curso é ministrado por Andrew Ng. Este repositório é um projeto de estudo independente e não é afiliado à DeepLearning.AI ou ao Coursera.

## Conteúdo

| Semana | Tópicos | Notebooks |
| --- | --- | --- |
| 1 | Convolução, pooling, backpropagation e classificação de sinais | [CNN passo a passo](week01/model-step-by-step.ipynb) · [Aplicação com TensorFlow](week01/model-application.ipynb) |
| 2 | Happy House, LeNet e ResNet | [Happy House](week02/keras-tutorial/keras-happy-house.ipynb) · [LeNet](week02/lenet/lenet-model.ipynb) · [ResNet](week02/resnet/resnet-model.ipynb) |
| 3 | Detecção de objetos com YOLO e supressão não máxima | [YOLO](week03/yolo-model.ipynb) |
| 4 | Reconhecimento facial e transferência de estilo neural | [Face Recognition](week04/face-recognition/face-recognition.ipynb) · [Neural Style Transfer](week04/neural-style-transfer/art-generation.ipynb) |

Os diretórios de cada semana também contêm funções auxiliares, imagens e datasets usados pelos notebooks.

## Como abrir

É necessário Python e Jupyter Notebook ou JupyterLab. Para criar um ambiente isolado e abrir o Jupyter:

```bash
python -m venv .venv
source .venv/bin/activate  # Windows: .venv\Scripts\activate
python -m pip install jupyter
jupyter lab
```

Abra o notebook desejado no Jupyter. Os notebooks usam caminhos relativos; execute cada um com o diretório do próprio notebook como diretório de trabalho.

## Compatibilidade e arquivos externos

Os notebooks foram escritos para versões antigas de TensorFlow, Keras e SciPy. Eles usam APIs que foram removidas ou alteradas nas versões atuais, como `tf.Session`, `tf.placeholder` e `scipy.misc.imread`. O repositório não fixa uma combinação de dependências validada; para executar os exercícios, pode ser necessário preparar um ambiente legado compatível com cada notebook.

Alguns exercícios também esperam arquivos de pesos que não estão incluídos aqui: `week02/resnet/ResNet50.h5`, `week03/model_data/yolo.h5`, os CSVs em `week04/face-recognition/weights/` e `week04/neural-style-transfer/pretrained-model/imagenet-vgg-verydeep-19.mat`. Consulte as instruções e referências dentro de cada notebook para obter esses arquivos. Alguns datasets da semana 4 estão compactados em `.zip` e podem precisar ser extraídos antes da execução.
