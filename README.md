# JavaScript

### Содержание:
- **[Recourse]()**
- **[Clousure]()**

---

![js.img](https://media.licdn.com/dms/image/v2/C4D12AQEWZhF2X25z_w/article-cover_image-shrink_720_1280/article-cover_image-shrink_720_1280/0/1606115147868?e=2147483647&v=beta&t=pSTolqMRYBEn-AU3O4PAcdXMzonHGiweJIiMdqVf5Us)

---

## Что такое **[RECOURSE]()** ?

*- это метод выполнения функции **[(Function)]()** при котором функция вызывает сама себя. Метод используется для упрощения решения некоторых задач.*

**Пример:**

```JavaScript

function factorial(x) {

  if (x == 0) return 1;
  return x * factorial(x - 1); 
  
}

console.log(factorial(5));  // 120


```
---

![js.img](https://media2.dev.to/dynamic/image/width=1280,height=720,fit=cover,gravity=auto,format=auto/https%3A%2F%2Fdev-to-uploads.s3.amazonaws.com%2Fuploads%2Farticles%2F16uvtgfsbbutez78sr98.png)

## Что такое **[CLOSURES]()** ?

*- это метод выполнения функции **[(Function)]()** при котором функции может создать внутри себя функцию которая в свою очередь имеет доступ к её внешнему окружению и выполняет определенную задачу.*

**Пример:**

```JavaScript

let counter = () => {
    let cnt = 0;
    return () => {
        return () => {
            cnt++;
            return cnt;
        }
    }
}
let get = counter()();

```

---