# Звіт до роботи
## Тема: _Оформлення робіт та перша програма_
### Мета роботи: _Розробка програми на Python та завантаження їх у репозиторій_
---
### Виконання роботи
- Результати виконання завдання *№1*;
1. Встановила додаткові плагіни
2. Створила новий файл `my_first_app.py` та скопіювала в нього код програми:
```python
from datetime import datetime
name = "Ivanna"
location = "Lviv"

print(f"{name} start programming at {datetime.now()}. {location} is the best city!") 
```

3.Програма вивела:

![alt text](https://github.com/ivanna2558/1_laba/raw/main/pictures/Результат.png "Результат")

4. Створила новий файл `my_first_app.ipynb` та прослідкувала як змінився вигляд Notebook. Зробила опис у вигляді заголовку.

![alt text](https://github.com/ivanna2558/1_laba/raw/main/pictures/code2.png "Результат")

5. Запитала у ChatGPT яку б першу програму написав АІ та чи б міг АІ пояснити її. Додала програму:
Ось приклад простої програми для класифікації текстової інформації за допомогою мови програмування Python та бібліотеки scikit-learn:

```python
# Імпортуємо необхідні бібліотеки
from sklearn.feature_extraction.text import CountVectorizer
from sklearn.naive_bayes import MultinomialNB
from sklearn.model_selection import train_test_split
from sklearn import metrics

# Задаємо дані для навчання (приклади текстів і їх класифікації)
texts = ["Це позитивний текст.", "Це також позитивний вислів.", "Це негативний вислів.", "Це негативний текст."]
labels = [1, 1, 0, 0]

# Розділяємо дані на тренувальний та тестовий набори
X_train, X_test, y_train, y_test = train_test_split(texts, labels, test_size=0.25, random_state=42)

# Використовуємо "bag of words" для представлення тексту числовими векторами
vectorizer = CountVectorizer()
X_train_vectorized = vectorizer.fit_transform(X_train)
X_test_vectorized = vectorizer.transform(X_test)

# Навчаємо класифікатор (використовуємо наївний Баєсівський класифікатор)
classifier = MultinomialNB()
classifier.fit(X_train_vectorized, y_train)

# Прогнозуємо класифікацію для тестового набору
y_pred = classifier.predict(X_test_vectorized)

# Виводимо результати
print("Точність класифікації:", metrics.accuracy_score(y_test, y_pred))

```


### Висновок: 
> у висновку потрібно відповісти на запитання:
- :question: Що зроблено в роботі;
- :question: Чи досягнуто мети роботи;
- :question: Які нові знання отримано;
- :question: Чи вдалось відповісти на всі питання задані в ході роботи;
- :question: Чи вдалося виконати всі завдання;
- :question: Чи виникли складності у виконанні завдання;
- :question: Чи подобається такий формат здачі роботи (Feedback);
- :question: Побажання для покращення (Suggestions);
---
