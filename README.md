# technopark-theme-template
[Hugo](https://gohugo.io/) тема для презентаций Технопарка

Это шаблон презентации для Технопарка.

В него входит:

 - https://github.com/shower/shower/ - собственно механизм отображения презентаций;
 - https://highlightjs.org/ - подсветка кода;
 - http://docs.mathjax.org/en/latest/ - отображение математических формул;
 - первый и последний слайд;
 - обвес для Hugo для оборачивания презентаций в шаблон и генерации индексного файла.

В результате генерации получается россыпь файлов, которая не имеет внешних зависимостей и может отображаться в браузере. В том числе при открытии индексного файла и локального каталога.

## Пример использования

- Исходный код: https://github.com/mailcourses/technopark-dbms-lectures

## Как создать презентацию?

Простой шаблон презентации можно взять из директории exampleSize.

После этого нужно:

 - Поправить название презентации и контактные данные в `config.yaml`;
 - Заменить `themes/technopark-theme-template` на ссылку на данный шаблон.
   
   Например:

   ```
rm -rf themes/technopark-theme-template && git submodule add https://github.com/mailcourses/technopark-theme-template.git themes/tech-template
```

Собрать презентацию можно будет командой `hugo`: презентация появится в каталоге `public`.

Запустить локальный сервер можно командой `hugo server -w -b http://localhost/`: презентация будет доступна по адресу [http://localhost:1313/](http://localhost:1313/).
