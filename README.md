# Итоговый проект модуля «Облачная инфраструктура. Terraform»

Предлагаем вам выполнить итоговый проект, чтобы закрепить полученные знания и навыки. 

---

## Обратите внимание
Перед выполнением итогового проекта, мы рекомендуем вам выполнить все обязательные и дополнительные домашние задания модулей «Виртуализация и контейнеризация» и «Облачная инфраструктура. Terraform».

---

### Цель итогового проекта 
Развернуть web-приложение для работы в облачной инфраструктуре Yandex Cloud. 

В результате выполнения итогового проекта вы:
- получите опыт работы с облачной инфраструктурой Yandex Cloud
- примените принципы IaaC при работе с виртуальными машинами
- овладеете навыками развертывания и настройки веб-приложений
- выполните оркестрацию контейнеров с Docker Compose и Docker Swarm
- получите опыт работы с Terraform для управления инфраструктурой
- сможете включить созданное web-приложение в свое портфолио

---

### Сроки выполнения 
На выполнение этого проекта вам дается 7 дней. У вас есть 2 попытки на доработку итогового проекта. 

---

### Чек-лист готовности к работе над проектом
- изучен основной и дополнительный теоретический материал по модулям «Виртуализация и контейнеризация» и «Облачная инфраструктура. Terraform»
- выполнены все обязательные домашние задания модулей

---

### Инструменты и дополнительные материалы, которые пригодятся для выполнения задания
- Docker
- Docker Compose
- Terraform

---

### Описание итогового проекта
Задания итогового проекта охватывают полный цикл создания и настройки инфраструктуры, установку необходимых инструментов, сборку и развертывание приложения, а также хранение образов в реестре контейнеров. 

В рамках итогового проекта вы:
1.	Соберете просто web-приложение на основании представленных нами данных (с описанием Dockerfile, docker compose yml).
2.	Настроите инфраструктуру в Yandex Cloud, используя Terraform.
Развернете приложение в облачной среде.

Инструкция по выполнению итогового проекта:
Используя инструменты Docker, Docker Compose и Terraform, вам необходимо сделать следующее: 

**Задание 1.** Развертывание инфраструктуры в Yandex Cloud.
1.1 Создайте Virtual Private Cloud (VPC).
1.2 Создайте подсети.
1.3 Создайте виртуальные машины (VM):
1.3.1 Настройте группы безопасности (порты 22, 80, 443).
1.3.2 Привяжите группу безопасности к VM.
1.4. Опишите создание БД MySQL в Yandex Cloud.
1.5. Опишите создание Container Registry.

**Задание 2.** Используя user-data (cloud-init), установите Docker и Docker Compose (см. Задания 5 модуля «Виртуализация и контейнеризация»).

**Задание 3.** Опишите Docker файл (см. Задания 5 «Виртуализация и контейнеризация») c web-приложением и сохраните контейнер в Container Registry. 

**Задание 4.** Завяжите работу приложения в контейнере на БД в Yandex Cloud.

**Задание 5 (дополнительное).** Положите пароли от БД в LockBox и настройте интеграцию с Terraform так, чтобы пароль для БД брался из LockBox.

---

### Чек-лист готовности итоговой работы:
- инфраструктура в Yandex Cloud описана без хардкода, state хранится удаленно, подключен statelocking
- Docker и Docker Compose установлены через cloud-init 
- Dockerfile включает  мультисборку и сохранение образа в Container Registry
- приложения доступны по ip-адресу машины (в усложненном варианте - настроить DNS)
- создан MD-файл, который корректно оформлен и содержит примеры, скриншоты, ссылки

---

### Формат сдачи проекта: 
- Опишите проект в MD-файле, сформируйте ссылку и загрузите в Git репозиторий.
- Вставьте ссылку на вашу работу в поле «Ссылка на решение» и нажмите «Отправить».

---

### Критерии оценивания итоговой работы:

#### Зачёт
Выполнены все задания:
- инфраструктура в Yandex Cloud создана и настроена корректно
- web-приложение развернуто и доступно через указанные порты
- Dockerfile и Docker Compose написаны правильно и применены для сборки и развертывания приложения
- образы сохранены в Container Registry
- виртуальные машины правильно настроены и управляются с помощью Terraform
- создан и корректно оформлен MD-файл
- код хранится в Git

#### На доработку
Инфраструктура нестабильная или приложение не работает:
–	существуют проблемы с созданием инфраструктуры, установкой Docker, созданием Dockerfile или развертыванием приложения
–	не удается запустить приложение или оно недоступно
–	виртуальные машины не настроены или не  управляются с помощью Terraform
–	код содержит хардкод

#### Незачёт
«Незачет» ставится в крайнем случае, если вы присылаете пустое или недоработанное задание во второй раз после отправки работы на доработку

---

### Удачи в выполнении заданий!
