
# 🚔 Detecção de Veículos Roubados com Visão Computacional

Este projeto utiliza modelos de visão computacional para auxiliar na detecção de veículos roubados em imagens. Por meio de algoritmos de detecção de objetos (YOLO e Faster R-CNN) combinados com OCR (Reconhecimento Óptico de Caracteres), o sistema identifica veículos e extrai suas placas, permitindo uma comparação com bancos de dados de veículos roubados.

## 🔍 Objetivo

Com o crescimento dos crimes relacionados a furtos e roubos de veículos, o uso de tecnologias como a visão computacional pode auxiliar as autoridades na identificação e recuperação desses automóveis. O projeto visa:

- Detectar veículos em imagens usando modelos pré-treinados.
- Aplicar OCR para leitura automática das placas.
- Comparar os resultados e o desempenho dos modelos YOLO e Faster R-CNN.
- Avaliar o desempenho com métricas como acurácia, revocação e perda.

## 🧠 Tecnologias Utilizadas

- **YOLOv8** (Ultralytics)
- **Faster R-CNN** (PyTorch + torchvision)
- **EasyOCR** para leitura de placas
- **Dataset ALPR/UFPR** (como referência de estrutura de treino/teste)
- **OpenCV**, **Matplotlib**, **NumPy**, **PIL**

## 📁 Estrutura do Projeto

```
.
├── data/                        # Diretório com imagens e rótulos
│   ├── images/
│   └── labels/
├── YOLO.ipynb                   # Notebook de detecção usando YOLO
├── FASTER_R_CNN.ipynb           # Notebook de detecção usando Faster R-CNN
└── README.md                    # Este arquivo
```

## 📦 Requisitos

**Requisitos principais:**

- `torch`
- `torchvision`
- `ultralytics`
- `easyocr`
- `opencv-python`
- `matplotlib`

## 📊 Resultados

O projeto exibe visualmente os resultados de detecção e os textos das placas detectadas, junto com gráficos de perda por época no caso do Faster R-CNN. Espera-se um desempenho superior em ambientes variados e flexibilidade na integração com sistemas de monitoramento público.

## 🛡️ Aplicações Futuras

- Integração com bancos de dados policiais em tempo real
- Detecção em vídeo (streaming)
- Aplicações embarcadas com Raspberry Pi ou Jetson Nano

## 📚 Referência Teórica

Este projeto foi desenvolvido no contexto de um estudo sobre o uso de visão computacional na segurança pública, focando na aplicação prática de modelos de detecção combinados com OCR. O objetivo final é contribuir com soluções tecnológicas que agilizem a identificação de veículos roubados em ambientes urbanos.
