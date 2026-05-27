## Laboratory work IV

Данная лабораторная работа посвящена изучению систем непрерывной интеграции (Continuous Integration).

### Task

Настроить систему CI для проекта C++ с использованием Travis CI и AppVeyor.

### Steps

1. Создан публичный репозиторий `lab04`
2. Склонирован исходный проект
3. Добавлен файл `.travis.yml`
4. Настроена сборка проекта через CMake
5. Подключён Travis CI для Linux
6. Подключён AppVeyor для Windows
7. Добавлен badge статуса сборки в `README.md`

### Files

#### .travis.yml

```yaml
language: cpp

script:
- cmake -H. -B_build -DCMAKE_INSTALL_PREFIX=_install
- cmake --build _build
- cmake --build _build --target install

addons:
  apt:
    packages:
    - cmake
    - cmake-data
```

### Links

- Repository: https://github.com/ahokard/lab04
- Travis CI: https://travis-ci.org/ahokard/lab04
- AppVeyor: https://ci.appveyor.com/project/ahokard/lab04
