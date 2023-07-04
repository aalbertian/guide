<!--|2|-->
# 2. CI/CD Automation
## 2.1 Helm
### 2.1.1 Описание
Helm - это менеджер пакетов для Kubernetes, называемые Chart. Helm может следующее:
* Создавать новый пустой Chart
*	Создавать архив tgz на основе существующего Chart
*	Взаимодействовать с репозиторием Chart
*	Устанавливать и удалять Charts на существующем Kubernetes кластере
*	Управлять существующими в Kubernetes релизами Charts
### 2.1.2 Первоначальная настройка
Для работы с Helm необходимы следующие компоненты:
*	Утилита kubectl
*	Kubernetes кластер

Установка Helm необходима на рабочих станциях, которые будут администрировать кластер Kubernetes. Для установки с помощью пакетного менеджера APT необходимо выполнить:

**Установка Helm** 

    curl https://baltocdn.com/helm/signing.asc | gpg --dearmor | sudo tee /usr/share/keyrings/helm.gpg > /dev/null
    sudo apt-get install apt-transport-https --yes
    echo "deb [arch=$(dpkg --print-architecture) signed-by=/usr/share/keyrings/helm.gpg] https://baltocdn.com/helm/stable/debian/ all    main" | sudo tee /etc/apt/sources.list.d/helm-stable-debian.list
    sudo apt-get update
    sudo apt-get install helm

**Обратите внимание**: пример приведен для ОС Ubuntu/Debian. Подробнее о первоначальной настройке можно прочитать в официальной документации - [ссылка](https://helm.sh/ru/docs/intro/quickstart/).


