## Laboratory work IV

### Тема
Непрерывная интеграция с использованием GitHub Actions

### Цель работы
Изучить принципы непрерывной интеграции (Continuous Integration) и настроить автоматическую проверку проекта с использованием GitHub Actions.

### Задание
В ходе выполнения лабораторной работы требовалось:

- клонировать репозиторий с GitHub;
- проверить структуру проекта;
- собрать проект с помощью CMake;
- запустить исполняемый файл;
- проверить настройку GitHub Actions;
- обновить документацию проекта;
- подготовить отчёт.

### Структура проекта
В проекте используются следующие файлы:

- `CMakeLists.txt` — файл конфигурации сборки;
- `main.cpp` — исходный код программы;
- `README.md` — описание проекта;
- `REPORT.md` — отчёт по лабораторной работе;
- `.github/workflows/ci.yml` — файл настройки GitHub Actions.

### Выполнение работы

#### Клонирование репозитория

```bash
git clone https://github.com/ahokard/lab09.git
cd lab09

## CI Status

[![CI](https://github.com/ahokard/lab04/actions/workflows/ci.yml/badge.svg)](https://github.com/ahokard/lab04/actions)
