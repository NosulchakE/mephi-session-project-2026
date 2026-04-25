# mephi-session-project-2026

Сессионный проект по курсу "Операционные системы семейства Unix".

## Выполненные задания

- Настроен статический IP и hostname
- Проверена сетевая связность
- Установлены пакеты: nginx, tcpdump, libcap-ng-utils
- Скачан и установлен локальный RPM-пакет tcpdump
- Создан и примонтирован раздел с файловой системой ext4 (loop-устройство)
- Настроен автозапуск nginx
- Настроены права доступа (DAC): пользователь mephi-admin, группа mephi-devs, setgid
- Настроен SELinux (Enforcing, контекст httpd_sys_content_t)
- Настроены capabilities для tcpdump
- Запрещён вход root через SSH (PAM)
- Развёрнут веб-сервер nginx, отдающий страницу из /data/mephi-web

## Файлы в репозитории

- project_history.txt — история команд
- network_check.txt — проверка сети
- nginx_recent_logs.txt — логи nginx
- fstab.txt — настройки монтирования
- selinux_status.txt — статус SELinux
- file_contexts.txt — контексты SELinux
- tcpdump_capabilities.txt — capabilities tcpdump
- permissions.txt — права и владельцы
- users_groups.txt — пользователи и группы
- index.html — веб-страница
- curl_output.txt — результат проверки nginx
- mephi-nginx-screenshot.png — скриншот
- tcpdump.rpm — локальный RPM-пакет

## Стенд

Fedora 43 Server Edition, реальное железо.

## Сеть

Адаптирована под локальную сеть: 192.168.0.100/24, шлюз 192.168.0.1.
