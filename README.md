# Reconhecimento de Emoções Faciais em Tempo Real com CNNs e filtro HaarCascade

O presente projeto é parte do trabalho de Exame da disciplina CT-213 - inteligência Artificial aplicada à Robótica Móvel. As referências utilizadas para o projeto encontram-se discriminadas no artigo presente neste repositório.

A apresentação das funcionalidades estão melhor descritas no arquivo .ipynb principal.

---

🚀 Tecnologias e Bibliotecas

- Python 3.10+
- TensorFlow / Keras
- OpenCV
- NumPy
- Matplotlib
- FER2013 Dataset

---

## 💻 Guia de Instalação e Execução

### 1. ⚙️ Clonar o repositório

```bash
git clone https://github.com/seu-usuario/seu-repositorio.git
cd seu-repositorio
```

### 2. 🧪 Criar Ambiente Virtual (recomendado)

```bash
# No Linux/macOS
python3 -m venv venv
source venv/bin/activate

# No Windows
python -m venv venv
venv\Scripts\activate
```

### 3. 📦 Instalar as dependências

Certifique-se de que o arquivo `requirements.txt` está presente. Para instalar:

```bash
pip install -r requirements.txt
```

---

## 🧠 Treinamento do Modelo

> O arquivo jupyter notebook contém toda a estrutura de pré-processamento, construção da CNN e treinamento. Recomenda-se que, caso você não queira utilizar os pesos prontos e deseje treinar novamente a rede, se utilize o Google Colab. Localmente pode ser muito custoso e demorado.

- Execute-o localmente ou em um ambiente como o JupyterLab.
- Os pesos do modelo final será salvo como `weights_emotions.hdf5`.

---

## 📸 Execução em Tempo Real (Detecção via Webcam)

A simulação se encontra ao final do script. É necessário rodar a aplicação localmente, para o programa ter acesso à webcam.

### 🔹 Tecla Especial:

- Pressione `q` para **encerrar o programa**

### 🚨 Requisitos:

- O arquivo `haarcascade_frontalface_default.xml` deve estar em `./detection`
- O modelo treinado `weights_emotions.hdf5` deve estar em `./model`

## 🎓 Dataset Utilizado

- [FER2013 - Facial Expression Recognition 2013](https://www.kaggle.com/c/challenges-in-representation-learning-facial-expression-recognition-challenge/data)
- 35.887 imagens 48x48 em tons de cinza com 7 classes: Angry, Disgust, Fear, Happy, Sad, Surprise, Neutral

---

📌 Melhorias Futuras

- Sugestões e contrubuições para melhorias no projeto são muito bem-vindas.

---

## 👥 Autores

- Ulisses Lopes da Silva - [@ulissesuls](https://github.com/ulissesuls)

---

## 📄 Licença

Este projeto está licenciado sob os termos da **MIT License**. Veja o arquivo [LICENSE](LICENSE) para mais detalhes.
