# Русская локализация MAVO 

Для использования плагина:
  1. Загрузите [файл локализации](https://github.com/sharabin/mavo-locale-ru/blob/master/mavo-locale-ru.js).
  2. Подключите загруженный файл к своему проекту с помощью элемента **<script>**.
  3. Добавьте атрибут **lang="ru"** к корневому элементу **Mavo**.

**P. S.** Дополнительно нужно внести правки в файл **mavo.css**, подменив жёстко закодированные строки:

```CSS
.mv-message.mv-warning::before {
  content: "⚠️ Внимание: ";
}

.mv-message.mv-error::before {
  content: "😳 Ой! ";
}

.mv-message::before {
    content: "Уведомление: ";
}

time[property][aria-label][mv-mode="edit"].mv-empty::before {
  content: "(Нет " attr(aria-label) ")";
}
```
