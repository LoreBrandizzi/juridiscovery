# Ambiente Python para Análise de Processos Judiciais

Este projeto utiliza bibliotecas de NLP, análise de tópicos e manipulação de dados para processar e analisar informações de processos judiciais.

---

## ✅ Pré-requisitos

- [Anaconda ou Miniconda instalado](https://www.anaconda.com/download)
- Python 3.9 (o ambiente será criado com essa versão)
- Arquivo `requirements.txt` fornecido (deve estar salvo no mesmo diretório)

---

## ⚙️ Passo a passo para instalar o ambiente do zero

### 1. Feche o Jupyter Notebook (se estiver aberto)

---

### 2. Abra o **Anaconda Prompt**

---

### 3. Crie o ambiente virtual com nome `processos_judiciais`

```bash
conda create -n processos_judiciais python=3.9 -y
```

---

### 4. Ative o ambiente

```bash
conda activate processos_judiciais
```

---

### 5. Navegue até a pasta onde está o `requirements.txt`

Por exemplo:

```bash
cd C:\Users\SeuUsuario\Documents\meu_projeto
```

Substitua pelo caminho correto da sua máquina.

---

### 6. Instale as bibliotecas listadas

```bash
pip install -r requirements.txt
```

---

### 7. Registre o ambiente no Jupyter

```bash
pip install ipykernel
python -m ipykernel install --user --name processos_judiciais --display-name "Python (processos_judiciais)"
```

---

### 8. Abra o Jupyter Notebook

```bash
jupyter notebook
```

No Jupyter, selecione o kernel:  
**`Python (processos_judiciais)`**

---

## 🔁 Como abrir o Jupyter nas próximas vezes

Sempre que quiser usar o ambiente novamente:

1. Abra o **Anaconda Prompt**
2. Ative o ambiente:

```bash
conda activate processos_judiciais
```

3. Abra o Jupyter:

```bash
jupyter notebook
```

E selecione o kernel **Python (processos_judiciais)**

---

## 🧪 Verificação rápida

Em uma célula Jupyter, rode:

```python
from bertopic import BERTopic
from umap import UMAP
import torch, pandas as pd, numpy as np
from transformers import AutoTokenizer

print("Ambiente pronto para uso!")
```

!IMPORTANTE! Certifique-se na sua IDE se está usando realmente o Kernel correto. 
No Jupyter, troque o kernel: Vá em Kernel > Change kernel > Python (processos_judiciais)

---

## ✅ Observações

- O arquivo `requirements.txt` já contém todas as bibliotecas com versões compatíveis, incluindo:
  - `bertopic`
  - `umap-learn`
  - `sentence-transformers`
  - `transformers`
  - `torch`
  - `psycopg2-binary`
  - `matplotlib`
  - `pandas`, `numpy`, `numba`, `llvmlite`, etc.
