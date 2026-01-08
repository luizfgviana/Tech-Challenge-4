# Tech-Challenge-4
👁️ Análise de Vídeo com Visão Computacional
Este projeto cria uma aplicação que utuliza a análise de vídeo incorporando detecção facial, reconhecimento de emoções e análise de movimentos corporais. Os scripts foram desenvolvidos independentemente para facilitar a organização e execução do código.

✨ Funcionalidades
O projeto é composto por três scripts principais:

face_detection_webcam.py:
Detecção Facial em Tempo Real: Identifica e marca rostos em um feed de vídeo da webcam.
emotion_detection_video.py:
Reconhecimento de Expressões Faciais: Analisa um arquivo de vídeo fornecido pelo curso de MBA IA pada Devs da FIAP/Alura. O script é utilizado para detectar rostos e identificar suas emoções dominantes (feliz, triste, neutro, etc.), gerando um novo vídeo com a deteção dos rostos e identificação das exmpressões.
movement_detection_video.py:
Análise de Poses e Movimentos Corporais: Processa um arquivo de vídeo ornecido pelo curso de MBA IA pada Devs da FIAP/Alura. O script é utilizado para detectar poses, contar movimentos específicos (agachamentos, levantar braços, T-poses, concordância, discordância, passos) e identificar anomalisas (movimentos não reconhecidos). Gera um vídeo com a identificação das lanmarks e resumo automático (contadores de movimentos e número de frames analisados).

⚙️ Pré-requisitos
Para rodar os scripts, você precisará ter o Python instalado e as seguintes bibliotecas:

Python 3.x
OpenCV (opencv-python)
DeepFace (deepface)
MediaPipe (mediapipe)
TensorFlow (tensorflow) e tf-keras (dependências da DeepFace e MediaPipe)
tqdm (para barras de progresso no processamento de vídeo)
numpy

📦 Instalação
Siga estes passos para configurar seu ambiente:

Clone o repositório (ou baixe os arquivos dos scripts):
git clone https://github.com/seu-usuario/seu-repositorio.git
cd seu-repositorio

Crie e ative um ambiente virtual (recomendado para isolar as dependências):
python -m venv venv
# No Windows:
.\venv\Scripts\activate
# No macOS/Linux:
source venv/bin/activate

Instale todas as dependências:
pip install opencv-python mediapipe deepface tensorflow tf-keras tqdm numpy

▶️ Como Usar
1. Detecção Facial em Tempo Real (face_detection_webcam.py)
Este script utiliza sua webcam para detectar rostos em tempo real.
Para executar:
python face_detection_webcam.py
Uma janela será aberta mostrando a sua webcam com retângulos ao redor dos rostos detectados.
Pressione a tecla q para parar a detecção.

2. Reconhecimento de Expressões (emotion_detection_video.py)
Este script processa um arquivo de vídeo e detecta emoções faciais.
Configuração:
Antes de executar, edite o script emotion_detection_video.py para definir os caminhos input_video_path (seu vídeo de entrada) e output_video_expressoes_path (onde o vídeo processado será salvo).
Para executar:
python emotion_detection_video.py
O script processará o vídeo e salvará um novo arquivo com as emoções detectadas.

3. Análise de Movimentos Corporais (movement_detection_video.py)
Este script processa um arquivo de vídeo para analisar poses e movimentos corporais.
Configuração:
Antes de executar, edite o script movement_detection_video.py para definir os caminhos input_video_path (seu vídeo de entrada) e output_video_movimentos_path (onde o vídeo processado será salvo).
Para executar:
python movement_detection_video.py
O script processará o vídeo e salvará um novo arquivo com as poses, movimentos e anomalias detectadas.
🤝 Contribuições
Agradeço todas as contribuições, críticas e comentários.

📄 Licença
Este projeto é de código aberto e está sob a licença MIT (se aplicável, inclua o arquivo LICENSE).
