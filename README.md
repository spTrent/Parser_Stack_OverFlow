## Программа парсит профили с первой страницы рейтинга по репутации за все время

### **Собирает:**
1. _Имя пользователя_
2. _Количество заданных вопросов_
3. _Количество ответов_
4. _Все badges_

---

**Ссылка на DockerHub:** https://hub.docker.com/repository/docker/sptrent/parser_sof/general

---

**Установка:**

    git clone https://github.com/spTrent/Parser_Stack_OverFlow.git
    cd Parser_Stack_OverFlow
    uv sync
    source .venv/bin/activate

---

**Запуск:**

    python main.py

---

**Сборка docker-образа:**

    docker build -t sptrent/parser_sof:latest .

---

**Запуск контейнера:**
    
    docker run -it sptrent/parser_sof:latest

---

**Запуск контейнера с BindMount:**

    docker run -it -v $(pwd):/app sptrent/parser_sof:latest
