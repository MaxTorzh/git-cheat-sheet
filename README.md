### **НАВИГАЦИЯ**


1. **pwd** - *(от англ. print working directory, «показать рабочую папку») — покажи, в какой я папке;*

2. **ls** - *(от англ. list directory contents, «отобразить содержимое директории») — покажи файлы и папки в текущей папке;*

3. **ls -a** - *покажи также скрытые файлы и папки, названия которых начинаются с символа **.**;*

4. **cd first-project** - *(от англ. change directory, «сменить директорию») — например, перейди в папку first-project;*

5. **cd first-project/html** - *перейди в папку html, которая находится в папке first-project;*

6. **cd ..** - *перейди на уровень выше, в родительскую папку;* 

7. **cd ~** - *перейди в домашнюю директорию (/Users/Username);*

8. **cd /** - *перейди в корневую директорию.*


---


### **РАБОТА С ФАЙЛАМИ И ПАПКАМИ**


##### **Создание**

1. **touch index.html** - (англ. touch, «коснуться») — создай файл index.html в текущей папке;

2. **touch index.html style.css script.js** - *если нужно создать сразу несколько файлов, можно напечатать их имена в одну строку через пробел;*

3. **mkdir second-project** - * (от англ. make directory, «создать директорию») — создай папку с именем second-project в текущей папке.*


---


#### **Копирование и перемещение**

1. **cp file.txt ~/my-dir** - *(от англ. copy, «копировать») — скопируй файл в другое место;*

2. **mv file.txt ~/my-dir** - *(от англ. move, «переместить») — перемести файл или папку в другое место.*


---


#### **Чтение**

1. **cat file.txt** - *(от англ. concatenate and print, «объединить и распечатать») — распечатай содержимое текстового файла file.txt.*


---


#### **Удаление**

1. **rm about.html** - *(от англ. remove, «удалить») — удали файл about.html;*

2. **rmdir images** - * (от англ. remove directory, «удалить директорию») — удали папку images;*

3. **rm -r second-project** - *(от англ. remove, «удалить» + recursive, «рекурсивный») — удали папку second-project и всё, что она содержит.*


---


### **ПОЛЕЗНЫЕ ВОЗМОЖНОСТИ**

1. *Команды необязательно печатать и выполнять по очереди. Можно указать их списком — разделить двумя амперсандами **(&&)**.*

2. *У консоли есть собственная память — буфер с несколькими последними командами. По ним можно перемещаться с помощью клавиш со стрелками вверх **(↑)** и вниз **(↓)**.*

3. *Чтобы не вводить название файла или папки полностью, можно набрать первые символы имени и дважды нажать **Tab**. Если файл или папка есть в текущей директории, командная строка допишет путь сама.*

#### *💡 Например, вы находитесь в папке dev. Начните вводить cd first и дважды нажмите **Tab**. Если папка first-project есть внутри dev, командная строка автоматически подставит её имя. Останется только нажать **Enter**.* 


---


### **ИНИЦИАЛИЗАЦИЯ РЕПОЗИТОРИЯ**

1. **git init** - *(от англ. initialize, «инициализировать») — инициализируй репозиторий.* 


---


### **ПОДГОТОВКА ФАЙЛА К КОММИТУ**

1. **git add todo.txt** - *(от англ. add, «добавить») — подготовь файл todo.txt к коммиту;* 

2. **git add --all** - *(от англ. add, «добавить» + all, «всё») — подготовь к коммиту сразу все файлы, в которых были изменения, и все новые файлы;*

3. **git add .** - *подготовь к коммиту текущую папку и все файлы в ней.* 


---


### **СОЗДАНИЕ КОММИТА**

1. **git commit -m "Комментарий к коммиту."** - *(от англ. commit, «совершать», «фиксировать» + message, «сообщение») — сделай коммит и оставь комментарий, чтобы было проще понять, какие изменения внесены.*


---


### **ПРОСМОТР ИНФОРМАЦИИ О КОММИТАХ**

1. **git log** - *(от англ. log, «журнал [записей]») — выведи подробную историю коммитов.*


---


### **ПРОСМОТР СОСТОЯНИЯ файлов**

1. **git status** - *(от англ. status, «статус», «состояние») — покажи текущее состояние репозитория.*


---


### **СИНХРОНИЗАЦИЯ ЛОКАЛЬНОГО И УДАЛЁННОГО РЕПОЗИТОРИЕВ**

1. **git remote add origin https://github.com/YandexPracticum/first-project.git** - *(от англ. remote, «удалённый» + add, «добавить») — привяжи локальный репозиторий к удалённому с URL https://github.com/YandexPracticum/first-project.git;*

2. **git remote -v** - *(от англ. verbose, «подробный») — проверь, что репозитории действительно связались;*

3. **git push -u origin main** - *(от англ. push, «толкать») — в первый раз загрузи все коммиты из локального репозитория в удалённый с названием origin.*

#### *💡 Ваша ветка может называться master, а не main. Подправьте команду, если это необходимо.*

4. **git push** - *(от англ. push, «толкать») — загрузи коммиты в удалённый репозиторий после того, как он был привязан с помощью флага **-u**.*


---


### **КОПИРОВАНИЕ ЧУЖИХ РЕПОЗИТОРИЕВ**

#### **Клонирование**

1. **git clone git@github.com:TheGreatOwner/the-great-project.git** - *(от англ. clone, «клон», «копия») — склонируй репозиторий с URL the-great-project.git из аккаунта TheGreatOwner на мой локальный компьютер.*


---


#### **«ФОРК»**

1. *«Форк» — операция, которая не связана с Git напрямую и выполняется через графический интерфейс GitHub (кнопка Fork в правом верхнем углу страницы репозитория). «Форк» создаёт независимую копию репозитория со всеми файлами, коммитами и ветками в аккаунте GitHub. Такая копия будет полностью независима. Внесённые изменения не будут синхронизированы с исходным репозиторием.*

#### *💡 Комбинацию «форк» + clone часто используют для внесения изменений в публичные репозитории. В этом случае «форк» становится подготовительным этапом перед клонированием чужого репозитория на локальный компьютер.Если репозиторий приватный или это репозиторий вашей компании, при работе с ним достаточно clone.*


---


### **SSH-КЛЮЧИ**

1. *Протокол SSH обеспечивает безопасный обмен данными в сети. С его помощью можно получать данные с удалённого компьютера или отправлять их на него. Трафик шифруется, поэтому протокол безопасен.*

2. *SSH-ключ состоит из двух частей — публичной и приватной. Приватный ключ хранится только на вашем компьютере и не должен передаваться кому-либо ещё. Он используется для расшифровки данных. Публичный ключ доступен всем и используется для шифрования данных. Они могут быть расшифрованы парным приватным ключом.*

3. *Файл с расширением **.pub** содержит публичный ключ, им можно делиться с веб-сайтами или коллегами. Файл без расширения **.pub** — приватный.*

4. *Прежде чем генерировать новую пару ключей, следует убедиться, что они отсутствуют на вашем компьютере. Проверить это можно командой **ls -la .ssh/** в домашней директории. Если ключи отсутствуют, создать их можно командой **ssh-keygen** в директории **~/.ssh.** После генерации ключ нужно привязать к GitHub.*