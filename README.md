# practicum-projects
Учебные проекты, выполненные на курсе **Специалист по Data Science** (Yandex Practicum)

## [Рекомендация тарифов для оператора мобильной связи](https://github.com/mayarosl/practicum-projects/blob/main/telecom_recommentations.ipynb)
**Задача:** построить систему, способную проанализировать поведение абонентов и предложить им новый тариф.  
**Данные:** записи о повелении абонентов, которые уже перешли на эти тарифы.

В проекте построено несколько моделей для задачи классификации, которые выбирают подходящий тариф. Выбрана модель с максимально большим значением *accuracy*.


## [Выбор локации для скважины](https://github.com/mayarosl/practicum-projects/blob/main/well-location.ipynb)
Добывающей компании «ГлавРосГосНефть» нужно решить, где бурить новую скважину. **Задачи**: (1) построить модель машинного обучения, которая поможет определить регион, где добыча принесёт наибольшую прибыль, (2) проанализировать возможную прибыль и риски техникой Bootstrap.
**Данные**: пробы нефти в трёх регионах: в каждом 10 000 месторождений с измерениями качества нефти и объёма её запасов.

На основании предоставленных данных построены модели для рассчета объемов сырья в скважинах в трех регионах. Рассчитан средний запас сырья в каждом регионе.
Методом Bootstrap выбраны 500 случайных скважин из всех скважин региона, из этих 500 взяты 200 самых богатых сырьем и по ним рассчитаны прибыль и убытки. В результате выбран самый подходящий для разработки регион.

## [Определение стоимости автомобилей](https://github.com/mayarosl/practicum-projects/blob/main/vehicle_price.ipynb)
Сервис по продаже автомобилей с пробегом разрабатывает приложение, в котором можно быстро узнать рыночную стоимость своего автомобиля. **Задача**: построить модель для определения стоимости автомобиля по историческим **данным**: техническим характеристикам, комплектациям и ценам автомобилей.

Было обучено три модели: Линейная регрессия, Случайный лес и LightGBM. Лучше всего себя показала LightGBM. При количестве итераций = 200 ее RMSE ниже, чем у леса, обучение и предсказание занимают 13 и 0.9 секунд соответственно. При этом можно уменьшить время предсказания, если сократить количество итераций.

## [Прогнозирование заказов такси]()
**Задача**: спрогнозировать количество заказов такси на следующий час, чтобы привлекать больше водителей в период пиковой нагрузки, на основании исторических **данных** о заказах такси в аэропортах. Построить модель для такого предсказания.

В данные были добавлены новые признаки. Выяснилось, что лучшие резлуьтаты RMSE достигаются при использовании градиентного бустинга.

## [Классификация токсичных комментариев]()
