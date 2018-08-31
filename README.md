# mavo-locale-ru
Русская локализация MAVO 

```CSS
.mv-message.mv-warning::before {
  content: "⚠️ Внимание: "; }

.mv-message.mv-error::before {
  content: "😳 Ой! ";
}

time[property][aria-label][mv-mode="edit"].mv-empty::before {
  content: "(Нет " attr(aria-label) ")";
}
```
