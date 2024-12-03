![29](https://github.com/user-attachments/assets/d57c90de-972c-4dd8-9a0b-9717e8dcc990)# Практика 3
## Беляев Степан Константинович
## ББМО-02-23

### Начало
#### 2 ВМ
Работа была выполнена на 2 виртуальных машинах на базе ОС Ubuntu, client и server
![1](https://github.com/user-attachments/assets/ec56e78e-5801-4528-90c1-21eaf8e7d15f)

#### Сетевой обмен
На виртуальных машинах был настроен сетевой мост
![3](https://github.com/user-attachments/assets/f146d885-381e-49ec-b196-05630dbadb12)
![2](https://github.com/user-attachments/assets/1d8549bb-eaeb-4086-9005-24f7010b6567)

Проверка "видимости" ВМ друг для друга
![4](https://github.com/user-attachments/assets/8c9793ea-7834-4e61-9070-2ec6773c58d0)
![5](https://github.com/user-attachments/assets/dcfcca07-08b6-45c8-9ddf-9e5a33c457d0)

### Разворачивание сервера Wazuh
В ходе подготовки и разворачивания сервера были предприняты следующие шаги:
- Установка mc для удобства при редактировании текстовых файлов
- Обновление списка пакетов и установка новых
- Выполнили установку на версии 4.9

Полученные после завершения установки логин и пароль от кабинета
![6](https://github.com/user-attachments/assets/4f8e0039-0d7d-4f1b-be10-8ec3e83a5af1)

Старотовый экран Wazuh без подключенного "агента"
![7](https://github.com/user-attachments/assets/fd932f39-8448-42ab-8f38-3ca351b673b3)

Экран Wazuh после подключения "агента"
![8](https://github.com/user-attachments/assets/363a59a3-6aa0-4964-81dc-06b213e0fd60)

Возможности про проверке "агента"
![9](https://github.com/user-attachments/assets/473af554-777a-4175-9720-d27a8b00aca0)

Результат сканирования уязвимых пакетов у "агента"
![10](https://github.com/user-attachments/assets/69ec5951-dded-46f7-a8bc-d74b4a230911)

### Проверка целостности файлов

Результат проверки целостности файлов
![11](https://github.com/user-attachments/assets/5db4826a-2e04-4425-99e5-7d2a0e45536a)

В ходе выполнения задания были предприняты следующие шаги:
- Установили с какой переодинчостью будет проверяться содержимое директории "*/test"
- Создавали, редактивровали и удаляли файлы

### Выявление уязвимостей в соотстветвии с документацияей

Внесенные в conf файл изменения
![12](https://github.com/user-attachments/assets/d7bdb7f2-8c19-4faf-82fb-8389a3d4497f)

Выявление уязвимостей пакетов на клиенте ("агенте")
![14](https://github.com/user-attachments/assets/3aff54fb-47eb-4478-aff5-de3a0bd6a424)

### Выявление скрытых процессов

Изменение в conf файле
![15](https://github.com/user-attachments/assets/153e6f7c-edde-4e06-a2a5-660490ded9ec)

Используя документацию для Wazuh собираем сборку для создаания аномалий. В результате Wazuh отобразит следующее после применения некоторых фильтров:
![16](https://github.com/user-attachments/assets/3d22dff7-d270-407d-ba60-67111aef4eba)

### Наcтрока выявления SQL-инъекций

Проверка статуса Apache посл его установки и настройки
![17](https://github.com/user-attachments/assets/4bda0088-ac10-4229-9473-be47e7e505a1)

Редактирование conf файла
![18](https://github.com/user-attachments/assets/b6e491ce-ea8c-4567-a224-a0bfa103bdb3)

Выявленные Wazuh аномалии
![29](https://github.com/user-attachments/assets/2eac4d44-df22-400d-acf8-2d2330096fb2)

### Выявление web shell attack

Редактирование conf файла
![19](https://github.com/user-attachments/assets/f6593c38-ed00-46ab-890c-2a270597cc39)

Правила для обнаружения модификации файлов
![20](https://github.com/user-attachments/assets/90978f4f-b7ce-4fde-8b77-cceae79fe52c)

Проверка целостности в conf файле
![21](https://github.com/user-attachments/assets/3b207c70-e846-46d0-a922-7ee915b2198b)

Просмотр id после перезапуска "агента"
![22](https://github.com/user-attachments/assets/7a1a612e-e42f-4959-bdbc-a0005a079f62)

Редактирование правил с указанием id полученного на прошлом шаге
![23](https://github.com/user-attachments/assets/2cf6f2bb-4d95-46a3-86e7-f4a69a53e02e)

Работа с conf файлами
![24](https://github.com/user-attachments/assets/de6e636f-5fd4-491d-945b-63324218b476)
![25](https://github.com/user-attachments/assets/13ffe3d3-f92d-47d4-835c-8a66f02b63c3)
![26](https://github.com/user-attachments/assets/3c1ccefd-0113-41f0-a9db-c05972604941)

Подготовка необходимого для "атаки"
![27](https://github.com/user-attachments/assets/1101ae8d-54a9-4215-b902-3a425ae56139)
![28](https://github.com/user-attachments/assets/093311a7-8c2f-489c-8c0d-d4d788ffbfdf)

Выявленные аномалии
![30](https://github.com/user-attachments/assets/52ae3a4c-247f-4db3-b013-2c982e700a0d)

В результате выполнения практической работы №3 по использованию Wazuh были выполнены следующие задачи:

- Развертывание виртуальных машин;
- Использовались VirtualBox и Ubuntu Server для развертывания;
- Настройка сетевого обмена между виртуальными машинами с использованием документации VirtualBox;
- Развертывание сервера Wazuh на одной из машин;
- Подключение агента;
- Анализ обнаруженных уязвимостей;
- Изучение предлагаемых пунктов меню сканирования;
- Создание проверки целостности файлов;
- Настройка выявления уязвимостей;
- Настройка выявления скрытых процессов;
- Настройка выявления SQL- инъекций;
- Настройка выявления web shell attack;
- Демонстрация работы настроенных механизмов;

Все выявленные Wazuh аномалии в ходе выполнения работы
![31](https://github.com/user-attachments/assets/96ec1c62-fe01-4ef7-938c-8760c8f0b8a4)
























