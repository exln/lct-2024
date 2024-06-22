[![Website](https://img.shields.io/website-up-down-green-red/http/shields.io.svg)](https://lct.undfnd.ru/)
[![us](https://img.shields.io/badge/exilon-lct_2024-purple)](https://github.com/exln/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
<br />
<div align="center">

  <a href="https://github.com/exln/lct-2024">
    <img src="docs/static/img/logo.png" alt="Logo" width="80" height="80">
  </a>

  <h1 align="center"> GeoXplore by exilon</h1>

  <p align="center">
    Сервис подбора и оценки территорий для вовлечения в хозяйственный оборот, Лидеры цифровой трансформации&nbsp;2024, команда&nbsp;exilon
    <br />
  </p>
</div>

## Навигация
- [Прототип решения ↗](https://lct.undfnd.ru/landing)
- [Документация API ↗](https://lct.undfnd.ru/docs/)
- [Описание проекта](#desc)
- [Диаграмма решения](#arch)
- [Стек технологий](#stack)
- [Сборка проекта](#launch)
- [Связанные репозитории](#repo)
- [Документация](#docs)
- [Лицензия](#license)

<a name="desc"></a>
## Описание проекта


<a name="arch"></a>
#### Диаграмма решения
![arch](docs/static/svg/arch.svg)<br>
Все компаненты контейнерезированы:
- `nginx` - Reverse-proxy, роутинг, SSL
- `frontend` - React SPA приложение для фронтенда
- `backend` - Python backend, использует `fastapi`, `uvicorn`, `sqlalchemy`, `pydantic` и `gigachain`
- `postgres` - Реляционая СУБД с расширением pg-vector

<a name="stack"></a>
## Стек технологий

- Frontend:
  [![React](https://img.shields.io/badge/React-61DAFB?logo=react&logoColor=black)](https://reactjs.org/)
  [![shadcn/ui](https://img.shields.io/badge/shadcn%2Fui-000?logo=shadcnui&logoColor=fff)](#)
  [![Next](https://img.shields.io/badge/Next-FFF?logo=nextdotjs&logoColor=black)](https://nextjs.org/)
  [![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?logo=typescript&logoColor=white)](https://www.typescriptlang.org/)
- Backend:
   [![Python](https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=white)](https://www.python.org/)
  [![Hugging Face](https://img.shields.io/badge/Hugging%20Face-FFD21E?logo=huggingface&logoColor=000)](#)
- Database:
  [![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?logo=postgresql&logoColor=white)](https://www.postgresql.org/)
- DevOps:
  [![Docker](https://img.shields.io/badge/Docker-2496ED?logo=docker&logoColor=white)](https://www.docker.com/)

<a name="launch"></a>

## Сборка проекта

### Запуск проекта в Docker

1. Установить [Docker](https://www.docker.com/get-started)
2. Склонировать данный репозиторий:
    ```bash
    git clone https://github.com/exln/lct-2024.git lct-exln
    cd lct-exln
    ```
2. Отредактируйте `.env.example` файл и переименуйте его в `.env`:
    ```bash
    cp .env.example .env
    ```
3. Запустите проект с помощью Docker Compose в фоновом режиме:
    ```bash
    docker-compose up -d --build
    ```
4. Теперь приложение доступно по адресу [http://localhost:3000](http://localhost:3000).


<a name="repo"></a>

## Репозитории
- [Frontend](https://github.com/exln/lct-2024-front)
- [Backend](https://github.com/exln/lct-2024-back)

<a name="docs"></a>

## Документация

- Документация к решению в формате pdf: [ссылка]()
- Презентация решения: [ссылка]()
- Прототип решения: [ссылка]()

<a name="license"></a>

## Лицензия

![License](https://img.shields.io/github/license/exln/lct-2024?color=blue)

&copy; 2024 **e**x**l**n
