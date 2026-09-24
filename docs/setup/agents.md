# Planner

`planner` — основной агент для подготовки планов изменений.

Он:

* читает код и документацию;
* пишет планы только в `docs/plan/`;
* не может изменять код;
* не может выполнять bash-команды.

# Scout

`scout` — субагент для поиска по коду.

Он:

* работает в режиме `subagent`;
* только читает код;
* не изменяет файлы;
* не выполняет bash-команды;
* возвращает найденные места с путями и строками.

# Результат scout по mileage

* `frontend/index.html:30–31` — поле формы `<input name="mileage">`.
* `frontend/app.js:8, 13–15` — `mileage` преобразуется в число при сборке JSON-запроса.
* `backend/src/Domain/ApplicationValidator.php:43–45` — чтение `payload['mileage']` и проверка диапазона.
* `backend/src/Domain/ApplicationValidator.php:78` — нормализованный `mileage` возвращается в `input`.
* `backend/src/Domain/AssessmentService.php:30–33` — получает `input`, но `mileage` не участвует в решении.
* `backend/src/Repository/ApplicationRepository.php:45` — пробег сохраняется в БД.
* `backend/src/Repository/ApplicationRepository.php:68` — пробег читается из БД.
* `backend/config/rules.php:23` — задан `max_mileage_km = 500000`.
