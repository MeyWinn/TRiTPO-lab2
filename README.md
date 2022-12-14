# TRiTPO-lab2

# Требования к проекту
---
# Содержание
1 [Введение](#intro)                                        
1.1 [Название продукта](#product_name)                    
1.2 [Назначение документа](#appointment)                     
1.3 [Бизнес-требования](#business_requirements)                      
1.3.1 [Исходные данные](#initial_data)  
1.3.2 [Возможности бизнеса](#business_opportunities)  
1.3.3 [Границы проекта](#project_boundary)  
1.4 [Аналоги](#analogues)  
2 [Требования пользователя](#user_requirements)  
2.1 [Программные интерфейсы](#software_interfaces)                        
2.2 [Интерфейс пользователя](#user_interface)  
2.3 [Характеристики пользователей](#user_specifications)  
2.3.1 [Классы пользователей](#user_classes)  
2.3.2 [Аудитория приложения](#application_audience)  
2.3.2.1 [Целевая аудитория](#target_audience)  
2.3.2.2 [Побочная аудитория](#collateral_audience)  
2.4 [Предположения и зависимости](#assumptions_and_dependencies)  
3 [Системные требования](#system_requirements)  
3.1 [Функциональные требования](#functional_requirements)  
3.1.1 [Основные функции](#main_functions)  
3.1.1.1 [Вход пользователя в приложение](#user_logon_to_the_application)  
3.1.1.2 [Настройка профиля зарегистрированного пользователя](#setting_up_the_profile_of_the_active_user)  
3.1.1.3 [Опрос пользователя о своих предпочтениях](#user_asking)  
3.1.1.4 [Просмотр информации об отдельной анкете](#view_information_about_an_individual_anket)  
3.1.1.5 [Выход зарегистрированного пользователя из учётной записи](#active_user_change)  
3.1.1.6 [Регистрация нового пользователя после входа в приложение](#add_new_user)                      
3.1.1.7 [Просмотр товаров](#watch_goods)                      
3.1.1.8 [Покупка товаров](#buy_goods)       
3.1.1.9 [Запроса на добавление нового товара](#buy_goods)   
3.1.2 [Ограничения и исключения](#restrictions_and_exclusions)  
3.2 [Нефункциональные требования](#non-functional_requirements)  
3.2.1 [Атрибуты качества](#quality_attributes)  
3.2.1.1 [Требования к удобству использования](#requirements_for_ease_of_use)  
3.2.1.2 [Требования к безопасности](#security_requirements)  
3.2.2 [Внешние интерфейсы](#external_interfaces)  
3.2.3 [Ограничения](#restrictions)  
# 1 Введение
<a name="intro"/>

## 1.1 Название продукта
<a name="product_name"/>
UStore

## 1.2 Назначение документа
<a name="appointment"/>
В этом документе описаны функциональные и нефункциональные требования к веб-сервису «UStore» для мобильных телефонов.
Этот документ предназначен для команды, которая будет реализовывать и проверять корректность работы веб-сервиса.

## 1.3 Бизнес-требования
<a name="business_requirements"/>

### 1.3.1 Исходные данные
<a name="initial_data"/>
Интернет-магазин — сайт, торгующий товарами посредством сети Интернет. С каждым годом он набирает всё большие обороты.
В первую очередь (для пользователей) интернет-магазин – это место, где можно быстро и легко найти нужные для тебя вещи или продукты и заказать их не вставая с дивана. Также такие сервисы предоставляют доставку заказанных товаров до дома покупателя, что еще больше упрощает покупки.

### 1.3.2 Возможности бизнеса
<a name="business_opportunities"/>
Многие люди желают иметь приложения, позволяющее быстро найти нужный товар и также быстро забрать его у курьера, который привезет эти товары. Подобный сервис позволит им тратить меньше времени на поиск необходимых товаров и использовать сервис в удобное время, чтобы не тратить время на поход в магазин и долгий поиск нужной вещи. Интерфейс, спроектированный с учётом всех особенностей похожих технологий, и дополнение веб-сервиса подробной инструкцией позволят увеличить количество людей, использующих данный сервис.
Подбор рекомендованных товаров будет осуществляться по специальному алгоритму, учитывающему все предыдущие запросы, а также обрабатывая все запросы в других приложениях.

### 1.3.3 Границы проекта
<a name="project_boundary"/>
Веб-сервис "UStore" позволит зарегистрированным пользователям просмотреть каталог магазина, оставлять и читать отзывы под любыми товарами, оставлять свой адрес проживания, для получения доставки на дом, оставлять свой адрес почты, для получения уведомлений о новых скидках и акциях. Так же можно заказать карту постоянного клиента, после 3 покупок, после чего будет предоставлена накопительная скидка, увеличивающаяся после каждой покупки.

## 1.4 Аналоги
<a name="analogues"/>
Wildberries  — популярный модный международный маркетплейс одежды, обуви, электроники, детских товаров, товаров для дома и других товаров. Компания напрямую сотрудничает с производителями одежды и официальными дистрибьюторами. Они самостоятельно формируют ассортимент своих товаров в интернет-магазине и розничные цены, а Wildberries зарабатывает на комиссии по итогам продаж Есть свое приложение для мобильных платформ Android и iOS. Компания частная, принадлежит основателям — семье Бакальчук.

21vek.by  — белорусский интернет-гипермаркет, специализирующийся на продаже электроники и бытовой техники, товаров для дома и т. д. Является одним из лидеров интернет-торговли в Республике Беларусь. Интернет-гипермаркет 21vek.by имеет собственную бонусную программу, участники которой могут частично оплачивать свои покупки накопленными баллами.

### 1.4.1 Отличия от аналогов
В отличие от Wildberries и 21vek.by пользователи веб-сервиса UStore имеют возможность получения персональных накопительных скидок, а также, можно будет отправить запрос, на добавление определенного товара в веб-сервис.

# 2 Требования пользователя
<a name="user_requirements"/>

## 2.1 Программные интерфейсы
<a name="software_interfaces"/>
Веб-сервис использует ресурс MovieBox.dev, созданный для реализации алгоритмов поиска и подборки 
Язык программирования: Java API: Java SE, Java EE 
Фреймворки: Spring, Hibernate, Play, Lombok, Java Media Framework

## 2.2 Интерфейс пользователя
<a name="user_interface"/>

Окно входа в сервис. 

![Окно входа в сервис](https://github.com/MeyWinn/TRiTPO-lab2/blob/main/%D0%A4%D0%BE%D1%82%D0%BE%20%D0%B8%D0%BD%D1%82%D0%B5%D1%80%D1%84%D0%B5%D0%B9%D1%81%D0%B0/%D0%9E%D0%BA%D0%BD%D0%BE%20%D0%B2%D1%85%D0%BE%D0%B4%D0%B0%20%D0%B2%20%D1%81%D0%B5%D1%80%D0%B2%D0%B8%D1%81.jpg)

Окно каталога товаров.

![Окно каталога товаров](https://github.com/MeyWinn/TRiTPO-lab2/blob/main/%D0%A4%D0%BE%D1%82%D0%BE%20%D0%B8%D0%BD%D1%82%D0%B5%D1%80%D1%84%D0%B5%D0%B9%D1%81%D0%B0/%D0%9E%D0%BA%D0%BD%D0%BE%20%D0%BA%D0%B0%D1%82%D0%B0%D0%BB%D0%BE%D0%B3%D0%B0%20%D1%82%D0%BE%D0%B2%D0%B0%D1%80%D0%BE%D0%B2.jpg)
 
Окно регистрации нового пользователя.

![Окно регистрации нового пользователя](https://github.com/MeyWinn/TRiTPO-lab2/blob/main/%D0%A4%D0%BE%D1%82%D0%BE%20%D0%B8%D0%BD%D1%82%D0%B5%D1%80%D1%84%D0%B5%D0%B9%D1%81%D0%B0/%D0%9E%D0%BA%D0%BD%D0%BE%20%D1%80%D0%B5%D0%B3%D0%B8%D1%81%D1%82%D1%80%D0%B0%D1%86%D0%B8%D0%B8%20%D0%BD%D0%BE%D0%B2%D0%BE%D0%B3%D0%BE%20%D0%BF%D0%BE%D0%BB%D1%8C%D0%B7%D0%BE%D0%B2%D0%B0%D1%82%D0%B5%D0%BB%D1%8F.jpg)

Окно после выбора товара.

![Окно после выбора товара](https://github.com/MeyWinn/TRiTPO-lab2/blob/main/%D0%A4%D0%BE%D1%82%D0%BE%20%D0%B8%D0%BD%D1%82%D0%B5%D1%80%D1%84%D0%B5%D0%B9%D1%81%D0%B0/%D0%9E%D0%BA%D0%BD%D0%BE%20%D0%BF%D0%BE%D1%81%D0%BB%D0%B5%20%D0%B2%D1%8B%D0%B1%D0%BE%D1%80%D0%B0%20%D1%82%D0%BE%D0%B2%D0%B0%D1%80%D0%B0.jpg)

Окно корзины товаров.

![Окно корзины товаров](https://github.com/MeyWinn/TRiTPO-lab2/blob/main/%D0%A4%D0%BE%D1%82%D0%BE%20%D0%B8%D0%BD%D1%82%D0%B5%D1%80%D1%84%D0%B5%D0%B9%D1%81%D0%B0/%D0%9E%D0%BA%D0%BD%D0%BE%20%D0%BA%D0%BE%D1%80%D0%B7%D0%B8%D0%BD%D1%8B%20%D1%82%D0%BE%D0%B2%D0%B0%D1%80%D0%BE%D0%B2.jpg)

Окно настроек.

![Окно настроек](https://github.com/MeyWinn/TRiTPO-lab2/blob/main/%D0%A4%D0%BE%D1%82%D0%BE%20%D0%B8%D0%BD%D1%82%D0%B5%D1%80%D1%84%D0%B5%D0%B9%D1%81%D0%B0/%D0%9E%D0%BA%D0%BD%D0%BE%20%D0%BD%D0%B0%D1%81%D1%82%D1%80%D0%BE%D0%B5%D0%BA.jpg)

## 2.3 Характеристики пользователей
<a name="user_specifications"/>

### 2.3.1 Классы пользователей
<a name="user_classes"/>
1)Зарегистрированные пользователи - пользователи, которые зарегестрировались в приложение. Имеют доступ к полному функционалу.
2)Незарегестрированные пользователи - пользователи, которые не зарегестрировались в приложение. Имеют доступ к частичному функционалу.

### 2.3.2 Аудитория приложения
<a name="application_audience"/>

#### 2.3.2.1 Целевая аудитория
<a name="target_audience"/>

Приложение расчитано на совершеннолетних пользователей возрастной категории(14-60) лет, обладающие умением взаимодействовать с телефоном.

#### 2.3.2.2 Побочная аудитория
<a name="collateral_audience"/>

Люди старшей возрастной аудитории, обладающие вышеперечисленными качествами.

### 2.4 Предположения и зависимости
<a name="assumptions_and_dependencies"/>
1. Веб-сервис должен иметь возможность обрабатывать значительное количество запросов в секунду;
2. Допустимое время ответа сервера не должно превышать 2 секунды;
3. На сервисе ожидается большое количество пользователей;
4. Требуется хранить значительное количество информации о товарах.

# 3 Cистемные требования
<a name="system_requirements"/>

## 3.1 Функциональные требования
<a name="functional_requirements"/>

### 3.1.1 Основные функции
<a name="main_functions"/>

#### 3.1.1.1 Вход пользователя в приложение
<a name="user_logon_to_the_application"/>
Описание. Пользователь имеет возможность использовать приложение без создания собственного профиля либо войдя в свою учётную запись.

| Функция | Требования | 
|:---|:---|
| Вход в приложение без создания собственного профиля | Приложение должно предоставить ползователю возможность войти в приложение анонимно |
| Регистрация нового пользователя | Приложение должно запросить у пользователя ввести свою почту, а также никнейм для создания учётной записи. Пользователь должен либо ввести данные, либо отменить действие |
| Пользователь с таким никнеймом (почтой) уже существует | Приложение должно известить пользователя об ошибке регистрации и запросить повторный ввод всех данных. Пользователь должен либо ввести данные, либо отменить действие |
| Вход зарегистрированного пользователя в приложение | Приложение должно предоставить пользователю список никнеймов уже зарегестрированных пользователей. Пользователь должен либо выбрать из списка свой никнейм, либо отменить действие |

#### 3.1.1.2 Настройка профиля зарегистрированного пользователя
<a name="setting_up_the_profile_of_the_active_user"/>
Описание. Зарегистрированный пользователь имеет возможность редактировать свой профиль.

| Функция | Требования | 
|:---|:---|
| Редактирование общей информации о пользователе | Приложение должно предоставить зарегистрированному пользователю поле для ввода общей информации о себе. Пользователь должен либо ввести информацию и подвердить действие, либо отменить его |
| Редактирование адреса доставки по умолчанию | Зарегистрированный пользователь имеет возможножность редактировать адрес доставки по умолчанию |

#### 3.1.1.3 Опрос пользователя о любимых товарах
<a name="user_asking"/>
Описание. Зарегистрированный пользователь имеет возможность указать приложению свои предпочтения, которые в дальнейшем обработаются приложением и используются для отображения рекомендуемых товаров

| Функция | Требования | 
|:---|:---|
| Заполнение анкеты о любимых товарах | Приложение должно предоставить зарегистрированному пользователю поле для ввода информации о любимых товарах. Пользователь должен либо ввести информацию и подвердить действие, либо пропустить его |

#### 3.1.1.4 Просмотр информации об отдельном товаре
<a name="view_information_about_an_individual_anket"/>
Описание. Пользователь имеет возможность просматривать краткую и полную информацию о любом товаре

| Функция | Требования | 
|:---|:---|
| Просмотр предварительной(краткой) информации | Приложение должно предоставить пользователю возможность увидеть краткую информацию о товаре на главной странице |
| Просмотр полной информации | Приложение должно предоставить пользователю возможность увидеть полную информацию о товаре |

#### 3.1.1.5 Выход зарегистрированного пользователя из учетной записи
<a name="active_user_change"/>
Описание. Зарегистрированный пользователь имеет возможность выйти из своего профиля.

Требование. Приложение должно предоставить зарегистрированному пользователю возможность выйти из учётной записи с возвратом к окну входа в приложение.

#### 3.1.1.6 Регистрация нового пользователя после входа в приложение
<a name="add_new_user"/>
Описание. Анонимный пользователь имеет возможность зарегистрироваться в приложении.

Требование. Приложение должно предоставить анонимному пользователю возможность [зарегистрироваться в приложении]

#### 3.1.1.7 Просмотр товаров
<a name="watch_goods"/>
Описание. Зарегистрированный пользователь имеет возможность просматривать товары онлайн

Требование. Приложение должно предоставить анонимному пользователю возможность просмотра товаров онлайн, отобразив графический интерфейс просмотра анкет

#### 3.1.1.8 Покупка товаров
<a name="buy_goods"/>
Описание. Зарегистрированный пользователь имеет возможность купить товары, указав адрес доставки

#### 3.1.1.9 Запрос на добавление нового товара
<a name="new_goods"/>
Описание. Зарегистрированный пользователь имеет возможность подать запрос на добавление нового товара, указав полное описание товара и добавив фотографии данного товара

Требование. Приложение должно предоставить зарегистрированному пользователю возможность отправить запрос на добавление нового товара, отобразив графический интерфейс отправления запроса на добавление нового товара

### 3.1.2 Ограничения и исключения
<a name="restrictions_and_exclusions"/>
1. Приложение работает только при наличии подключения к Интернету;
2. Приложение функционирует корректно только при корректной работе сервиса UStore.dev 

## 3.2 Нефункциональные требования
<a name="non-functional_requirements"/>

### 3.2.1 Атрибуты качества
<a name="quality_attributes"/>

#### 3.2.1.1 Требования к удобству использования
<a name="requirements_for_ease_of_use"/>
1. Доступ к основным функциям приложения не более чем за две операции;
2. Все функциональные элементы пользовательского интерфейса имеют названия, описывающие действие, которое произойдет при выборе элемента;
3. Пошаговая инструкция использования основных функций приложения отображена в справке;
4. Обновление информации о товарах происходит каждые 30 минут в фоновом режиме
5. Понятный графический интерфейс

#### 3.2.1.2 Требования к безопасности
<a name="security_requirements"/>
Приложение предоставляет возможность просмотра и редактирования профиля только активного пользователя.
Приложение гарантирует безопасность личных данных пользователей.

### 3.2.2 Внешние интерфейсы
<a name="external_interfaces"/>
Окна приложения удобны для использования пользователями с плохим зрением:
  * размер шрифта не менее 14пт;
  * функциональные элементы контрастны фону окна.

### 3.2.3 Ограничения
<a name="restrictions"/>
1. Приложение реализовано на платформе Spring Framework 5.3.1; 2;
2. Профиль пользователя хранится в файле с расширением XML, название файла совпадает с никнеймом;
3. Информация о товарах хранится в базе данных MySQL.
4. Приложение не работает при отсутствии подключения к Интернету;
5. Приложение не обрабатывает данные анкет, недоступных в момент запроса;
6. Качество изображения зависит от скорости подключения пользователя.
