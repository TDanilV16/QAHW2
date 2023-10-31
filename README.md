# Домашка по настройке проекта

## [Poetry](https://python-poetry.org/)

## Линтеры: 
 - [flake8](https://pypi.org/project/flake8/) и обёртка над ним [pyproject-flake8](https://pypi.org/project/pyproject-flake8/) (pflake8) для настройки в pyproject.toml
 - Конфигурация flake8 в ``pyproject.toml`` ``[tool.flake8]``
   - Пример прогона линтера flake8 по всем файлам проекта:
     ```
      (hw2poetry-py3.11) PS C:\Dev\QA\HW2Poetry> pflake8 . 
      .\app\main.py:4:1 E302 expected 2 blank lines, found 1
      ```
 - [isort](https://pypi.org/project/isort/)
   - Конфигурация isort в ``pyproject.toml`` ``[tool.isort]``
     - Пример прогона isort по всем файлам проекта:
        ```
        (hw2poetry-py3.11) PS C:\Dev\QA\HW2Poetry> isort .
        Fixing C:\Dev\QA\HW2Poetry\app\main.py
        Skipped 2 files
        ```
## Автоформатер:
- [black](https://pypi.org/project/black/)
  - Конфигурация black в ``pyproject.toml`` ``[tool.black]``
    - Пример прогона black по всем файлам проекта:
    ```
       (hw2poetry-py3.11) PS C:\Dev\QA\HW2Poetry> black .
       reformatted C:\Dev\QA\HW2Poetry\app\main.py
       All done! ✨ 🍰 ✨
       1 file reformatted.
       ```
