# Проект 4. Задача классификации

## Оглавление
[1. Описание проекта](https://github.com/KislyukAnna/sf_data_science/tree/main/Project_4#%D0%BE%D0%BF%D0%B8%D1%81%D0%B0%D0%BD%D0%B8%D0%B5-%D0%BF%D1%80%D0%BE%D0%B5%D0%BA%D1%82%D0%B0)
[2. Какой кейс решаем?](https://github.com/KislyukAnna/sf_data_science/tree/main/Project_4#%D0%BA%D0%B0%D0%BA%D0%BE%D0%B9-%D0%BA%D0%B5%D0%B9%D1%81-%D1%80%D0%B5%D1%88%D0%B0%D0%B5%D0%BC)
[3. Информация о данных](https://github.com/KislyukAnna/sf_data_science/tree/main/Project_4#%D0%B8%D0%BD%D1%84%D0%BE%D1%80%D0%BC%D0%B0%D1%86%D0%B8%D1%8F-%D0%BE-%D0%B4%D0%B0%D0%BD%D0%BD%D1%8B%D1%85)
[4. Этапы работы над проектом](https://github.com/KislyukAnna/sf_data_science/tree/main/Project_4#%D1%8D%D1%82%D0%B0%D0%BF%D1%8B-%D1%80%D0%B0%D0%B1%D0%BE%D1%82%D1%8B-%D0%BD%D0%B0%D0%B4-%D0%BF%D1%80%D0%BE%D0%B5%D0%BA%D1%82%D0%BE%D0%BC)
[5. Результат](https://github.com/KislyukAnna/sf_data_science/tree/main/Project_4#%D1%80%D0%B5%D0%B7%D1%83%D0%BB%D1%8C%D1%82%D0%B0%D1%82%D1%8B)
[6. выводы ](https://github.com/KislyukAnna/sf_data_science/tree/main/Project_4#%D0%B2%D1%8B%D0%B2%D0%BE%D0%B4%D1%8B)


### Описание проекта
Вам предоставили данные о последней маркетинговой кампании, которую проводил банк: задачей было привлечь клиентов для открытия депозита. Вы должны проанализировать эти данные, выявить закономерность и найти решающие факторы, повлиявшие на то, что клиент вложил деньги именно в этот банк. Если вы сможете это сделать, то поднимете доходы банка и поможете понять целевую аудиторию, которую необходимо привлекать путём рекламы и различных предложений.

:arrow_up:[к оглавлению](https://github.com/KislyukAnna/sf_data_science/tree/main/Project_4#%D0%BE%D0%B3%D0%BB%D0%B0%D0%B2%D0%BB%D0%B5%D0%BD%D0%B8%D0%B5)


### Какой кейс решаем?
Задача бинарной классификации по табличным данным.

Бизнес-задача: определить характеристики, по которым можно выявить клиентов, более склонных к открытию депозита в банке, и за счёт этого повысить результативность маркетинговой кампании.

Техническая задача специалиста Data Science: построить модель машинного обучения, которая на основе предложенных характеристик клиента будет предсказывать, воспользуется он предложением об открытии депозита или нет.

:arrow_up:[к оглавлению](https://github.com/KislyukAnna/sf_data_science/tree/main/Project_4#%D0%BE%D0%B3%D0%BB%D0%B0%D0%B2%D0%BB%D0%B5%D0%BD%D0%B8%D0%B5)

### Информация о данных

[Файл с исходными данными можно скачать здесь](https://lms.skillfactory.ru/assets/courseware/v1/dab91dc74eb3cb684755123d224d262b/asset-v1:SkillFactory+DSPR-2.0+14JULY2021+type@asset+block/bank_fin.zip)

Данные о клиентах банка:

- age (возраст);
- job (сфера занятости);
- marital (семейное положение);
- education (уровень образования);
- default (имеется ли просроченный кредит);
- housing (имеется ли кредит на жильё);
- loan (имеется ли кредит на личные нужды);
- balance (баланс).
- deposit (имеется ли открытый депозит)

Данные, связанные с последним контактом в контексте текущей маркетинговой кампании:

- contact (тип контакта с клиентом);
- month (месяц, в котором был последний контакт);
- day (день, в который был последний контакт);
- duration (продолжительность контакта в секундах).

Прочие признаки:

- campaign (количество контактов с этим клиентом в течение текущей кампании);
- pdays (количество пропущенных дней с момента последней маркетинговой кампании до контакта в текущей кампании);
- previous (количество контактов до текущей кампании);
- poutcome (результат прошлой маркетинговой кампании);
- целевая переменная deposit, которая определяет, согласится ли клиент открыть депозит в банке.

:arrow_up:[к оглавлению](https://github.com/KislyukAnna/sf_data_science/tree/main/Project_4#%D0%BE%D0%B3%D0%BB%D0%B0%D0%B2%D0%BB%D0%B5%D0%BD%D0%B8%D0%B5)

### Этапы работы над проектом

1. Первичная обработка данных
2. Разведывательный анализ данных (EDA)
3. Отбор и преобразование признаков
4. Решение задачи классификации: логистическая регрессия и решающие деревья
5. Решение задачи классификации: ансамбли моделей и построение прогноза

:arrow_up:[к оглавлению](https://github.com/KislyukAnna/sf_data_science/tree/main/Project_4#%D0%BE%D0%B3%D0%BB%D0%B0%D0%B2%D0%BB%D0%B5%D0%BD%D0%B8%D0%B5)

### Результаты:
[ Ноутбук с выполненными заданиями](https://github.com/KislyukAnna/sf_data_science/blob/main/Project_4/Project_4_ML.ipynb)
Реализована задача классификации, на основе соответствующих метрик проведено сравнение эффективности различных моделей. Выявлены признаки с наибольшим влиянием на исход маркетинговой кампании. Обозначены возможные способы дальнейшего улучшения модели машинного обучения.

### Выводы

- Проведена предобработка признаков. Простыми способами (медиана, мода) заменены пропущенные значения. Методом Тьюкки удалены выбросы баланса.
- Проведен разведывательный анализ данных в контексте влияния на целевой признак.
- Проведено кодирование признаков и масштабирование значений. Для соответствия ответам на обучающей платформе не соблюдается порядковое кодирование возрастных групп - фактически они маркируются как несвязанные зависимостью классы (Label Encoder). Не проводилась трансформация признаков к нормальному распределению.
- На основе корреляции Кендалла дана оценка влияния признаков на целевой признак (выбрана из-за очевидного отсутствия связи с целевым признаком по монотонной функции, а также ввиду распределений признаков, отличных от нормальных). С помощью ANOVA F-value (f_classif) для построения моделей отобраны 15 наиболее значимых признаков, отобор в целом соответствует результатам по корреляции Кендалла. Попытка отобрать признаки по взаимной информации (mutual_info_classif, не отображено в данном ноутбуке) показала большое несоответствие с оценкой значимости по корреляции Кендалла.
- Построены простые базовые модели - логистическая регрессия и решающее дерево.
- Построены ансамблевые модели - случайный лес, градиентный бустинг на решающих деревьх, стекинг из деревьев, регрессии и бустинга.
- Реализованы примеры подбора гиперпараметров - поиск по сетке, Tree-tructured Parzen estimator (в Optuna).
- На каждом этапе моделирования оценивались метрики качества классификации. Ансамблевые решения закономерно показывают лучшие значения. Какая либо качественная разница между ансамблевыми моделями на данном датасете не прослеживается. Подбор гиперпараметров модели случайного леса незначительно, на десятые доли процента, улучшил результат.

Задача решена на базовом уровне в соответствии с минимумом требований, необходимых для сдачи проекта. Безусловно остается потенциал по возможному улучшению метрик при более тщательной и творческой обработке признаков, транформации данных, экспериментировании с различными моделями.

:arrow_up:[к оглавлению](https://github.com/KislyukAnna/sf_data_science/tree/main/Project_4#%D0%BE%D0%B3%D0%BB%D0%B0%D0%B2%D0%BB%D0%B5%D0%BD%D0%B8%D0%B5)
