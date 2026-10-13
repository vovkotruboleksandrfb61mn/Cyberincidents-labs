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

## Запуск

**У Colab** — відкрити ноутбук за кнопкою в таблиці й виконати *Runtime → Run all*.
Датасет завантажується з Kaggle автоматично, вивантажувати вручну нічого не треба.

**Локально** (Python 3.13):

```bash
python -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
jupyter notebook lab1/solution.ipynb   # або lab2/…, lab3/…
```

Перша клітинка ноутбука створює теки `data/` і `assets/` поруч із ним,
завантажує потрібні набори й перевіряє кількість колонок — щоб оновлення
версії набору на Kaggle не дало мовчки інших чисел, ніж у звіті.
