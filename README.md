### Курсовой проект

1. Обучить модель прогнозирования дохода человека (больше или меньше 50 тыс.долл.) на основе его личных характеристик
2. Создать rest api сервис, к которому можно будет обращаться для получения прогнозов

Title: База данных UCI взрослых. Предсказать, если доход> или <50 тыс. Долларов США на основе данных переписи

Attributes:

age u (16,Inf] # Person's age
workclass u Private Self-emp-not-inc Self-emp-inc Federal-gov Local-gov State-gov Without-pay Never-worked # Work type
fnlwgt u [-Inf,Inf] # ??
education u Preschool 1st-4th 5th-6th 7th-8th 9th 10th 11th 12th HS-grad Assoc-acdm Assoc-voc Some-college Prof-school Bachelors Masters Doctorate # Education level
educational-num u [0,Inf] #
marital-status u Married-civ-spouse Divorced Never-married Separated Widowed Married-spouse-absent Married-AF-spouse #
occupation u Tech-support Craft-repair Other-service Sales Exec-managerial Prof-specialty Handlers-cleaners Machine-op-inspct Adm-clerical Farming-fishing Transport-moving Priv-house-serv Protective-serv Armed-Forces #
relationship u Wife Own-child Husband Not-in-family Other-relative Unmarried #
race u White Asian-Pac-Islander Amer-Indian-Eskimo Other Black
gender u Female Male #
capital-gain u [0,Inf] #
capital-loss u [0,Inf] #
hours-per-week u [0,168] #
native-country u United-States Cambodia England Puerto-Rico Canada Germany Outlying-US(Guam-USVI-etc) India Japan Greece South China Cuba Iran Honduras Philippines Italy Poland Jamaica Vietnam Mexico Portugal Ireland France Dominican-Republic Laos Ecuador Taiwan Haiti Columbia Hungary Guatemala Nicaragua Scotland Thailand Yugoslavia El-Salvador Trinadad&Tobago Peru Hong Holand-Netherlands #
income u <=50K >50K # Income breakpoint


Целью работы является построение модели прогнозирование дохода пользователя (больше или меньше 50 тыс долл) в зависимости от его личных параметров.

Инструментом моделирования служат различные модели машинного обучения:

линейная регрессия (в т.ч. с регуляризацией если будет необходимо (при высокой автокорреляции));
дерево решений;
случайный лес;
gradient Boosting;
LGBMRegressor;
XGBRegressor... .
Будут рассчитаны различные метрики качества моделей и выбрана наиболее оптимальная.

В качестве проверки будет сделана дополнительная валидационная выборка.

Далее будет построен pipeline и оценено качество модели на дополнительной подвыборке данных.

Далее будет подготовлено api для возмодности удаленной работы с моделью.
