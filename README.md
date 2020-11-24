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

### git config \<--global\> -e
откроет редактирование файла конфига в редакторе
```javascript
git config --global -e
git config --global --edit
```

### git config \<--global\> core.editor \<path to redactor bin\>
устанавливает редактор конфига по умолчанию  
-w (--wait) - параметр, который не позволит команде git закончиться  
пока редактирование не завершено
```javascript
git config --global core.editor -w "C:\Users\Rustam\AppData\Local\Programs\Microsoft VS Code\bin\code"
```




### git config \<--global\> alias.\<alias-name\> \<command-name\>
устанавливает алиас для команды git
```javascript
git config --global aliac.c config
git c
```
команды в алиасах можно комбинировать следующим образом
```javascript
git config --global aliac.pu "!git fetch; git rebase"
git pu
```
[ссылка на список алиасов из zsh](https://github.com/ohmyzsh/ohmyzsh/blob/master/plugins/git/git.plugin.zsh)