
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <link href="https://fonts.googleapis.com/css2?family=Orbitron:wght@600&family=Share+Tech+Mono&display=swap" rel="stylesheet" />
  <style>
    body {
      margin: 0;
      font-family: 'Share Tech Mono', monospace;
      background: black;
      color: #00ffcc;
      overflow-x: hidden;
      position: relative;
    }
    .glitch-bg {
      position: fixed;
      top: 0;
      left: 0;
      width: 100vw;
      height: 100vh;
      z-index: -1;
      background: radial-gradient(circle at center, #0ff 0%, #004 80%);
      animation: cyberPulse 6s ease-in-out infinite;
      filter: blur(2px) brightness(0.6) contrast(1.2);
    }
    @keyframes cyberPulse {
      0%, 100% {
        background: radial-gradient(circle at center, #0ff 0%, #004 80%);
      }
      50% {
        background: radial-gradient(circle at center, #00f0ff 10%, #001122 80%);
      }
    }
    header {
      text-align: center;
      padding: 2rem 1rem;
      z-index: 1;
      position: relative;
    }
    .logo {
      width: 200px;
      border-radius: 50%;
      transition: transform 0.5s ease, filter 0.5s ease;
      filter: drop-shadow(0 0 10px #00ffee);
      animation: pulse 3s ease-in-out infinite;
    }
    .logo:hover {
      transform: scale(1.1) rotate(1deg);
      filter: drop-shadow(0 0 20px #00ffee) brightness(1.2);
    }
    @keyframes pulse {
      0%, 100% {
        transform: scale(1);
        filter: drop-shadow(0 0 10px #00ffee);
      }
      50% {
        transform: scale(1.05);
        filter: drop-shadow(0 0 20px #00ffee);
      }
    }
    h1 {
      font-family: 'Orbitron', sans-serif;
      font-size: 3rem;
      margin-top: 1rem;
      text-shadow: 0 0 5px #00ffee, 0 0 10px #00ffee;
      animation: flicker 1.5s infinite alternate, shake 0.1s infinite;
    }
    @keyframes flicker {
      0% { opacity: 1; }
      50% { opacity: 0.8; }
      100% { opacity: 1; }
    }
    @keyframes shake {
      0% { transform: translate(0px, 0px); }
      25% { transform: translate(1px, -1px); }
      50% { transform: translate(-1px, 1px); }
      75% { transform: translate(1px, 1px); }
      100% { transform: translate(-1px, -1px); }
    }
    main {
      max-width: 900px;
      margin: 0 auto;
      padding: 2rem;
    }
    section {
      margin-bottom: 3rem;
    }
    h2 {
      color: #ff00cc;
      text-shadow: 0 0 5px #ff00cc;
      font-size: 2rem;
    }
    pre {
      background: rgba(0, 0, 0, 0.7);
      padding: 1rem;
      border: 1px solid #00ffee;
      overflow-x: auto;
      white-space: pre-wrap;
    }
  </style>
  
# My profile 
# Nickname: Voldemar Soturum 

![alt-текст](https://avatars.githubusercontent.com/u/125198406?s=400&u=7d72e8ca033272aeb44d752b8fa57b7e038ccca9&v=4 "Текст заголовка логотипа 1")

## Name: 
    Ivan Chernyshev
## Profession: 
    Python Developer
    
## Location: 
>  Moscow,🇷🇺Russia 


> Email:  ivangoe110692@gmail.com 



>LinkedIn/GitHub: 
![VoldemarSoturum](https://github.com/VoldemarSoturum "VoldemarSoturum")


## Profile Summary
- Motivated and detail-oriented Python - Developer with a strong background in backend development, data processing, and software architecture. - Passionate about clean code, automation, and building scalable solutions. Experienced in working both independently and in collaborative teams to deliver high-quality software products.

## Technical Skills

    Languages: 
>Python, SQL, JavaScript (basic), Bash
---
    Frameworks: 
>Django, Flask, FastAPI
---
    Tools & Libraries:
>Celery, SQLAlchemy, Pandas, NumPy, Requests, BeautifulSoup
Databases: PostgreSQL, MySQL, SQLite, Redis
---

    DevOps:
> Docker, Git, GitHub Actions, Jenkins
Cloud & Hosting: AWS (EC2, S3, Lambda), Heroku
Other: REST API development, Web scraping, Unit testing (PyTest, unittest)

## Work Experience

### Python Developer

    Company Name – MASCOM
---
            07-2022 – Present

- Designed and implemented backend services using Django and FastAPI

- Created RESTful APIs for internal and external applications
- Developed data pipelines and automated reporting systems
- Collaborated with frontend developers and product managers to deliver features on time
- Improved application performance by optimizing database queries and code structure
---

### Junior Python Developer
    Company Name – NETOLOGY
---
                03-2025 – 03-2026

- Maintained and updated legacy codebase written in Flask
- Participated in daily stand-ups and sprint planning
- Wrote unit and integration tests to ensure code reliability
- Assisted in deployment processes using Docker and CI/CD pipelines
### Education
    COMPUTER SYSTEM  DYSIGNING AND INTELYGENCE SYS. ADMINISTARTOR

- University Name – Lughansk, East Ukrainian University of Vladimir Dahl 
- Studies in 2011 to 2014
---
    SENIOR OF LABORATORIES FOR RESEARCHING DATA LEAKAGE VIA THE CHANNEL OF SIDE ELECTROMAGNETIC SIGNALS AND INTERFERENCE 

- University Name – Moscow "MASKOM" Education Centert of InfoSec
- Studies in 2023 to 2023
---
    PYTHON-DEV
- Internet Education - **NETOLOGY** 
- 2025 - 2026

## Languages
    Russian 
- **Native**
---
    English 
- **Advanced** – depending on technition blogs and command line skill)

## Hobbies & Interests
> Open-source contribution, algorithm challenges (e.g. LeetCode) 

> Reading tech blogs

> Exploring new frameworks and tools.

<br>
<br>
<br>

# MY PORTFOLIO
---

## CODE FOR SORTING FOLDERS

```
    documents = [
        {"type": "passport", "number": "2207 876234", "name": "Василий Гупкин"},
        {"type": "invoice", "number": "11-2", "name": "Геннадий Покемонов"},
        {"type": "insurance", "number": "10006", "name": "Аристарх Павлов"},
        {"type": "driver license", "number": "5455 028765", "name": "Василий Иванов"},
      ]

directories = {
        '1': ['2207 876234', '11-2', '5455 028765'],
        '2': ['10006'],
        '3': []
      }
def get_name(doc_number):
    # Ищем документ с указанным номером в списке documents
    for document in documents:
        if document['number'] == doc_number:
            return document['name']
    return "Документ не найден"  # Если не найден, выводим сообщение

def get_directory(doc_number):
    # Ищем, на какой полке находится документ
    for shelf, docs in directories.items():
        if doc_number in docs:
            return shelf
    return "Полки с таким документом не найдено"  # Если полка не найдена, выводим сообщение


def add(document_type, number, name, shelf_number):
    # Добавляем новый документ в список
    new_document = {"type": document_type, "number": number, "name": name}
    documents.append(new_document)
    
    # Добавляем номер документа на соответствующую полку в directories
    # Если полка не существует, создаем её
    if str(shelf_number) not in directories:
        directories[str(shelf_number)] = []
    
    directories[str(shelf_number)].append(number)

if __name__ == '__main__':
    print(get_name("10006"))
    print(get_directory("11-2"))
    print(get_name("101"))
    add('international passport', '311 020203', 'Александр Пушкин', 3)
    print(get_directory("311 020203"))
    print(get_name("311 020203"))
    print(get_directory("311 020204"))

```

## CODE FOR SEARCH COUNT NAMESAKES


```
courses = ["Java-разработчик с нуля", "Fullstack-разработчик на Python", "Python-разработчик с нуля", "Frontend-разработчик с нуля"]
mentors = [
    ["Филипп Воронов", "Анна Юшина", "Иван Бочаров", "Анатолий Корсаков", "Юрий Пеньков", "Илья Сухачев", "Иван Маркитан", "Ринат Бибиков", "Вадим Ерошевичев", "Тимур Сейсембаев", "Максим Батырев", "Никита Шумский", "Алексей Степанов", "Денис Коротков", "Антон Глушков", "Сергей Индюков", "Максим Воронцов", "Евгений Грязнов", "Константин Виролайнен", "Сергей Сердюк", "Павел Дерендяев"],
    ["Евгений Шмаргунов", "Олег Булыгин", "Александр Бардин", "Александр Иванов", "Кирилл Табельский", "Александр Ульянцев", "Роман Гордиенко", "Адилет Асканжоев", "Александр Шлейко", "Алена Батицкая", "Денис Ежков", "Владимир Чебукин", "Эдгар Нуруллин", "Евгений Шек", "Максим Филипенко", "Елена Никитина"],
    ["Евгений Шмаргунов", "Олег Булыгин", "Дмитрий Демидов", "Кирилл Табельский", "Александр Ульянцев", "Александр Бардин", "Александр Иванов", "Антон Солонилин", "Максим Филипенко", "Елена Никитина", "Азамат Искаков", "Роман Гордиенко"],
    ["Владимир Чебукин", "Эдгар Нуруллин", "Евгений Шек", "Валерий Хаслер", "Татьяна Тен", "Александр Фитискин", "Александр Шлейко", "Алена Батицкая", "Александр Беспоясов", "Денис Ежков", "Николай Лопин", "Михаил Ларченко"]
]
durations = [14, 20, 12, 20]

courses_list = []
for course, mentor, duration in zip(courses, mentors, durations):
    course_dict = {"title": course, "mentors": mentor, "duration": duration}
    courses_list.append(course_dict)

# С этого момента начинается выполнение задания 4.
# На входе у вас есть только список курсов courses_list. Об исходных данных, на базе которых он был сделан, вы ничего не знаете

# На каждом курсе в отдельности вам необходимо: 1) найти имена, которые встречаются более 1 раза;
# 2) отобрать людей (Имя + Фамилия), для которых совпало Имя. Это и будут наши тёзки

for course in courses_list:
    # Самостоятельно напишите код, который создаёт множество уникальных имён без фамилий
    # Подсказка: вам нужно вспомнить и повторить код из задания 1 по множествам
    # Результат (уникальные имена без фамилий) запишите в переменную под названием unique_names, преобразуйте в список и отсортируйте по возрастанию
    # Это необходимо, чтобы ваша программа всегда давала один и тот же результат и тренажёр смог его сверить
    name_counts = {}
    for mentor in course["mentors"]:
        first_name = mentor.split()[0]
        name_counts[first_name] = name_counts.get(first_name, 0) + 1
    unique_names = sorted(set(name_counts))
    # Напишите алгоритм, который подсчитывает частоту встречаемости каждого имени из names_set в исходном списке преподавателей
    # Подсказка: при работе со строками воспользуйтесь конструкцией in
    # Внимание: в список same_name_list вы будете сохранять найденных тёзок-преподавателей
    same_name_list = []
    # Организуйте цикл по всем именам на курсе из множества:
    for name in unique_names:
        # Подсчитайте частоту встречаемости имени (должно быть более 1 раза):
        if name_counts[name] > 1:
            # Сделайте цикл по исходному списку преподавателей (с Именем и Фамилией)
            for mentor in course["mentors"]:
                # Найдите тех преподавателей, у кого совпало имя (для них if вернёт True)
                if name in mentor:
                    # Добавьте преподавателя с этим именем в список тёзок
                    same_name_list.append(mentor)
    # Если список тёзок не пустой, выведите всех преподавателей из него
    if same_name_list:
        # Дополните конструкцию ниже, чтобы выводилось сообщение такого вида: На курсе Название есть тёзки: тёзки через запятую
        # Подсказка: для соединения преподавателей через запятую используйте string.join()
        
        print(f'На курсе {course["title"]} есть тёзки: {", ".join(sorted(same_name_list))}')
```
