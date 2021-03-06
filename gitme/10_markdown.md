[К содержанию](../../../)
# Основы языка разметки Markdown

## Теги

### Парные теги:

| Тег    | Значение |
| -------|----------|
|* или _ | курсив |
|**      | жирный |
|~~ 	 | зачеркнутый |
|***     | жирный с курсивом |

### Строчные теги:
| Тег    | Значение |
| -------|----------|
| >       | цитата |
| >>      | вложенная цитата |
| 4 пробела | выделенный абзац |
| * или - или + | элемент маркированного списка |
| (цифра любая) | элемент нумерованного списка |

Если в тексте документа требуется отобразить символ, который используется как тег, то этот символ нужно экранировать с помощью обратного слеша. Например, следующий текст:

    ```\* – это звездочка, а не *курсив* и не список```

соберется как:

* – это звездочка, а не курсив и не список.
Вставки

В дополнение к отформатированному тексту в markdown можно вставить дополнительные элементы.

Для вставки гиперссылки используется следующая конструкция:

    [Текст](ссылка)

Например, исходный текст:

    [Поисковая система Яндекс](http://yandex.ru)

соберется как: 

[Поисковая система Яндекс](http://yandex.ru).

Для вставки картинки используется следующая конструкция:

    ![альтернативный текст](ссылка на картинку)

Альтернативный текст будет показываться в то время, когда картинка загружается. Например, исходный текст:

    ![Логотип markdown](https://upload.wikimedia.org/wikipedia/commons/4/48/Markdown-mark.svg)

будет собран в такую картинку: 

![Логотип markdown](https://upload.wikimedia.org/wikipedia/commons/4/48/Markdown-mark.svg)

Для вставки более сложных элементов (например, видео) или использования более сложных элементов оформления в исходный текст на языке markdown могут быть вставлены теги языка HTML. Например, следующим образом можно создать метку в тексте:

    <a name="label">на этот текст мы сможем сделать гиперссылку</a>

а затем сослаться на нее:

[гиперссылка на метку](#label)

[К содержанию](../../../)