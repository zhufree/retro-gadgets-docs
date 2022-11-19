# Keypad

<img src="https://docs.retrogadgets.game/api/modules/Keypad.png" width="200" align="right">

Keypad являють собою сітку кнопок, які повідомляють про свій стан в декількох таблицях 4х4. Їм можна присвоювати символи за допомогою мультитула, але на відміну від більшості кнопок вони не мають світлодіодів.

## Властивості

### ButtonsState - `{{boolean}}` **[Тільки для читання]**
Таблиця, що відображає стан кожної кнопки у вигляді булевого значення.
До таблиці слід звертатись за допомогою [стовпчик][рядок]. Кожна комірка таблиці повертає значення "true", якщо відповідна кнопка утримується натиснутою, інакше - "false".

### ButtonsDown - `{{boolean}}` **[Тільки для читання]**
Як `ButtonsState`, але тільки `true` для конкретної кнопки в таблиці яку утримують.

### ButtonsUp - `{{boolean}}` **[Тільки для читання]**
Як `ButtonsState`, але тільки `true` для конкретної кнопки в таблиці яку відпускають.

## Обладнання
Ці властивості можуть бути встановлені за допомогою інспектора мультитула, але не можуть бути встановлені в програмному забезпеченні.

### Symbols - `{{Symbol}}` *(Обладнання)*
Таблиця символів для відображення на відповідних кнопках. Символи можуть бути пофарбовані за допомогою інструменту малювання в інший колір, ніж фон, але всі символи на клавіатурі будуть однакового кольору.