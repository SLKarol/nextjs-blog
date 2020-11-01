---
title: "Когда использовать статическую генерацию вместо Рендеринг на стороне сервера"
date: "2020-01-02"
---

Мы рекомендуем использовать **Static Generation** (с данными или без них) когда это возможно, потому что ваша страница может быть создана один раз и обслужена CDN, что делает ее намного быстрее, чем сервер, отображающий страницу при каждом запросе.

Вы можете использовать статическую генерацию для многих типов страниц, включая:

- Маркетинговые страницы
- Сообщения в блоге
- Списки продуктов электронной коммерции
- Справка и документация

Ты должен спросить себя: "Могу ли я предварительно отобразить эту страницу **перед** запросом пользователя?" Если ответ положительный, вам следует выбрать «Статическая генерация».

On the other hand, Static Generation is **not** a good idea if you cannot pre-render a page ahead of a user's request. Maybe your page shows frequently updated data, and the page content changes on every request.

In that case, you can use **Server-Side Rendering**. It will be slower, but the pre-rendered page will always be up-to-date. Or you can skip pre-rendering and use client-side JavaScript to populate data.
