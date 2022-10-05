Задание № 1 Вам даны результаты проверки двух препаратов.
Требуется:
Оценить, есть ли различие в эффекте у этих пациентов?
Визуально подтвердить результат
A - результаты для группы людей получающих препарат А.
B - результаты для другой группы людей, получающих препарат B.
np.random.seed(11)
A = stats.norm.rvs(scale=30, loc=11, size=100)
B = A + stats.norm.rvs(scale=54, loc=11, size=100)

Задание № 2 Вам даны результаты проверки двух препаратов.
Требуется:
Оценить, есть ли различие в эффекте у этих пациентов?
Визуально подтвердить результат
А - группа людей без препарата.
B - та же группа людей, но получающая препарат
np.random.seed(11)
A = stats.norm.rvs(scale=30, loc=11, size=100)
B = A + stats.norm.rvs(scale=54, loc=11, size=100)

Задание № 3 Допустим вы решили устроить дачный эксперимент. Берем и поливаем одни огурцы водой, другие огурцы водой с удобнением, третью группу огурцов будем поливать минералкой.
Используя дисперсионный анализ, сделайте выводы о распредлениях результатов. Есть ли эффект от удобрения по сравнению с минералкой?
Помимо результата статистического теста, продемонстрируйте отличия визуально с помощью boxplot или hist
water = [1, 2, 3, 4, 2, 4, 2, 4, 5, 2, 3, 4, 2, 1, 3, 4, 3, 2, 5, 1]
nutri = [1, 2, 4, 6, 5, 6, 7, 5, 4, 5, 6, 7, 4, 3, 5, 5, 6, 5, 4, 3, 5]
mineral = [2, 1, 1, 3, 2, 4, 2, 4, 5, 4, 3, 2, 3, 2, 3, 1, 3, 4, 5, 1, 4]

Описание набора данных
Профессор Оук скопировал все содержимое память одного устройства Pokedex, в результате чего получился набор данных, с которым Вы будете работать в этой задаче. В этом файле каждая строка представляет характеристики одного покемона:
pid: Numeric - ID покемона
HP: Numeric - Очки здоровья
Attack: Numeric - Сила обычной атаки
Defense: Numeric - Сила обычной защиты
Sp. Atk: Numeric - Сила специальной атаки
Sp. Def: Numeric - Сила специальной защиты
Speed: Numeric - Скорость движений
Legendary: Boolean - «True», если покемон редкий
Class 1: Categorical - Класс покемона
Class 2: Categorical - Класс покемона

Задание № 1:
Профессор Оук подозревает, что покемоны в классе grass имеют более сильную обычную атаку, чем у покемонов в классе rock. Проверьте, прав ли он, и убедите его в своем выводе статистически.
Примечание: если есть покемоны, которые относятся к обоим классам, просто выбросьте их;
Вы можете предположить, что распределение обычных атак является нормальным для всех классов покемонов.

Задание № 2:
Профессор Оук уже долго не может спать по ночам ведь его волнует вопрос, а правда, что покемоны что покемоны в классе Water в среднем более быстрые, чем покемоны в классе Normal.
Проверьте, прав ли он, и убедите его в своем выводе статистически.
Примечание: если есть покемоны относятся к обоим классам, выбросьте их;
Вы можете предположить, что распределение скорости движения является нормальным для всех классов покемонов.

Задание № 3:
Профессор Оук тот еще безумец. Он изобрел сыворотку, способную ускорить покемона. Однако, мы усомнились в эффективности его вакцины. Професоор дал эту сыворотку следующим покемонам: смотри массив treathed_pokemon. Проверьте, работает ли вообще его сыворотка, убедите всех в своем выводе статистически.
Вы можете предположить, что распределение скорости движения является нормальным для всех классов покемонов.

Задание № 4:
Профессор Оук тот еще безумец. Он изобрел сыворотку, способную ускорить покемона. Однако, мы усомнились в эффективности его вакцины. Професоор дал эту сыворотку следующим покемонам: смотри массив treathed_pokemon. Проверьте, работает ли вообще его сыворотка, убедите всех в своем выводе статистически.
Вы можете предположить, что распределение скорости движения является нормальным для всех классов покемонов.

Задание № 5:
Профессор Оук всегда любил истории про легендарных покемонов. Однако, профессор не очень уверен, что они самые лучшие относительно остальных покемонов. Оук предложил разобраться в этом нам. Проверьте, действительно ли сумма характеристик HP,Attack,Defense у легендарных покемонов выше, чем у других покемонов? А произведение этих же параметров?? Найдите ответы на эти вопросы и убедите всех в своем выводе статистически.
Вы можете предположить, что распределение сум и произведений этих параметров является нормальным для всех классов покемонов.

Задание № 6:
Профессор Оук частенько наблюдает за боями покемонов. После очередных таких боев Оук выделил три класса best_defence_class, которые на его взгляд одинаковы по "силе обычной защиты" Defense. Проверьте, действительно ли эти классы покемонов не отличаются по уровню защиты статистически значимо? Все та же статистика вам в помощь!
Вы можете предположить, что распределение сум и произведений этих параметров является нормальным для всех классов покемонов.
