# Практикум «Младший разработчик: первая неделя»

МДК.01.01 · аннотации типов и окружение проекта

- Студент: Сысуева Екатерина
- Группа: РПО-25/2
- Сдано: 30.10.2026, 12:56:27

## Рецензия

| Письмо | Результат | Баллы |
|---|---|---|
| Письмо 1 · рабочее место | 12 из 18 | 1 / 2 |
| Письмо 2 · подписи по заявкам | 4 из 10 | 1 / 4 |
| Письмо 3 · вызовы и подпись | 34 из 40 | 1 / 2 |
| Письмо 4 · подпись вручную | 2 из 4 | 1 / 2 |
| **Итого** | | **4 / 10 · неудовлетворительно** |

- Рабочее место: повторите порядок создания окружения и установки (глава 2.1, 2.3); что попадает в Git и зачем нужен .gitignore (глава 2.6); причины проблем с окружением — вопросы 1, 2.
- Подписи по заявкам: не решены заявки 1, 2, 3, 4, 5, 8. Повторите: словари и кортежи в аннотациях (глава 4.2, §2); какие данные нужны функции, а какие нет; запись X | None и объединение int | str (глава 4.2, §4–5); -> None у функции без результата (глава 4.2, §1).
- Вызовы и подпись: ошибки в подписях 1, 2, 3, 5. Прочитайте разбор под каждой.
- Подпись вручную: не решены заявки 2, 3.

## Письмо 1. Рабочее место

### Порядок команд — неверно

1. `Распаковать архив и открыть папку проекта в VS Code: File → Open Folder, затем Terminal → New Terminal`
2. `python -m venv .venv`
3. `Активировать окружение: .venv\Scripts\activate в Windows или source .venv/bin/activate в macOS и Linux`
4. `python -m pip install -r requirements.txt`

### Первый коммит — верно 7 из 10

| Файл | Ваш ответ | Верно |
|---|---|---|
| `main.py` | в репозиторий | ✓ |
| `app/calculator.py` | в репозиторий | ✓ |
| `tests/test_calculator.py` | в репозиторий | ✓ |
| `requirements.txt` | в репозиторий | ✓ |
| `README.md` | в репозиторий | ✓ |
| `.gitignore` | на компьютере | ✗ |
| `.venv/` | на компьютере | ✓ |
| `__pycache__/` | в репозиторий | ✗ |
| `app/__pycache__/calculator.cpython-312.pyc` | в репозиторий | ✗ |
| `.env` | на компьютере | ✓ |

### Вопросы из чата — верно 5 из 7

| Вопрос | Ваша причина | Верно |
|---|---|---|
| 1. Денис | VS Code использует другой интерпретатор, не из .venv | ✗ |
| 2. Лиза | Пакет установлен в другой Python, не в окружение проекта | ✗ |
| 3. Ксюша | Зависимости проекта не записаны в requirements.txt | ✓ |
| 4. Глеб | Нет правил .gitignore для окружения и кэша | ✓ |
| 5. Марат | Список зависимостей снят не в окружении проекта | ✓ |
| 6. Оля | VS Code использует другой интерпретатор, не из .venv | ✓ |
| 7. Тимур | Окружение перенесено с другого компьютера | ✓ |

## Письмо 2. Подписи по заявкам

### 1. Колледж «Северный» · электронный журнал — неверно

```python
def average_grade(grades: list[int]) -> int:
```

### 2. Колледж «Северный» · посещаемость — неверно

```python
def count_absences(marks: int | str) -> dict[str, int]:
```

### 3. Кофейня «Зерно» · касса — неверно

```python
def order_total(items: str | int, discount: int = 0) -> dict[str, int] | int:
```

### 4. Кофейня «Зерно» · постоянные гости — неверно

```python
def find_guest_phone(name: str) -> str | None:
```

### 5. Фитнес-клуб «Пульс» · абонементы — неверно

```python
def is_membership_active(end_date: date, today: date) -> str:
```

### 6. Книжный магазин «Переплёт» · склад — верно

```python
def parse_quantity(value: int | str) -> int:
```

### 7. Курьерская служба «Квартал» · отчёт за день — верно

```python
def distance_bounds(distances: list[float]) -> tuple[float, float]:
```

### 8. Кофейня «Зерно» · печать чека — неверно

```python
def print_receipt(lines: list[str]) -> None:
```

### 9. Колледж «Северный» · ведомость группы — верно

```python
def average_by_student(journal: dict[str, list[int]]) -> dict[str, float]:
```

### 10. Фитнес-клуб «Пульс» · карта клиента — верно

```python
def format_name(first_name: str, last_name: str, middle_name: str | None = None) -> str:
```

## Письмо 3. Вызовы и подпись

| Подпись | Верно |
|---|---|
| `def average_grade(grades: list[int]) -> float:` | 7 из 8 |
| `def find_guest_phone(guests: dict[str, str], name: str) -> str \| None:` | 6 из 8 |
| `def format_name(last_name: str, first_name: str, middle_name: str \| None = None) -> str:` | 6 из 8 |
| `def parse_quantity(value: int \| str) -> int:` | 8 из 8 |
| `def print_receipt(lines: list[str], width: int = 32) -> None:` | 7 из 8 |

## Письмо 4. Подпись вручную

### 1. Колледж «Северный» · лучший студент — верно

```python
def best_student(averages: dict[str, float]) -> str|None:
```

### 2. Фитнес-клуб «Пульс» · бонусы — неверно

```python
def add_bonus(balans: int, visits: int, is_vip: bool = False) -> int:
```

- параметры: balans, visits, is_vip, а нужны balance, visits, is_vip

### 3. Курьерская служба «Квартал» · адреса — неверно

```python
def split_address(adress: str) -> tuple[str,str]:
```

- параметры: adress, а нужны address

### 4. Книжный магазин «Переплёт» · авторы — верно

```python
def unique_authors(books: list[tuple[str, str]]) -> set[str]:
```
