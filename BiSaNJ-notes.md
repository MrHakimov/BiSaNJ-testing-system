## Некоторые важные поинты
1. `Standings` - для того, чтобы работал нужно флаги пользователей убрать (с инвизибл на пустой).
2. Если добавляешь новую задачку во время контеста или дорешивания, нужно сначала остановить, а потом запустить ejudge.
3. Регистрация нового пользователя:
Вход для администратора / `Users` для необходимого контеста / `User creation operations` / `Contest registration` / `Status`
4. `/var/www/html` - `index.html`
5. `service httpd restart` - перезагрузка сервера Apache;
6. `/etc/httpd/` - конфигурационные файлы сервера;
7. `/home/judges/data/contests` - конфигурационные файлы контестов;
8. Как создать общую папку для Windows и Виртуальной ОС:
    - Создать папку в Windows (например, `D:\Muhammadjon`);
    - В настройках виртуальной машины добавить созданную папку как общую (Настроить->Общие папки);
    - Изменяем права пользователя в Terminal (`su -`);
    - Создать папку в Fedora (`/home/ejudge/FolderName`);
    - Изменить права папки в Terminal (`chmod 777 /home/ejudge/FolderName`);
    - Набираем следующую команду: "`sudo mount -t vboxsf -o uid=1000,gid=1000 Muhammadjon /home/ejudge/FolderName" (Muhammadjon - это название папки в Windows - D:\Muhammadjon`).
