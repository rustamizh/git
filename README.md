### git config \<parameter\> \<--global\>
устанавливает parameter в качестве конфигурации  
флаг --global делает установку глобальной для текущего пользователя
```javascript
git config user.name "User Name"
git config user.email "email@mail.ru"
```

### git config --unset \<parameter\> \<--global\>
удаляет parameter из конфигурации
```javascript
git config --unset user.name "User Name"
git config --unset user.email "email@mail.ru"
```

### git config --remove-section \<parameter\> \<--global\>
удаляет всю секцию из конфигурации
```javascript
git config --remove-section user
```

### git config -h
показать документацию-подсказу по команде config
```javascript
git config -h
```

### git help \<command\>
откроет подробную документацию по команде
```javascript
git help config
```