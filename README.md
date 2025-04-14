# 🧠 Voldemar Soturum

![Voldemar Soturum Logo](https://avatars.githubusercontent.com/u/125198406?s=400&u=7d72e8ca033272aeb44d752b8fa57b7e038ccca9&v=4)

## 🧑‍💻 Ivan Chernyshev

**👨‍💻 Python Developer**  
📍 Moscow, 🇷🇺 Russia  
✉️ [ivangoe110692@gmail.com](mailto:ivangoe110692@gmail.com)  
🔗 [GitHub — VoldemarSoturum](https://github.com/VoldemarSoturum)

---

## ⚡ Summary

> Motivated and detail-oriented Python Developer with a strong background in backend development, data processing, and software architecture.  
> Passionate about clean code, automation, and building scalable solutions.

---

## 🛠️ Tech Stack

**Languages:**  
`Python`, `SQL`, `JavaScript (basic)`, `Bash`

**Frameworks:**  
`Django`, `Flask`, `FastAPI`

**Tools & Libraries:**  
`Celery`, `SQLAlchemy`, `Pandas`, `NumPy`, `Requests`, `BeautifulSoup`

**Databases:**  
`PostgreSQL`, `MySQL`, `SQLite`, `Redis`

**DevOps / Hosting:**  
`Docker`, `Git`, `GitHub Actions`, `Jenkins`, `AWS (EC2, S3, Lambda)`, `Heroku`

**Other:**  
`REST API`, `Web scraping`, `PyTest`, `unittest`

---

## 🧳 Work Experience

### 🔹 Python Developer — MASCOM  
📅 *July 2022 – Present*

- Developed backend services with Django and FastAPI  
- Created and maintained REST APIs  
- Built data pipelines and automation tools  
- Worked in cross-functional teams to deliver new features  
- Optimized performance and reduced query load

---

### 🔹 Junior Python Developer — NETOLOGY  
📅 *March 2025 – March 2026*

- Maintained and refactored Flask-based legacy projects  
- Participated in agile processes (daily/sprints)  
- Wrote unit and integration tests  
- Used Docker & CI/CD for deployments

---

## 🎓 Education

- **Computer System Designing & InfoSec Admin**  
  _East Ukrainian University of Vladimir Dahl (2011–2014)_

- **Senior Lab Specialist on EM Leakage Research**  
  _MASKOM InfoSec Center, Moscow (2023)_

- **Python Developer**  
  _Netology Online Course (2025–2026)_

---

## 🌐 Languages

- 🇷🇺 **Russian** — Native  
- 🇬🇧 **English** — Advanced (Tech/Command Line)

---

## 🧩 Hobbies & Interests

- 🧠 Algorithm challenges (e.g. LeetCode)  
- 🛠️ Open-source contribution  
- 📚 Reading tech blogs  
- 🧪 Exploring new frameworks/tools

---

## 📂 Portfolio

### 📌 Folder Sorting Script

```python
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
    for document in documents:
        if document['number'] == doc_number:
            return document['name']
    return "Документ не найден"

def get_directory(doc_number):
    for shelf, docs in directories.items():
        if doc_number in docs:
            return shelf
    return "Полки с таким документом не найдено"

def add(document_type, number, name, shelf_number):
    documents.append({"type": document_type, "number": number, "name": name})
    directories.setdefault(str(shelf_number), []).append(number)

if __name__ == '__main__':
    print(get_name("10006"))
    print(get_directory("11-2"))
    print(get_name("101"))
    add('international passport', '311 020203', 'Александр Пушкин', 3)
    print(get_directory("311 020203"))
    print(get_name("311 020203"))
    print(get_directory("311 020204"))
  ```
### 📌 Namesakes Detection in Course Mentors
```python
for course in courses_list:
    name_counts = {}
    for mentor in course["mentors"]:
        first_name = mentor.split()[0]
        name_counts[first_name] = name_counts.get(first_name, 0) + 1

    same_name_list = []
    for name, count in name_counts.items():
        if count > 1:
            for mentor in course["mentors"]:
                if mentor.startswith(name):
                    same_name_list.append(mentor)

    if same_name_list:
        print(f'На курсе {course["title"]} есть тёзки: {", ".join(sorted(same_name_list))}')
```