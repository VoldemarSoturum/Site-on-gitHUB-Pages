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

>CODE FOR SORTING FOLDERS

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


