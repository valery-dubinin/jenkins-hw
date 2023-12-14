# Домашнее задание к занятию "`Что такое DevOps. СI/СD`" - `Дубинин Валерий`

---

### Задание 1

**Что нужно сделать:**

1. Установите себе jenkins по инструкции из лекции или любым другим способом из официальной документации. Использовать Docker в этом задании нежелательно.
2. Установите на машину с jenkins [golang](https://golang.org/doc/install).
3. Используя свой аккаунт на GitHub, сделайте себе форк [репозитория](https://github.com/netology-code/sdvps-materials.git). В этом же репозитории находится [дополнительный материал для выполнения ДЗ](https://github.com/netology-code/sdvps-materials/blob/main/CICD/8.2-hw.md).
3. Создайте в jenkins Freestyle Project, подключите получившийся репозиторий к нему и произведите запуск тестов и сборку проекта ```go test .``` и  ```docker build .```.

В качестве ответа пришлите скриншоты с настройками проекта и результатами выполнения сборки.

**Решение:**
1. Конфиг первого задания:
![1](https://github.com/valery-dubinin/jenkins-hw/blob/main/1%20HW1%20config.png)
![2](https://github.com/valery-dubinin/jenkins-hw/blob/main/2%20HW1%20config2.png)

2. Run:
![3](https://github.com/valery-dubinin/jenkins-hw/blob/main/3%20HW1%201%20run.png)
![4](https://github.com/valery-dubinin/jenkins-hw/blob/main/4%20HW1%201%20run2.png)
![5](https://github.com/valery-dubinin/jenkins-hw/blob/main/5%20HW1%201%20run3.png)
![6](https://github.com/valery-dubinin/jenkins-hw/blob/main/6%20HW1%203%20run1.png)
![7](https://github.com/valery-dubinin/jenkins-hw/blob/main/7%20HW1%203%20run2.png)
---

### Задание 2

**Что нужно сделать:**

1. Создайте новый проект pipeline.
2. Перепишите сборку из задания 1 на declarative в виде кода.

В качестве ответа пришлите скриншоты с настройками проекта и результатами выполнения сборки.

**Решение:**

Исходники:
https://github.com/valery-dubinin/jenkins-hw/blob/main/Jenkins%20HW2

Скрины:

1. Конфиг 2 задания
![8](https://github.com/valery-dubinin/jenkins-hw/blob/main/8%20HW2%20config.png)

2. Run
![9](https://github.com/valery-dubinin/jenkins-hw/blob/main/9%20HW2%20run.png)
![10](https://github.com/valery-dubinin/jenkins-hw/blob/main/10%20HW2%20run2.png)

3. Результат
![11](https://github.com/valery-dubinin/jenkins-hw/blob/main/11%20HW2%20result.png)


---

### Задание 3

**Что нужно сделать:**

1. Установите на машину Nexus.
1. Создайте raw-hosted репозиторий.
1. Измените pipeline так, чтобы вместо Docker-образа собирался бинарный go-файл. Команду можно скопировать из Dockerfile.
1. Загрузите файл в репозиторий с помощью jenkins.

В качестве ответа пришлите скриншоты с настройками проекта и результатами выполнения сборки.

**Решение:**

Исходники:

https://github.com/valery-dubinin/jenkins-hw/blob/main/Jenkins%20HW3


1. Конфиг 3 задания
![12](https://github.com/valery-dubinin/jenkins-hw/blob/main/12%20HW3%20config.png)

2. Run
![13](https://github.com/valery-dubinin/jenkins-hw/blob/main/13%20HW3%20run.png)
![14](https://github.com/valery-dubinin/jenkins-hw/blob/main/14%20HW3%20run2.png)

3. Результат
![15](https://github.com/valery-dubinin/jenkins-hw/blob/main/15%20HW3%20result.png)



---
## Дополнительные задания* (со звёздочкой)

Их выполнение необязательное и не влияет на получение зачёта по домашнему заданию. Можете их решить, если хотите лучше разобраться в материале.

---

### Задание 4*

Придумайте способ версионировать приложение, чтобы каждый следующий запуск сборки присваивал имени файла новую версию. Таким образом, в репозитории Nexus будет храниться история релизов.

Подсказка: используйте переменную BUILD_NUMBER.

В качестве ответа пришлите скриншоты с настройками проекта и результатами выполнения сборки.

**Решение:**

См все предидущие сборки. Они версионированы
