# используемый образ (OS) + установленный Python
FROM python:3.12-alpine

# установка библиотек при помощи команды pip3 install
RUN pip3 install Flask-Login
RUN pip3 install Flask-SQLAlchemy

# переместить все что находится в папке, где находится
# данный Dockerfile в указанную директорию контейнера
COPY . /opt/app

# переход на указанную директорию для выполнения след-й команды
WORKDIR /opt/app

# команда, выполняемая при запуске контейнера
CMD [ "python", "./app.py" ]