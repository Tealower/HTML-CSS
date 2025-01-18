# Заняття 15

### Grid

__CSS Grid__ — це техніка в каскадних таблицях стилів, що дозволяє веб-розробникам створювати складні адаптивні макети вебдизайну більш легко і послідовно у різних веб-переглядачах.

Є й інші методи макета вебсторінок, що використовувались раніше, включаючи tables, CSS Box model та CSS Flexbox.


#### Основні поняття CSS Grid

**CSS Grid** складається з контейнера сітки (grid container) і елементів сітки (grid items). Контейнер сітки визначає поведінку сітки, а елементи сітки розміщуються всередині цього контейнера.

**Приклад контейнера сітки:**
```css
.container {
    display: grid;
}
```

**Основні властивості контейнера сітки:**
- `grid-template-columns`
- `grid-template-rows`
- `gap`

**Приклад елементів сітки:**
```html
<div class="container">
    <div class="item item1">1</div>
    <div class="item item2">2</div>
    <div class="item item3">3</div>
    <div class="item item4">4</div>
</div>
```

**Основні властивості елементів сітки:**
- `grid-column`
- `grid-row`
- `justify-self`
- `align-self`

---

#### Визначення колонок і рядків

Властивості `grid-template-columns` і `grid-template-rows` визначають кількість і розміри колонок і рядків.

```css
.container {
    display: grid;
    grid-template-columns: 100px 100px 100px;
    grid-template-rows: 100px 100px;
}
```

####  Розриви між елементами

Властивість `gap` використовується для встановлення розривів між елементами сітки.

```css
.container {
    display: grid;
    grid-template-columns: 100px 100px 100px;
    grid-template-rows: 100px 100px;
    gap: 10px;
}
```

#### Розміщення елементів

Властивості `grid-column` і `grid-row` дозволяють розміщувати елементи сітки у визначених колонках і рядках.

```css
.item1 {
    grid-column: 1 / 3; /* Займає першу та другу колонки */
    grid-row: 1; /* Займає перший рядок */
}
```

#### Вирівнювання елементів

Властивості `justify-self` та `align-self` використовуються для вирівнювання елементів всередині своєї сіткової області.

```css
.item1 {
    justify-self: center; /* Горизонтальне вирівнювання по центру */
    align-self: end; /* Вертикальне вирівнювання по нижньому краю */
}
```

---

### Завдання

Відкрийте index.htm та style.css в папці traveling. 

Оформіть завдання так як показано на зображенню.

<img src='traveling.jpg' width='400'>