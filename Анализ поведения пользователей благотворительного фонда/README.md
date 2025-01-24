## **Суть проекта. Описание данных. Этапы работы**

Для исследования были представлены данные о пользователях, в том числе их гендере, регионе проживания, дате регистрации, подписке. 
Так же имеющиеся данные содержат информацию об их пожертвованиях фонду, дате, стоимости и названии продукта. 
Помимо этого получена информация о пользователях, сотрудничающих с фондом уже длительное время, а так же данные о каналах привлечения пользователей.

### **Цель исследования:**
Определить портрет пользователя в целом. Выявить особенности поведения исторических пользователей и новых отдельно. Рассчитать пользовательские, 
маркетинговые и коммерческие метрики. Провести RFM-анализ и описать полученные сегменты. Определить эффективность каналов привлечения пользователей. 
Дать общие выводы и практические рекомендации опираясь на результаты анализа.

### **Описание данных:**
**Файл donor_id.csv (информация о донорах):**

<li>
CustomerCustomFieldsRecurrent	- рекуррент да / нет;
<li>
CustomerCustomFieldsVolunteer	- волонтер да / нет;
<li>
CustomerSex	- пол пользователя;
<li>
CustomerAreaIdsExternalId -	идентификатор региона пользователя;
<li>
CustomerAreaName -	название региона пользователя;
<li>
CustomerIanaTimeZone -	часовой пояс пользователя;
<li>
CustomerTimeZoneSource -	источник данных о часовом поясе;
<li>
CustomerIdsMindboxId -	идентификатор пользователя;
<li>
CustomerIsEmailInvalid - почта невалидна да / нет;
<li>
CustomerChangeDateTimeUtc -	дата регистрации / редактирования;
<li>
CustomerCustomerSubscriptions DobroaifIsSubscribed -	подписка;
<li>
CustomerCustomerSubscriptions DobroaifSmsIsSubscribed -	подписка в точке контакта SMS;
<li>
CustomerCustomerSubscriptions DobroaifEmailIsSubscribed -	подписка в точке контакта email;
<li>
CustomerCustomerSubscriptions DobroaifViberIsSubscribed	- подписка в точке контакта Viber;
<li>
CustomerCustomerSubscriptions;
<li>
CustomerCustomerDobroaifMobilePushIsSubscribed - подписка в точке контакта Mobile Push;
<li>
CustomerCustomerSubscriptions;
<li>
CustomerCustomerDobroaifWebPushIsSubscribed -	подписка в точке контакта Web Push

**Файл order.csv (информация о пожертвованиях):**

<li>
OrderIdsMindboxId - идентификатор платежа;
<li>
OrderFirstActionIdsMindboxId - идентификатор действия;
<li>
OrderFirstActionDateTimeUtc -	дата и время оформления заказа;
<li>
OrderFirstActionChannelIdsMindboxId -	идентификатор точки контакта;
<li>
OrderFirstActionChannelIdsExternalId - внешний идентификатор точки контакта;
<li>
OrderFirstActionChannelName -	наименование точки контакта;
<li>
OrderAreaIdsExternalId - идентификатор региона пользователя;
<li>
OrderTransactionIdsExternalId - внешний идентификатор транзакции;
<li>
OrderTotalPrice -	стоимость заказа;
<li>
OrderIdsWebsiteID - идентификатор заказа на сайте;
<li>
OrderCustomFieldsNewyear - наличие поля с новым годом;
<li>
OrderCustomFieldsNextPayDate - дата следующего списания денег;
<li>
OrderCustomFieldsRecurrent - рекурент да / нет;
<li>
OrderCustomFieldsRepayment - повторный платеж;
<li>
OrderLineProductIdsWebsite - идентификатор продукта на сайте;
<li>
OrderLineProductName - название продукта;
<li>
OrderLineQuantity -	количество единиц продукта;
<li>
OrderLineBasePricePerItem -	базовая цена за единицу продукта;
<li>
OrderLinePriceOfLine - итоговая цена;
<li>
OrderLineStatusIdsExternalId - идентификатор статуса позиции заказа;
<li>
OrderCustomerIdsMindboxId -	идентификатор пользователя;

**Файл import.csv (информация об историческом импорте):**

<li>
CustomerActionCustomerIdsMindboxId - идентификатор пользователя

**Файл channels.pkl (информация о каналах привлечения):**

<li>
User_action	- название действия пользователя;
<li>
Action_date	- дата действия пользователя;
<li>
Channel_id	- идентификатор канала (описание в текстовом файле);
<li>
Utm_campaign	- кампания;
<li>
Utm_source	- ресурс;
<li>
Utm_medium	- что-то дублирующееся;
<li>
User_id	- идентификатор пользователя;
<li>
Action_time	- час действия пользователя;

### **Этапы анализа:**

<li>
загрузка данных;
<li>
предобработка данных. Подготовка к анализу;
<li>
исследовательский анализ;
<li>
аналитический блок;
<li>
основные выводы
