## Настройки для WebStorm после установки

#### Импортируем настройки из файла `webstorm.zip`
```
File > Import Settings...
```

#### Устанавливаем доступ по программе `Early Access Preview`
```
File > Settings... > Apperance & Behavior > System Settings > Updates
Automatically check updates for Early Access Preview
```

#### Настраиваем автоисправление `eslint` по `ctrl+s`
```
File > Settings... > Tools > File Watchers > Add > <custom>
Name: ESlint fix
File type: any
Scope: Project Files
Program: ./node_modules/.bin/eslint
Arguments: --fix $FilePath$
Output paths to refresh: $FileDir$
Auto-save edited files to trigger the watcher: false
Trigger the watcher on external changes: false
```
