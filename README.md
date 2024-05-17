# Транскрибация видео в текст
![Лого](https://timeweb.com/ru/community/article/a1/a179096fabed2b3a361f52471f1ed1a5.jpg)

# Обзор и актуальность 
Транскрибация — перевод данных из видеоформата в текст. Такое решение используют, когда необходимо качественное распознавание слов в потоке речи и создание текстовой расшифровки.
Прочитать текст по диагонали быстрее и эффективнее, чем переслушивать часовую запись конференции или интервью. Но подготовка протокола встречи тоже требует времени. Ускорить процесс позволит данное приложение, основаное на модели OPEN AI WHISPER, которое обучено осуществять перевод видео в текстовый формат. 

# Сферы применения транскрибации

### В обучении:
В сфере онлайн-образования сервисы для расшифровки используют для создания текстовой версии видеоуроков. Некоторые ученики лучше воспринимают информацию визуально, чем на слух. Также программы для транскрибации нужны и в офлайн-образовании. Речь преподавателя на семинаре или конференции можно записать, а потом расшифровать автоматически, чтобы не тратить много времени. Научным сотрудникам такие сервисы нужны, чтобы переводить в текст видеоархивы — они становятся основой для монографий и статей.

### В работе:
Перевод в текст записей встреч и конференций. Иногда важно зафиксировать выступления коллег на собраниях: подвести итоги, распределить задачи, записать идеи. Чтобы сотрудники не отвлекались на записи во время встречи и не тратили рабочее время на расшифровку, используются сервисы транскрибации.

### В бизнесе:
Расшифровка интервью с клиентами в рамках исследований. Текстовая расшифровка позволяет сохранять результаты глубинных интервью в доступном виде. Благодаря транскрипции можно не переслушивать старые записи, а быстро находить нужные фрагменты с помощью поиска по тексту и делиться материалами с коллегами.

 ***
# Иструкция по запуску приложения 

> [!NOTE]
> Приложение доступно для запуска в облаке Streamlit Cloud: [Open app](https://video-to-text-demo-app.streamlit.app/ "video-to-text-demo-app")

 ***

### Для локального запуска необходимо установить:

```
pip install -r requirements.txt
```
### Также требуется установить в системе инструмент ffmpeg, который доступен в менеджерах пакетов:

```
# on Ubuntu or Debian
sudo apt update && sudo apt install ffmpeg
```
```
# on Arch Linux
sudo pacman -S ffmpeg
```
```
# on MacOS using Homebrew (https://brew.sh/)
brew install ffmpeg
```
```
# on Windows using Chocolatey (https://chocolatey.org/)
choco install ffmpeg
(Слетует открывать командную строку с правами администратора, иначе не установится и ничего работать не будет)
```
```
# on Windows using Scoop (https://scoop.sh/)
scoop install ffmpeg
```
### Запуск проекта:
```
streamlit run /main.py
```
 ***

# Инструкция по работе с приложением

1. На главной странице приложения нажать "Browse files":
![Скрин прило](https://github.com/xobivan/Video-to-text-demo-app/assets/153428984/e0c1e7ee-c6cb-4d33-8857-6a371a1d508f)
2. Выбрать видео файл в формате .mp4 из накомителя Вашего ПК и нажать "Открыть":
![Выбор файла](https://github.com/xobivan/Video-to-text-demo-app/assets/153428984/9c3d395a-6125-4c1d-9459-b3f4be1300ae)
3. Дождаться загрузки видео на платформу:
![Загрузка файла](https://github.com/xobivan/Video-to-text-demo-app/assets/153428984/b6248afe-856c-4918-b443-971aa90d1ca7)
4. В поле ниже автоматически сформируется транскрибация из загруженого видео.

 ***

# Команда проекта:

1. Спивак Д. В.
2. Надеждин М. А.
3. Абкадыров Э. П.
4. Тимонин И. Л.
5. Колегов В. С.

 ***

# Идеи по улучшению и развитию проекта 

1. Предоставить пользователю возможность настроить параметры модели суммирования (например, max_length, num_beams и т.д.) через интерфейс.
2. Добавить обработку исключений и логирование для лучшей диагностики и устранения ошибок.
3. Перенести вычислительные задачи на более мощные серверы или использовать облачные сервисы для масштабирования.
4. Реализовать поддержку других языков для транскрипции и суммирования, используя соответствующие модели.














