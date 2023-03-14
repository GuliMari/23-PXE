# Домашнее задание: Настройка PXE сервера для автоматической установки
1. Установить и настроить загрузку по сети для дистрибутива CentOS8.
    - В качестве шаблона воспользуйтесь репозиторием https://github.com/nixuser/virtlab/tree/main/centos_pxe.
    - Поменять установку из репозитория NFS на установку из репозитория HTTP.
    - Настроить автоматическую установку для созданного kickstart файла (*) Файл загружается по HTTP.
2. Задание со звездочкой *
    - автоматизировать процесс установки Cobbler cледуя шагам из документа https://cobbler.github.io/quickstart/.
    
# Выполнение:

Следуя шагам в методичке, разворачиваем две виртуалки `pxeserver` и `pxeclient`.
Попробуем запустить процесс установки вручную:

![Image alt](https://github.com/GuliMari/23-PXE/blob/main/Screenshot%20from%202023-03-14%2009-38-37.png)

Выбираем графическую установку и указываем все необходимые компоненты настройки:

![Image alt](https://github.com/GuliMari/23-PXE/blob/main/Screenshot%20from%202023-03-14%2010-27-20.png)

После добавления в `ansible` автоматической установки с помощью Kickstart-файла:

![Image alt](https://github.com/GuliMari/23-PXE/blob/main/Screenshot%20from%202023-03-14%2010-48-45.png)

    
