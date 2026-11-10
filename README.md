# Аналіз кіберінцидентів — практичні роботи

Вовкотруб Олександр Віталійович, група ФБ-61мн
Навчально-науковий фізико-технічний інститут, кафедра інформаційної безпеки
КПІ ім. Ігоря Сікорського

Викладач: Наконечна Юлія Володимирівна

| № | Тема | Датасет | Ноутбук | Звіт |
|---|------|---------|---------|------|
| 1 | Логістична регресія | [UCI Malware Executable Detection](https://www.kaggle.com/datasets/piyushrumao/malware-executable-detection) | [solution.ipynb](lab1/solution.ipynb) · [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/vovkotruboleksandrfb61mn/Cyberincidents-labs/blob/main/lab1/solution.ipynb) | [PDF](lab1/PZ1_LogisticRegression_Vovkotrub_FB-61mn.pdf) |
| 2 | Дерево рішень і ліс дерев рішень | [UGRansome](https://www.kaggle.com/datasets/nkongolo/ugransome-dataset), [NSL-KDD](https://www.kaggle.com/datasets/sampadab17/network-intrusion-detection), [Cybersecurity Intrusion](https://www.kaggle.com/datasets/dnkumars/cybersecurity-intrusion-detection-dataset) | [solution.ipynb](lab2/solution.ipynb) · [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/vovkotruboleksandrfb61mn/Cyberincidents-labs/blob/main/lab2/solution.ipynb) | [PDF](lab2/PZ2_DecisionTreeForest_Vovkotrub_FB-61mn.pdf) |
| 3 | Метод опорних векторів | [UGRansome](https://www.kaggle.com/datasets/nkongolo/ugransome-dataset) | [solution.ipynb](lab3/solution.ipynb) · [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/vovkotruboleksandrfb61mn/Cyberincidents-labs/blob/main/lab3/solution.ipynb) | [PDF](lab3/PZ3_SVM_Vovkotrub_FB-61mn.pdf) |
| 4 | Наївний байєсівський класифікатор | [Ham & Spam Messages](https://www.kaggle.com/datasets/muhammadahmedansari/ham-spam-messages-dataset) | [solution.ipynb](lab4/solution.ipynb) · [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/vovkotruboleksandrfb61mn/Cyberincidents-labs/blob/main/lab4/solution.ipynb) | [PDF](lab4/PZ4_NaiveBayes_Vovkotrub_FB-61mn.pdf) |
| 5 | Метод k-найближчих сусідів | [UGRansome](https://www.kaggle.com/datasets/nkongolo/ugransome-dataset) | [solution.ipynb](lab5/solution.ipynb) · [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/vovkotruboleksandrfb61mn/Cyberincidents-labs/blob/main/lab5/solution.ipynb) | [PDF](lab5/PZ5_kNN_Vovkotrub_FB-61mn.pdf) |
| 6 | Метод k-середніх та ієрархічна кластеризація | [UGRansome](https://www.kaggle.com/datasets/nkongolo/ugransome-dataset) | [solution.ipynb](lab6/solution.ipynb) · [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/vovkotruboleksandrfb61mn/Cyberincidents-labs/blob/main/lab6/solution.ipynb) | [PDF](lab6/PZ6_Clustering_Vovkotrub_FB-61mn.pdf) |
| 7 | LSH-хешування | [MNIST](https://www.kaggle.com/datasets/wasiqaliyasir/digital-mnist-dataset) | [solution.ipynb](lab7/solution.ipynb) · [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/vovkotruboleksandrfb61mn/Cyberincidents-labs/blob/main/lab7/solution.ipynb) | [PDF](lab7/PZ7_LSH_Vovkotrub_FB-61mn.pdf) |
| 8 | DBSCAN і A/B-тестування | [UGRansome](https://www.kaggle.com/datasets/nkongolo/ugransome-dataset) | [solution.ipynb](lab8/solution.ipynb) · [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/vovkotruboleksandrfb61mn/Cyberincidents-labs/blob/main/lab8/solution.ipynb) | [PDF](lab8/PZ8_DBSCAN_ABTesting_Vovkotrub_FB-61mn.pdf) |
| 9 | Нейронні мережі | [MNIST](https://www.kaggle.com/datasets/wasiqaliyasir/digital-mnist-dataset) | [solution.ipynb](lab9/solution.ipynb) · [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/vovkotruboleksandrfb61mn/Cyberincidents-labs/blob/main/lab9/solution.ipynb) | [PDF](lab9/PZ9_NeuralNetworks_Vovkotrub_FB-61mn.pdf) |

## Запуск

**У Colab** — відкрити ноутбук за кнопкою в таблиці й виконати *Runtime → Run all*.
Датасет завантажується з Kaggle автоматично, вивантажувати вручну нічого не треба.

**Локально** (Python 3.13):

```bash
python -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
jupyter notebook lab1/solution.ipynb   # або lab2/…, lab3/… — до lab9
```

Перша клітинка ноутбука створює теки `data/` і `assets/` поруч із ним,
завантажує потрібні набори й перевіряє форму таблиці — щоб оновлення
версії набору на Kaggle не дало мовчки інших чисел, ніж у звіті.
