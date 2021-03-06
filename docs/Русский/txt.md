# Формат .txt
Вызов функций этого формата:

```python
import pulling.Txt as txt

txt.function(arguments)
result = txt.function(arguments)
```
## Возможные методы:
**get_text(** *path*, *coding='utf-8'* **)** - функция, которая возвращает текст из файла, в виде списка, где элементы списка - это предложения в файле.

 - *path* - путь к нужному файлу.

 - *coding* - кодировка для декодирования. По умолчанию стоит кодировка utf-8.


**find_text(** *path*, *pattern_list*, *coding='utf-8'* **)** - функция, которая возвращает совпадения из текста файла в виде словаря, где ключ - это шаблон поиска, а значение - это список с найденными совпадениями.

 - *path* - путь до нужного файла.

 - *pattern_list* - список с шаблонами, где каждый шаблон является отдельным элементом списка.

 - *coding* - кодировка для декодирования. По умолчанию стоит кодировка utf-8.


**write_text(** *path*, *line_list*, *mode='w'*, *coding='utf-8'* **)** - функция, которая записывает текст в файл и сохраняет его.

 - *path* - путь файла в который надо записать.

 - *line_list* - список со строками, которые нужно сохранить в файле.

 - *mode* - режим открытия файла. По умолчанию стоит режим чтения 'w'.

 - *coding* - кодировка для декодирования. По умолчанию стоит кодировка utf-8.
			


**replace_text(** *path*, *new_path*, *replacement_dict*, *coding='utf-8'*, *new_coding='utf-8'* **)** - функция, которая принимает словарь со словами, заменяет слова и сохраняет эти изменения в новом файле.

 - *path* - путь файла из которого надо взять текст.

 - *new_path* - путь файла, в который надо записать изменения. Если ввести тот же путь, то изменения сохранятся в этом файле.

 - *replacement_dict* - словарь со словами, где ключ - это слово, которое надо заменить, а значение - слово на которое надо заменить.

 - *coding* - кодировка для декодирования. По умолчанию стоит кодировка utf-8.

 - *new_coding* - кодировка для кодирования. По умолчанию стоит кодировка utf-8.