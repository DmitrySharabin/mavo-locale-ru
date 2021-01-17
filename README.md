# Русская локализация Mavo 

Вы можете подключить плагин локализации, как и любой другой плагин Mavo, с помощью атрибута `mv-plugins` или вручную.

Чтобы подключить плагин вручную:
  1. Загрузите [файл локализации](https://cdn.jsdelivr.net/gh/DmitrySharabin/mavo-locale-ru/mavo-locale-ru.js).
  2. Подключите загруженный файл к своему проекту с помощью элемента `<script>`.
  3. Добавьте атрибут `lang="ru"` к корневому элементу приложения.

**P. S.** Дополнительно нужно переопределить следующие правила из `mavo.css`:

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

С более подробной информацией по локализации Mavo можно ознакомиться [здесь](https://mavo.io/docs/ui/#localization).
