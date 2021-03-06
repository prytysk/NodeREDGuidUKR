[<- На головну](../)  [Розділ](README.md)

## HTML

![img](media/html.png) Витягує елементи з HTML-документа, що міститься в `msg.payload`  за допомогою селекторів CSS (рис.10.1).

В якості вхідного значення приймає наступні властивості повідомлень:

- payload (string)     – html- рядок з якого вилучаються елементи.
- select (string) -  селектор, може бути використане це значення     властивості msg, якщо воно не налаштовано на панелі редагування.

![img](media/10_1.png)

рис.10.1. Налаштування вузлу HTML

На виході формує:

- payload (array | string) - результатом може бути одне повідомлення з корисним     навантаженням, що містить масив відповідних елементів, або кілька     повідомлень, кожен з яких містить відповідний елемент. Якщо надсилаються     декілька повідомлень, вони також мають набір `parts`.

Цей вузол підтримує комбінацію селекторів CSS і jQuery. Докладніше про підтримуваний синтаксис див. [тут](https://developer.mozilla.org/uk/docs/Web/CSS/CSS_Selectors) або [Документацію css-select](https://github.com/fb55/CSSselect#user-content-supported-selectors). 