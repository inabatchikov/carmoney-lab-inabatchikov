готов.
1) Учебный сервис предварительной оценки заявки на заём под ПТС: принимает заявку, считает LTV и возвращает `approve` / `review` / `reject`.
2) Makefile: `help`, `up`, `down`, `ps`, `logs`, `install`, `test`, `lint`, `seed`; docker-compose.yml: сервисы `backend` (PHP-сервер на 8080) и `db` (MySQL 8), healthcheck базы.
3) Решение по заявке считается в папке `backend/src/Domain`.
модель: training-2026-09-gpt-5.6-terra
