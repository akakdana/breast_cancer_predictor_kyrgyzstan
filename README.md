# breast_cancer_predictor_kyrgyzstan

Тема: Медицинский анализ данных для предсказания BIRADS( категория оценки маммографиских снимок): Использование машинного обучения.


О данных

В структуре онкологической заболеваемости в Кыргызской Республике 1 место
занимает рак молочной железы – 18,5 %. В 2020 году зарегистрировано всего
615 новых случаев рака молочной железы. Первое место в структуре смертности
занимает также рак молочной железы (8,9 %). При этой форме рака
запущенными считаются 3 и 4 стадии и их показатели, следующие: 26,5% и 12,4%.
Т.е. 38,9% новых случаев рака молочной железы выявляются на поздних стадиях.

Данные были собраны в рамках проекта «Ранняя диагностика рака молочной железы и рака шейки матки в Кыргызской Республике с использованием передвижного маммографического центра» по инициативе Общественного фонда «Эргэнэ», с целью обеспечения справедливого доступа к ранней диагностике распространенных видов рака у женщин в регионах с применением высокотехнологичных методов.

Целью этого проекта является исследование здоровья женщин на рак
молочной железы, являющегося ведущей причиной заболеваемости и смертности
среди онкозаболеваний в нашей стране.


Анализ данных

Медицинская наука исчерпывающе использует преимущества современных методов обработки данных и машинного обучения для предсказания различных заболеваний и диагностики пациентов. В данной статье представлена работа, в которой мы исследовали методы анализа данных предварительно подготовленного набора данных о женщинах, проходящих маммографию. В данной статье мы сосредоточились на предсказании BIRADS (Breast Imaging Reporting and Data System) по данным анамнезов и маммографических снимков. BIRADS представляет собой систему классификации маммографических результатов, которая помогает врачам стандартизировать и описывать образцы обнаружения изменений в молочных железах.
Перед анализом данных мы провели тщательную очистку, удаление выбросов и заполнение пропущенных значений. Затем мы произвели визуализацию данных с использованием библиотеки Python для более глубокого понимания распределения признаков и зависимостей между ними. 
В данной статье мы использовали визуализацию для выделения ключевых аспектов данных и определения важных признаков, которые могут оказать влияние на предсказание категории BIRADS. Визуализация позволяет наглядно представить структуру данных, выявить закономерности и корреляции между признаками, а также выявить выбросы или аномалии, которые могут повлиять на качество предсказания.
С помощью визуализации мы можем проанализировать взаимосвязи между различными параметрами анамнеза и маммографических снимков с категорией BIRADS. Например, возможно выделить определенные характеристики, которые чаще встречаются у пациентов с разными категориями BIRADS. Это может помочь выявить важные признаки, которые можно использовать для улучшения точности предсказания и помочь врачам принимать более информированные решения.
Использование визуализации в исследовании данных оказывает значительную помощь в понимании структуры данных, выявлении паттернов и сборе инсайтов, которые могут быть использованы для разработки более эффективных моделей предсказания BIRADS и улучшения качества диагностики.


На следующем этапе мы применили несколько моделей машинного обучения, таких как Logistic Regression, Random Forest Classifier, Gradient Boosting Classifier и Cat Boost Classifier. Чтобы получить более объективную оценку производительности моделей, мы применили несколько подходов и методов оценки производительности моделей.
Результаты данного исследования могут быть использованы в медицинской практике для более эффективного и точного диагностирования рака молочной железы у женщин. Однако, для получения более полной картины и применения моделей на практике, рекомендуется провести дополнительные исследования на больших наборах данных и применить модели на новых пациентах для проверки их эффективности в реальных условиях.


О применяемой системе оценки при чтении маммографических снимков

Категории оценки BI-RADS и соответствующие им рекомендации
Категория 0 – неполные данные, невозможно прийти к однозначному выводу
по результатам визуализации, необходимо дообследование. Эта категория
правомерна только при скрининговых обследованиях.
Категория 1 – нормальные результаты маммографии. Нет образований,
нарушений архитектоники или подозрительных кальцинатов.
Категория 2 – безусловно, доброкачественные изменения.
Категория 3 – наиболее вероятно доброкачественное образование (до 98% за
то, что есть доброкачественный процесс), контрольная визуализация изменений
через 6 месяцев – маммография одной молочной железы, при этом категория
остается 3. Далее, при стабильной картине, рекомендована маммография обеих
молочных желез через 12 месяцев. При стабильной картине выявленных
изменений категория изменяется на 2 и контроль назначается через 12 месяцев.
Пограничная категория, динамический контроль по схеме 6-12-12 месяцев.
Категория 4 – выявленные изменения на маммограммах подозрительны на
злокачественный процесс с вероятностью от 2 до 94%:
низкая степень вероятности, от 2 до 10% - BI-RADS 4a;
средняя (умеренная) степень вероятности, от 10 до 50% - BI-RADS 4b;
высокая степень вероятности, от 50 до 95% - BI-RADS 4c.
При присвоении данной категории необходима морфологическая верификация
путем выполнения стереотаксической трепан-биопсии.
Категория 5 – вероятны злокачественные изменения, все выявленные признаки
указывают на наличие рака молочной железы.
Категория 6 – безусловно, злокачественные изменения. Под эту категорию
подпадают пациентки с уже верифицированным диагнозом злокачественный
процесс молочной железы.