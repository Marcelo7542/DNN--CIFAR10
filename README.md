English Description Below:

Prática de Redes Neurais Profundas (DNN) com Diferentes Inicializações e Arquiteturas

Decidi explorar o treinamento de Redes Neurais Profundas (DNN) aplicadas ao conjunto de dados CIFAR-10. 

Meu objetivo foi experimentar diferentes abordagens de inicialização de pesos e modificações nas arquiteturas. 

Aqui estão os tipos de DNN que implementei:

Estrutura Geral

DNN com Inicialização He Normal e Swish:

Camadas densas com ativação "Swish".

Inicialização dos pesos com "He Normal".

Treinamento sem normalização dos dados.

DNN com Batch Normalization:

Camadas densas com inicialização "He Normal".

Aplicação de "Batch Normalization" após cada camada.

Ativação "Swish" após a normalização.

DNN com Inicialização LeCun Normal e SELU:

Camadas densas com ativação "SELU".

Inicialização dos pesos com "LeCun Normal".

Dados normalizados antes do treinamento.

DNN com Dropout, Batch Normalization e Swish:

Camadas densas maiores, combinando "Batch Normalization" e "Dropout".

Ativação "Swish" após cada camada.

Uso de inicialização "He Normal" para os pesos.

Configuração dos Hiperparâmetros

Para todas as redes, testei diferentes otimizadores, funções de perda e callbacks para acompanhar o progresso e melhorar o treinamento. Adotei técnicas como:

EarlyStopping para interromper o treinamento quando não houvesse melhora significativa.

ModelCheckpoint para salvar os melhores pesos.

TensorBoard para monitoramento visual.

ReduceLROnPlateau para ajustes dinâmicos na taxa de aprendizado.




Practice with Deep Neural Networks (DNN) Using Different Initializations and Architectures

I decided to explore training Deep Neural Networks (DNN) applied to the CIFAR-10 dataset. My goal was to experiment with different weight initialization approaches and architectural modifications. 

Here are the types of DNNs I implemented:

General Structure

DNN with He Normal Initialization and Swish Activation:

Dense layers with "Swish" activation.

Weight initialization using "He Normal".

Training without data normalization.

DNN with Batch Normalization:

Dense layers with "He Normal" initialization.

Application of "Batch Normalization" after each layer.

"Swish" activation after normalization.

DNN with LeCun Normal Initialization and SELU Activation:

Dense layers with "SELU" activation.

Weight initialization using "LeCun Normal".

Data normalized before training.

DNN with Dropout, Batch Normalization, and Swish Activation:

Larger dense layers combining "Batch Normalization" and "Dropout".

"Swish" activation after each layer.

Weight initialization using "He Normal".

Hyperparameter Configuration

For all networks, I tested different optimizers, loss functions, and callbacks to track progress and enhance training. I employed techniques such as:

EarlyStopping to stop training when no significant improvement was observed.

ModelCheckpoint to save the best weights.

TensorBoard for visual monitoring.

ReduceLROnPlateau for dynamic learning rate adjustments.

