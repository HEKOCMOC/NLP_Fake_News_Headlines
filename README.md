# Детектирование фейковых новостей :newspaper:
## Задача
Требуется разработать модель, которая будет способна различать заголовки реальных и выдуманных новостей.
## Дано
Для обучения модели будут использоваться данные из файла `train.tsv`. В файле находится таблица, состоящая из двух колонок. В колонке `title` записаны заголовки новостей. В колонке `is_fake` содержатся метки: 0 – новость реальная, 1 – новость выдуманная. <br/>
Для демонстрации работы модели используются данные тестового набора из файла `test.tsv`. В нем также есть колонка `title`, данные которой являются входными для модели. 
Необходимо скопировать файл `test.tsv`, переименовать его в predictions.tsv и заполнить колонку `is_fake` значениями предсказания модели, аналогично `train.tsv`. 
Изначально колонка заполнена значением 0.
## Результаты
index |	classifier |	results
--- | --- | ---
0 |	PassiveAggressiveClassifier	| 0.827257
2	| Logistic Regression	| 0.845486
3	| Linear SVC |	0.854167
1 |	MultinomialNB (Naive Bayes) |	0.855903

## Что можно добавить
- реализовать пайлайн
- попробовать automl
- применить BERT
