# 

Идею с свг утащил у Николая громова [svg-sprite](https://github.com/nicothin/svg-sprite/).

Для запуска сборки нужно поставить необходимые пакеты. Из папки проекта запустить:

```bash
npm i
```

# SVG-спрайты

Для сборки спрайта, запуска демки и автообновления:

```bash
grunt
```

## Что где

`/img/svg/` —  папка для мелких файлов, из которых собирается спрайт.

`/img/sprite.svg` — собираемый спрайт.

`/js/sсript.js` — готовый код для подгрузки svg-спрайта в localStorage (загружается один раз). Аккуратно с тестами, я пока не разобрался, как НЕ В РУЧНУЮ удалять ключи из localstorge.

## Найденные проблемы с SVG

Упорно не отображался спрайт, пока не разобрался, как должен выглядеть маленький svg-файл
```
<svg xmlns="http://www.w3.org/2000/svg" width="18" height="15" viewBox="0 0 18 15"><path d="код свг"/></svg>
```
