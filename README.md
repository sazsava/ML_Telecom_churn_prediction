# Прогнозирование оттока клиентов телекоммуникационной комании

*Курсовая работа по начальному машинному обучению*

***Machine learning***

***
<img src="https://img.freepik.com/premium-vector/discontent-concept-set-dissatisfaction-product-service-negative_277904-20252.jpg?w=1380" width="759" height="293" />

## 1.1. Задача
***
Проанализировать данные телекоммуникационной компании и спрогнозировать отток пользователей (выявить людей, которые продлят контракт и которые не продлят).
<br>
В ходе работы было выполнено следующее: 
1. Данные очищены и обработаны для дальнейшего использования.
1. Произведено описание данных с расчетом ряда базовых статистик и построением простых графиков.
2. На основании анализа графических данных были выявлены показатели, наибольшим образом влияющие на отток пользователей.
3. Построены модели для прогнозирования оттока на основе проверенных гипотез и выявленных взаимосвязей. 
4. Было произведено сравнение качества полученных моделей.
5. Были предприняты попытки улучшения качества преджсказания с помощью GridSearch, а также построения ансамблей моделей.
6. Выявлена лучшая модель для указанной цели, сделаны выводы по итогам работы.

## 1.2. Набор данных
***
Данные можно скачать по ссылке:
[Ссылка на Google Drive](https://drive.google.com/file/d/1dPCG76ST6NohYKtVMGv6HpFL-jD5p1eJ/view)
***
telecom_users.csv содержит следующие значения:
- customerID – id клиента
- gender – пол клиента (male/female)
- SeniorCitizen – яляется ли клиент пенсионером (1, 0)
- Partner – состоит ли клиент в браке (Yes, No)
- Dependents – есть ли у клиента иждивенцы (Yes, No)
- tenure – сколько месяцев человек являлся клиентом компании
- PhoneService – подключена ли услуга телефонной связи (Yes, No)
- MultipleLines – подключены ли несколько телефонных линий (Yes, No, No phone service)
- InternetService – интернет-провайдер клиента (DSL, Fiber optic, No)
- OnlineSecurity – подключена ли услуга онлайн-безопасности (Yes, No, No internet service)
- OnlineBackup – подключена ли услуга online backup (Yes, No, No internet service)
- DeviceProtection – есть ли у клиента страховка оборудования (Yes, No, No internet service)
- TechSupport – подключена ли услуга технической поддержки (Yes, No, No internet service)
- StreamingTV – подключена ли услуга стримингового телевидения (Yes, No, No internet service)
- StreamingMovies – подключена ли услуга стримингового кинотеатра (Yes, No, No internet service)
- Contract – тип контракта клиента (Month-to-month, One year, Two year)
- PaperlessBilling – пользуется ли клиент безбумажным биллингом (Yes, No)
- PaymentMethod – метод оплаты (Electronic check, Mailed check, Bank transfer (automatic), Credit card (automatic))
- MonthlyCharges – месячный размер оплаты на настоящий момент
- TotalCharges – общая сумма, которую клиент заплатил за услуги за все время
- Churn – произошел ли отток (Yes or No)
