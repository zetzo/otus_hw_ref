ДЗ - 3 в таблице id 4

Вебинар Занятие «Знакомство с облачной инфраструктурой и облачными сервисами»

ДЗ Запуск VM в Yandex Cloud, управление правилами фаервола, настройка SSH подключения, настройка SSH подключения через Bastion Host, настройка VPN сервера и VPN-подключения.

Ссылка: https://otus.ru/teacher-lk/programs/1316/40669/

bastion_IP = 51.250.91.111
\
someinternalhost_IP = 10.128.0.6
\

Host bastion
    HostName 51.250.91.111
    User appuser
    IdentityFile ~/.ssh/appuser

Host someinternalhost
    HostName 10.128.0.6
    User appuser
    ProxyJump bastion