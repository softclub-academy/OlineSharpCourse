### Вазифаҳо дар мавзуи Class ва Object  

---

### **Вазифа 1: сохтани класси `Car` (Мошин)**  
**Тавсифи вазифа:**  
Класси `Car` созед, ки тағйирёбандаҳои public `make`, `model` ва `year` дошта бошад. Метод `displayDetails()` бояд маълумоти мошинро чоп кунад.  

**Воридот:**  
```csharp
Car car1 = new Car();
car1.make = "Toyota";
car1.model = "Corolla";
car1.year = 2020;
car1.displayDetails();

Car car2 = new Car();
car2.make = "Honda";
car2.model = "Civic";
car2.year = 2018;
car2.displayDetails();
```

**Баромад:**  
```
Toyota Corolla, 2020  
Honda Civic, 2018
```

---

### **Вазифа 2: Сохтани класси `Person` (Шахс)**  
**Тавсифи вазифа:**  
Класcи `Person` созед, ки тағйирёбандаҳои  `name` ва `age` дошта бошад. Метод `introduce()` бояд бигӯяд:  
"Салом, номи ман [name] аст ва ман [age] солаам."

**Воридот:**  
```csharp
Person person1 = new Person();
person1.name = "Аҳмад";
person1.age = 25;
person1.introduce();

Person person2 = new Person();
person2.name = "Зуҳро";
person2.age = 30;
person2.introduce();
```

**Баромад:**  
```
Салом, номи ман Аҳмад аст ва ман 25 солаам.  
Салом, номи ман Зуҳро аст ва ман 30 солаам.
```

---

### **Вазифа 3: Сохтани класси `Rectangle` (Роскунҷа)**  
**Тавсифи вазифа:**  
Синфи `Rectangle` созед, ки тағйирёбандаҳои public `length` ва `width` дошта бошад. Метод `calculateArea()` масоҳати росткунҷа ҳисоб мекунад.  

**Воридот:**  
```csharp
Rectangle rectangle = new Rectangle();
rectangle.length = 5;
rectangle.width = 10;
Console.WriteLine(rectangle.calculateArea());
```

**Баромад:**  
```
50
```

---

### **Вазифа 4: Сохтани класи `Circle` (Доира)**  
**Тавсифи вазифа:**  
Класси `Circle` созед, ки тағйирёбандаи public `radius` дошта бошад. Метод `calculateCircumference()` гирдогирии доираро ҳисоб мекунад.  

**Воридот:**  
```csharp
Circle circle = new Circle();
circle.radius = 7;
Console.WriteLine(circle.calculateCircumference());
```

**Баромад:**  
```
43.982297150257104
```

---

### **Вазифа 5: Сохтани класси `Account` (Суратҳисоб)**  
**Тавсифи вазифа:**  
Класси `Account` созед, ки тағйирёбандаҳои public `ownerName` ва `balance` дошта бошад. Методҳо:  
- `deposit(amount)` - маблағро ба тавозун илова мекунад.  
- `withdraw(amount)` - маблағро аз тавозун ихтисор мекунад.  

**Воридот:**  
```csharp
Account account = new Account();
account.ownerName = "Фирдавс";
account.balance = 1000;
account.deposit(500);
account.withdraw(300);
Console.WriteLine(account.balance);
```

**Баромад:**  
```
1200
```

---

### **Вазифа 6: Сохтани класси `Book` (Китоб)**  
**Тавсифи вазифа:**  
Класси `Book` созед, ки тағйирёбандаҳои public `title`, `author` ва `price` дошта бошад. Метод `showInfo()` маълумоти китобро чоп мекунад.  

**Воридот:**  
```csharp
Book book = new Book();
book.title = "Дунёи нав";
book.author = "Муҳаммад Иқбол";
book.price = 150;
book.showInfo();
```

**Баромад:**  
```
Китоб: Дунёи нав  
Муаллиф: Муҳаммад Иқбол  
Нарх: 150
```  

--- 
