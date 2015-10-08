## About
Здесь находятся материалы сайта http://www.nas-faq.com
относящегося к конференции [NAS своими руками](http://forum.ixbt.com/topic.cgi?id=109:82).

"Родной" адрес на GitHub Pages: http://nas-faq.github.io. Следует его использовать в случае проблем с доменом nas-faq.com.

## Рекомендации редактирующим

- Заголовки определяют структуру оглавления. Не следует использовать заголовок первого уровня (т.е. заданный #).
  Используйте ##, ### и т.д.
- Не пренебрегайте атрибутами _title_ и _permalink_ в заголовках страницы.
- В данный момент в заголовок сайта автоматически линкуются страницы, имеющие заголовочный атрибут ```for_head: true```.
- На корневую страницу (т.е. _index.html_) выводится содержимое страниц c заголовочным атрибутом ```for_index: true```.
- Если нужно запретить автогенерацию TOC (т.е. содержания) на странице, то нужно добавть в заголовок страницы ```suppress_toc: true```.
- По умолчанию ширина TOC 25% (см. main.css). Для отдельной страницы можно переопределить ширину
  с помощью атрибута _toc_width_ (например _toc_width: 40%_).
- Для обсуждений вопросов, связанных с этим репозиторием и сайтом, используйте
конференцию [FAQ по "NAS своими руками"](http://forum.ixbt.com/topic.cgi?id=0:60781).
- В данный момент карта сайта не генерируется автоматически. Т.о. после создания новых страниц
не забывайте вносить их в site_map.md.
