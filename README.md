# Проект парсинга pep

# Склонируйте репозиторий

git clone git@github.com:AMDisplay/bs4_parser_pep.git

# Установите виртуальное окружение 

python -m venv venv

### Обновите pip

python -m pip install pip --upgrade

### Установите зависимости

pip install -r requirements.txt

### Перейдите в директорию src

cd /src

### Запустите парсер

python main.py [вид парсинга] [аргументы]

## Виды парсинга

* whats new
Выводит список изменений в python

python main.py whats-new [аргументы]

* latest_version
Выводит список версий python и ссылки на документацию

python main.py latest-version [аргументы]

* download
Скачивает и упаковывает в zip архив документацию python в pdf формате

python main.py download [аргументы]

* pep
Выводит список статусов документов pep и количество документов в каждом статусе

pyton main.py pep [аргументы]

## Аргументы

* -h, --help Общая информация о командах.

* -c, --clear-cache Очистка кеша перед выполнением парсинга.

* -o {pretty,file}, --output {pretty,file}
    Дополнительные способы вывода данных
    pretty - выводит данные в командной строке в таблице
    file - сохраняет информацию в формате csv в папке ./results/