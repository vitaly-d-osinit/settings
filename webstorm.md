## Настройки для WebStorm после установки

#### Импортируем настройки из файла `webstorm.zip`
```
File > Import Settings...
```

#### Настраиваем автоисправление `eslint` по `ctrl+s`
```
File > Settings... > Tools > File Watchers > Add > <custom>
Name: ESlint fix
File type: any
Scope: Project Files
Program: ./node_modules/.bin/eslint
Arguments: --fix $FilePatch$
Output paths to refresh: $FileDir$
Auto-save edited files to trigger the watcher: false
Trigger the watcher on external changes: false
```
