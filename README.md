# Описание
Данный проект - реализация примитивной системы работы склада (WMS) для аптеки. Был разработан в качестве курсовой работы по ООП для РЭУ им. Г.В. Плеханова. Как любой учебной проект, в нем присутствуют идеи нужные только для проверки знаний, и не являющиеся необходимыми в конечном продукте. 

Проект работает с несколькими таблицами, реализованы CRUD функции, поиск по всей таблице, сортировка.

Важно было реализовать формирование отчетов, поддерживаются `DOC`, `XLSX`, `PDF` и печать на бумаге. Были использованы библиотеки `EPPlus`, `Aspose`, `E-Iceblue Spire`. Работает быстро. Из минусов отсутствие печати файлов в бесплатной версии `Spire`. Альтернативой было использование `COM`, но это медленно и требует наличие установленного `MS Office`. [Примеры отчетов](#Reports)

Одним из обязательных критериев сдачи работы было использование `WinForms`. Также в дополнение был выбрана UI-фреймворк - `Bunifu`. `Bunifu` оказался не самым лучшим выбором, из-за постоянно меняющейся системы лицензий и периодически появляющихся багов. [Пользовательский интерфейс](#UI)

Для ведения логов используется `NLog`. Для хеширования паролей используется `Bcrypt`.

# Статус
[![auto-release](https://github.com/dmitrsablin/WMSPharmacyPublic/actions/workflows/build.yml/badge.svg)](https://github.com/dmitrsablin/WMSPharmacyPublic/actions/workflows/build.yml)
[![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2Fdmitrsablin%2FWMSPharmacyPublic.svg?type=shield)](https://app.fossa.com/projects/git%2Bgithub.com%2Fdmitrsablin%2FWMSPharmacyPublic?ref=badge_shield)

# Замечания
1. Для упрощения установки используется установщик `ClickOnce`. Подписи у приложения нет. Приложение можно удалить через панель управления Windows. 

# Инструкция
1.  Скачать [последний релиз](https://github.com/dmitrsablin/WMSPharmacyPublic/releases);
2.  Запустить Setup.exe;
3.  Перейти в настройки на главной странице;
4.  Настроить подключения к SQL Server;
5.  Нажать кнопку ‘Создать БД’.

Логин и пароль по умолчанию: admin/admin

# <a name="UI"></a> Пользовательский интерфейс

### Окно авторизации
![Авторизация](https://user-images.githubusercontent.com/37047275/133948473-1bd879c0-2420-4b27-9491-59d0116eba72.PNG)
### Работа с товарами
![Наименования](https://user-images.githubusercontent.com/37047275/133948488-99c069b1-ac3b-4e02-82b3-f2fcf34b9922.PNG)
### Работа с пользователями
![Пользователи](https://user-images.githubusercontent.com/37047275/133948490-b27385a6-a047-413a-8c73-64a4f5fb1fe8.PNG)
### Работа с настройками
![Все настройки](https://user-images.githubusercontent.com/37047275/133948495-778f4090-5bf4-4d35-863e-7f417bc59b25.PNG)
### Изменение пароля пользователем 
![Смена паролей](https://user-images.githubusercontent.com/37047275/133948499-655e2761-038d-4234-8572-a951380c99cb.PNG)


# <a name="Reports"></a> Примеры отчетов
### Отчет в XLSX
![Отчет в XLSX](https://user-images.githubusercontent.com/37047275/133948453-ffcc16fc-9367-41e1-a7a3-7c33c8c04a2e.PNG)
### Отчет в DOC
![Отчет DOC](https://user-images.githubusercontent.com/37047275/133948455-e1f425ec-ccc0-4f90-9eaf-9af3e4f8b40a.PNG)
### Отчет в PDF
![Отчет PDF](https://user-images.githubusercontent.com/37047275/133948461-76a8f19f-de4b-4aff-b235-a43235a01ef3.PNG)


## License
[![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2Fdmitrsablin%2FWMSPharmacyPublic.svg?type=large)](https://app.fossa.com/projects/git%2Bgithub.com%2Fdmitrsablin%2FWMSPharmacyPublic?ref=badge_large)