D:/smart_horizon/other/carmoney-lab-inabatchikov                                   77b45dd [d1/1.2.1-1.2.3-inabatchikov]
D:/smart_horizon/other/carmoney-lab-inabatchikov/.kilo/worktrees/better-staircase  77b45dd [better-staircase]
D:/smart_horizon/other/carmoney-lab-inabatchikov/.kilo/worktrees/horn-burn         77b45dd (detached HEAD)



- `VinValidatorTest.php` — формат VIN: длина 17, регистр, запрещённые буквы I/O/Q, спецсимволы, пустая строка.
- `LtvCalculatorTest.php` — расчёт LTV в процентах (половина, треть, больше стоимости) и исключение при нулевой стоимости или неположительной сумме.
- `DecisionEngineTest.php` — решение по LTV: approve до 60, review до 85, reject выше, включая границы зон.
- `AssessmentServiceTest.php` — сквозной сценарий оценки заявки: approve с лимитом = запрошенной сумме, review/reject с нулевым лимитом и возрастом авто.
- `ApplicationValidatorTest.php` — валидация заявки: нормализация VIN, отказ при годе из будущего, сумме ниже минимума, сбор всех ошибок сразу.

Папка: `D:\smart_horizon\other\carmoney-lab-inabatchikov\.kilo\worktrees\better-staircase`, ветка: `better-staircase`.