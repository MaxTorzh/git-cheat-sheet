### **НАВИГАЦИЯ**


1. **> pwd** - *(от англ. print working directory, «показать рабочую папку») — покажи, в какой я папке;*

2. **> ls** - *(от англ. list directory contents, «отобразить содержимое директории») — покажи файлы и папки в текущей папке;*

3. **> ls -a** - *покажи также скрытые файлы и папки, названия которых начинаются с символа **.**;*

4. **> cd first-project** - *(от англ. change directory, «сменить директорию») — например, перейди в папку first-project;*

5. **> cd first-project/html** - *перейди в папку html, которая находится в папке first-project;*

6. **> cd ..** - *перейди на уровень выше, в родительскую папку;* 

7. **> cd ~** - *перейди в домашнюю директорию (/Users/Username);*

8. **> cd /** - *перейди в корневую директорию.*


---


### **РАБОТА С ФАЙЛАМИ И ПАПКАМИ**


##### **Создание**

1. **> touch index.html** - (англ. touch, «коснуться») — создай файл index.html в текущей папке;

2. **> touch index.html style.css script.js** - *если нужно создать сразу несколько файлов, можно напечатать их имена в одну строку через пробел;*

3. **> mkdir second-project** - * (от англ. make directory, «создать директорию») — создай папку с именем second-project в текущей папке.*


---


#### **Копирование и перемещение**

1. **> cp file.txt ~/my-dir** - *(от англ. copy, «копировать») — скопируй файл в другое место;*

2. **> mv file.txt ~/my-dir** - *(от англ. move, «переместить») — перемести файл или папку в другое место.*


---


#### **Чтение**

1. **> cat file.txt** - *(от англ. concatenate and print, «объединить и распечатать») — распечатай содержимое текстового файла file.txt.*


---


#### **Удаление**

1. **> rm about.html** - *(от англ. remove, «удалить») — удали файл about.html;*

2. **> rmdir images** - * (от англ. remove directory, «удалить директорию») — удали папку images;*

3. **> rm -r second-project** - *(от англ. remove, «удалить» + recursive, «рекурсивный») — удали папку second-project и всё, что она содержит.*


---


### **ПОЛЕЗНЫЕ ВОЗМОЖНОСТИ**

1. *Команды необязательно печатать и выполнять по очереди. Можно указать их списком — разделить двумя амперсандами **(&&)**.*

2. *У консоли есть собственная память — буфер с несколькими последними командами. По ним можно перемещаться с помощью клавиш со стрелками вверх **(↑)** и вниз **(↓)**.*

3. *Чтобы не вводить название файла или папки полностью, можно набрать первые символы имени и дважды нажать **Tab**. Если файл или папка есть в текущей директории, командная строка допишет путь сама.*

#### *💡 Например, вы находитесь в папке dev. Начните вводить cd first и дважды нажмите **Tab**. Если папка first-project есть внутри dev, командная строка автоматически подставит её имя. Останется только нажать **Enter**.* 


---


### **ИНИЦИАЛИЗАЦИЯ РЕПОЗИТОРИЯ**

1. **> git init** - *(от англ. initialize, «инициализировать») — инициализируй репозиторий.* 


---


### **ПОДГОТОВКА ФАЙЛА К КОММИТУ**

1. **> git add todo.txt** - *(от англ. add, «добавить») — подготовь файл todo.txt к коммиту;* 

2. **> git add --all** - *(от англ. add, «добавить» + all, «всё») — подготовь к коммиту сразу все файлы, в которых были изменения, и все новые файлы;*

3. **> git add .** - *подготовь к коммиту текущую папку и все файлы в ней.* 


---


### **СОЗДАНИЕ КОММИТА**

1. **> git commit -m "Комментарий к коммиту."** - *(от англ. commit, «совершать», «фиксировать» + message, «сообщение») — сделай коммит и оставь комментарий, чтобы было проще понять, какие изменения внесены.*


---


### **ПРОСМОТР ИНФОРМАЦИИ О КОММИТАХ**

1. **> git log** - *(от англ. log, «журнал [записей]») — выведи подробную историю коммитов.*


2. **> git log --oneline** - *(от англ. log, «журнал [записей]» + one line, «одной строкой») — покажи краткую информацию о коммитах: сокращённый хеш и сообщение.*


---


### **ПРОСМОТР СОСТОЯНИЯ файлов**

1. **> git status** - *(от англ. status, «статус», «состояние») — покажи текущее состояние репозитория.*


---


### **СИНХРОНИЗАЦИЯ ЛОКАЛЬНОГО И УДАЛЁННОГО РЕПОЗИТОРИЕВ**

1. **> git remote add origin https://github.com/YandexPracticum/first-project.git** - *(от англ. remote, «удалённый» + add, «добавить») — привяжи локальный репозиторий к удалённому с URL https://github.com/YandexPracticum/first-project.git;*

2. **> git remote -v** - *(от англ. verbose, «подробный») — проверь, что репозитории действительно связались;*

3. **> git push -u origin main** - *(от англ. push, «толкать») — в первый раз загрузи все коммиты из локального репозитория в удалённый с названием origin.*

#### *💡 Ваша ветка может называться master, а не main. Подправьте команду, если это необходимо.*

4. **> git push** - *(от англ. push, «толкать») — загрузи коммиты в удалённый репозиторий после того, как он был привязан с помощью флага **-u**.*


---


### **КОПИРОВАНИЕ ЧУЖИХ РЕПОЗИТОРИЕВ**

#### **Клонирование**

1. **> git clone git@github.com:TheGreatOwner/the-great-project.git** - *(от англ. clone, «клон», «копия») — склонируй репозиторий с URL the-great-project.git из аккаунта TheGreatOwner на мой локальный компьютер.*


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


---


### **ДОБАВЛЕНИЕ ИЗМЕНЕНИЙ В ПОСЛЕДНИЙ КОММИТ**

1. **> git commit --amend --no-edit** - *(от англ. amend, «исправить») — добавь изменения к последнему коммиту и оставь сообщение прежним;*

2. **> git commit --amend -m** - *"Новое сообщение" — измени сообщение к последнему коммиту на Новое сообщение.*

#### *💡 Выйти из редактора Vim: нажать Esc, ввести :qa!, нажать Enter.*


---

### **«ОТКАТ» ФАЙЛОВ И КОММИТОВ**

1. **> git restore --staged hello.txt** - *(от англ. restore, «восстановить») — переведи файл hello.txt из состояния staged обратно в untracked или modified.*

2. **> git restore hello.txt** - *верни файл hello.txt к последней версии, которая была сохранена через git commit или git add.*

3. **> git reset --hard b576d89** - *(от англ. reset, «сброс», «обнуление» + hard, «суровый») — удали все незакоммиченные изменения из staging и «рабочей зоны» вплоть до указанного коммита.*


---


### **ПРОСМОТР ИЗМЕНЕНИЙ**

1. **> git diff** - *(от англ. difference, «отличие», «разница») — покажи изменения в «рабочей зоне», то есть в modified-файлах.*

2. **> git diff a9928ab 11bada1** - *выведи разницу между двумя коммитами.*

3. **> git diff --staged** - *покажи изменения, которые добавлены в staged-файлах.*


---


### **СОЗДАНИЕ ВЕТОК**

1. **> git branch feature/the-finest-branch** - *(от англ. branch, «ветка») — создай ветку от текущей с названием feature/the-finest-branch.*

2. **> git checkout -b feature/the-finest-branch** - *создай ветку feature/the-finest-branch и сразу переключись на неё.*


---


### **НАВИГАЦИЯ ПО ВЕТКАМ**

1. **> git branch** - *покажи, какие есть ветки в репозитории и в какой из них я нахожусь (текущая ветка будет отмечена символом \*).*

2. **> git branch -a** - *покажи все известные ветки, как локальные (в локальном репозитории), так и удалённые (в origin на GitHub).*

3. **> git checkout feature/br** - *переключись на ветку feature/br.*


---


### **СРАВНЕНИЕ ВЕТОК**

1. **> git diff main HEAD** - *(от англ. difference, «отличие», «разница») — покажи разницу между веткой main и указателем на HEAD.*

2. **> git diff HEAD~2 HEAD** - *покажи разницу между тем коммитом, который был два коммита назад, и текущим.*


---


### **УДАЛЕНИЕ ВЕТОК**

1. **> git branch -d br-name** - *удали ветку br-name, но только если она является частью main.*

2. **> git branch -D br-name** - *удали ветку br-name, даже если она не объединена с main.*


---


### **СЛИЯНИЕ ВЕТОК**

1. **> git merge main** - *(от англ. merge, «сливать», «поглощать») — объедини ветку main с текущей активной веткой.*


---


### **РАБОТА С УДАЛЕННЫМ РЕПОЗИТОРИЕМ**

1. **> git push -u origin my-branch** - *(от англ. push, «толкнуть», «протолкнуть») — отправь новую ветку **my-branch** в удалённый репозиторий и свяжи локальную ветку с удалённой, чтобы при дополнительных коммитах можно было писать просто **git push**, без **-u**.*

2. **> git push my-branch** - *отправь дополнительные изменения в ветку **my-branch**, которая уже существует в удалённом репозитории.*

3. **> git pull** - *(от англ. pull, «вытянуть») — подтяни изменения текущей ветки из удалённого репозитория.*


---


## **КАК СДЕЛАТЬ PULL REQUEST (PR) ЧЕРЕЗ КОНСОЛЬ ᕦ(ò_óˇ)ᕤ**

### **ПОДГОТОВКА (локальные изменения)**

1. **Переключись на main/master и обнови его:**

**> git checkout main** *\# переключись на основную ветку*

**> git pull origin main** *\# скачай последние изменения*

---

2. **Создай новую ветку для своей фичи:**

**> git checkout -b feature/my-awesome-feature** *\# создай ветку и переключись в неё*

---

3. **Внеси изменения в код:**

**> file.txt** *\# отредактируй файл (или через IDE)*

---

4. **Добавь изменения в коммит:**

**> git add .** *\# добавь ВСЕ изменения*

**\# или**

**> git add file.txt** *\# добавь только конкретный файл*

---

5. **Закоммить изменения:**

**> git commit -m "Добавил новую фичу"** *\# осмысленное описание, уровня КТН!*

---

6. **Запушь ветку на GitHub/GitLab:**

**> git push -u origin feature/my-awesome-feature** *\# **-u** связывает локальную и удалённую ветку*

---

### **СОЗДАНИЕ PULL REQUEST (через Git CLI)**

1. **Проверь, что ветка залита**

**> git branch -a** *# список всех веток (локальных и удалённых)*

---

2. **Открой PR через GitHub CLI (если установлен):**

**> gh pr create --base main --head feature/my-awesome-feature --title "Новая фича" --body "Описание изменений"** *\# осмысленное описание, уровня КТН!*

**Где:**

**> --base main — в какую ветку мерджить (обычно main).**

**> --head feature/my-awesome-feature — твоя ветка.**

**> --title и --body — заголовок и описание PR.*

---

3. **Если нет GitHub CLI — делаем вручную**

**Зайди в репозиторий на GitHub/GitLab.**

**Перейди во вкладку Pull Requests → New Pull Request.**

**Выбери:**

**base: main (куда мерджить).**

**compare: feature/my-awesome-feature (твоя ветка).**

**Напиши заголовок и описание.**

**Нажми Create Pull Request.**

---

### **ДАЛЬНЕЙШИЕ ДЕЙСТВИЯ (если PR требует правок) (ง°ل°)ง**

1. **Добавить новые изменения в существующий PR**

**> git checkout feature/my-awesome-feature** *\# переключись в свою ветку*

**\# внеси правки в код**

**> git add .**

**> git commit -m "Поправил баги по ревью"** *\# осмысленное описание, уровня КТН!*

**> git push origin feature/my-awesome-feature** *\# новые коммиты автоматически попадут в PR*

---

2. **Обновить ветку относительно main (если были конфликты)**

**> git checkout feature/my-awesome-feature** *\# переключись в свою ветку*

**> git fetch origin** *\# скачай свежие изменения*

**> git merge origin/main** *\# замерджь main в свою ветку*

**# или (лучше)**

**git rebase origin/main** *\# перебазируй свою ветку поверх main*

---

**Если конфликты:**

**Исправь их вручную.**

**Продолжи ребейс:**

**> git rebase --continue**

**Запушь с --force (если делал rebase):**

**> git push --force origin feature/my-awesome-feature**

---

## **ПОСЛЕ МЕРДЖА PR**

1. **Удали локальную ветку**

**> git checkout main** *\# переключись обратно в main*

**> git branch -d feature/my-awesome-feature** *\# удали свою ветку*

---

2. **Удали удалённую ветку (опционально)**

**> git push origin --delete feature/my-awesome-feature** *\# удалит ветку на GitHub*

---

### **📌 Итоговый чеклист**

✅ *Создал ветку → git checkout -b feature/name.*

✅ *Закоммитил изменения → git add + git commit.*

✅ *Запушил → git push -u origin feature/my-awesome-feature.*

✅ *Создал PR → через gh pr create или вручную в GitHub/GitLab.*

✅ *Обновил PR (если нужно) → новые коммиты + git push.*

✅ *После мержа → удалил ветку (git branch -d).*

### *Если что-то пошло не так — читай ошибки и гугли ¯\_(ツ)_/¯*