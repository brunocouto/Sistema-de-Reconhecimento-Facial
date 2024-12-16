Sistema de Reconhecimento Facial

Introdução

Este projeto implementa um sistema de detecção e reconhecimento facial utilizando o framework TensorFlow em conjunto com outras bibliotecas, como OpenCV. O sistema é capaz de detectar múltiplas faces em tempo real e classificá-las utilizando um modelo de reconhecimento pré-treinado.

Funcionalidades

Detecção de faces: Baseado em um modelo de detecção de faces, como Haar Cascade.

Reconhecimento facial: Utiliza um modelo pré-treinado para classificar as faces detectadas.

Detecção em tempo real: Integração com a webcam para processar vídeos ao vivo.

Requisitos

Ferramentas Necessárias

Python 3.6 ou superior

TensorFlow (>= 2.0)

OpenCV

Instalação das Dependências

Execute o seguinte comando para instalar as dependências:

pip install tensorflow opencv-python numpy

Arquivos Necessários

Modelo de detecção de faces: Arquivo XML do Haar Cascade, já incluído no OpenCV.

Modelo de reconhecimento facial: Um modelo .h5 pré-treinado salvo no mesmo diretório do script Python.

Estrutura do Projeto

/facial_recognition_project
  - facial_recognition.py
  - recognition_model.h5
  - README.md

Como Usar

Prepare o Modelo de Reconhecimento:

Treine ou baixe um modelo de reconhecimento facial e salve-o como recognition_model.h5.

O modelo deve ser compatível com a entrada de imagens no formato (224, 224, 3).

Configure as Classes:

Edite o arquivo facial_recognition.py para incluir os rótulos correspondentes ao seu modelo:

labels = ["Person 1", "Person 2", "Unknown"]

Execute o Sistema:

Inicie o script com:

python facial_recognition.py

O sistema abrirá a câmera e mostrará as faces detectadas e reconhecidas em tempo real.

Interrompa o Sistema:

Pressione a tecla q para finalizar a execução.

Exemplo de Resultado

O sistema exibirá a imagem da câmera com:

Retângulos ao redor das faces detectadas.

Rótulos indicando a identidade da pessoa ou "Unknown" para não reconhecidos.

Considerações Finais

Este projeto pode ser adaptado para diversas aplicações que envolvem reconhecimento facial, como sistemas de segurança e autenticação. Ele oferece uma base sólida para futuras melhorias e personalizações.