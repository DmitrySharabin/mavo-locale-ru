# Русская локализация MAVO 

**P. S.** Дополнительно нужно внести правки в CSS-код, подменив жёстко закодированные строки:

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
