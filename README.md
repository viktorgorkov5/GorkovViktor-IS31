# Ядекс Музыка
## Причина Создания
- Необходим удобный сервис для поиска и прослушивания музыки с рекомендациями для каждого пользователя.
## Функционал
- Прослушивание музыки и подкастов
- Получение персональных рекомендаций
- Поиск и структурирование каталога
- Составление плей-листов и их перенос между аккаунтами и устройствами;
- Прослушивание скачанных треков офлайн
- Сохранение музыки в своей коллекции
## Диаграммы
### Диаграмма классов
![image](https://github.com/user-attachments/assets/7fd62272-9760-407b-8631-f983a922227e)


### Диаграмма Сценария
![image](https://github.com/user-attachments/assets/fa098c90-64b4-42c5-b5ee-c7c24856c15c)

###
Пользователь       Клиентское приложение        Сервер               База данных
     |                        |                     |                       |
     |---- Запрос на воспроизведение трека ---->|                     |                       |
     |                        |                     |                       |
     |                        |---- Запрос на получение информации о треке --->| 
     |                        |                     |                       |
     |                        |                     |---- Запрос на информацию о треке --->| 
     |                        |                     |                       |
     |                        |                     |                       |---- Информация о треке -->|
     |                        |<--- Информация о треке ---|                       |
     |<-- Воспроизведение трека -------------------|                       |
     |                        |                     |                       |
     |                        |---- Запрос на потоковые данные ------------>|                       |
     |                        |                     |                       |
     |                        |                     |                       |
     |                        |<--- Потоковые данные ---|                       |
     |<-- Воспроизведение трека -------------------|                       |
     |                        |                     |                       |

