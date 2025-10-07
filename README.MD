Инструкция по запуску:
1. Создать виртуальное окружение: python -m venv venv
2. Активировать окружение: venv\Scripts\activate
3. Установить зависимости: pip install -r requirements.txt
4. Открыть блокнот: jupyter notebook NLP5.ipynb
5. В меню "Run" нажать "Run All Cells"

Описание работы:

В предыдущих работах 1-4 были построены классификаторы текстов

  Пр1:
  Наивный байесовского классификатор
  https://colab.research.google.com/drive/1PE1-ZMKvgFEU3bzm0uCBN3Hk6uyhBZGQ#scrollTo=03JrPK0ax3aZ

  Пр2:
  Классификатор на основе TfIdf и K ближайших соседей
  https://colab.research.google.com/drive/1gI4by1GY0tq9ZmD2DhI_Tfy_SzQ6Pdxk#scrollTo=aKweGb47Xn4X

  Пр3:
  Doc2Vec модель, позволяющая сравнивать близость текстов  
  https://colab.research.google.com/drive/18FCLP9r72usyY9cktZJinzpgkSD6EPNR#scrollTo=2rjRws177JRN

  Пр4:
  CNN-классификатор на базе Doc2Vec модели
  https://colab.research.google.com/drive/1USavQLcUXA08xcmoow0U50wZK2j_mv5_#scrollTo=N_BhyNFrRGYk


В настоящей работе реализован генератор текста на базе LSTM, обученный на векторах полученной ранее в Пр3 Doc2Vec модели.
В генераторе текста используется классификатор из Пр4 на базе CNN, обученный на тех же векторах.
Функцию очистки небходимо было модицифицировать (в данной работе не используется очистка от стоп-слов, лемматизация) в целях геренации более осмысленного текста
