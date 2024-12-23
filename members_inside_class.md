Вазифаҳо дар мавзӯи Аъзоҳои **Class**

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

### **Вазифа 2: сохтани конструктор**  
**Тавсифи вазифа:**  
Класси `Car` созед, ки тағйирёбандаҳои private `make`, `model` ва `year` дошта бошад. Конструктори он бояд ин тағйирёбандаҳоро инициализатсия кунад.  

**Воридот:**  
```csharp
Car car1 = new Car("Toyota", "Corolla", 2020);
car1.displayDetails();

Car car2 = new Car("Honda", "Civic", 2018);
car2.displayDetails();
```

**Баромад:**  
```
Toyota Corolla, 2020  
Honda Civic, 2018
```

---

### **Вазифа 3: истифодаи Access Modifiers**  
**Тавсифи вазифа:**  
Класси `BankAccount` созед, ки тағйирёбандаи private `balance` дошта бошад. Методҳои public `Deposit` ва `GetBalance` барои зиёд кардани маблағ ва дидани бақияро илова кунед.  

**Воридот:**  
```csharp
BankAccount account = new BankAccount();
account.Deposit(1000);
account.Deposit(500);
Console.WriteLine(account.GetBalance());
```

**Баромад:**  
```
1500
```

---

### **Вазифа 4: сохтани методҳои иловагӣ**  
**Тавсифи вазифа:**  
Класси `Calculator` созед, ки методҳои `Add`, `Subtract`, `Multiply` ва `Divide` дошта бошад. Ҳар метод бояд ду параметр гирад ва натиҷа диҳад.  

**Воридот:**  
```csharp
Calculator calc = new Calculator();
Console.WriteLine(calc.Add(10, 5));       // 15
Console.WriteLine(calc.Subtract(10, 5)); // 5
Console.WriteLine(calc.Multiply(10, 5)); // 50
Console.WriteLine(calc.Divide(10, 5));   // 2
```

**Баромад:**  
```
15  
5  
50  
2
```

---

### **Вазифа 5: сохтани Properties**  
**Тавсифи вазифа:**  
Класси `Student` созед, ки property-ҳои зеринро дошта бошад:

- `Name` (read/write): Ном бояд ҳадди ақал 3 ҳарф дошта бошад. Агар ном кӯтоҳ бошад, онро ба Unknown иваз кунед.
- `Grade` (write-only): Танҳо арзишҳои аз 0 то 100 қабул карда шаванд. Агар арзиш берун аз ин диапазон бошад, онро ба 0 иваз кунед.
- `ID` (read-only): ID бояд ҳангоми сохтани объект бо истифода аз конструктор таъин карда шавад.
- Метод `GetStudentInfo()` илова кунед, ки номи донишҷӯ ва ID-и ӯро баргардонад.
- Метод `IsPassed()` илова кунед, ки санҷад, ки донишҷӯ дар асоси grade аз 60 гузашт ё не.

**Воридот:**  
```csharp
Student student1 = new Student(101);
student1.Name = "Ali";
student1.Grade = 85;
Console.WriteLine(student1.GetStudentInfo());
Console.WriteLine($"Passed: {student1.IsPassed()}");

Student student2 = new Student(102);
student2.Name = "An";
student2.Grade = 150; // Нодуруст, бояд 0 гузошта шавад.
Console.WriteLine(student2.GetStudentInfo());
Console.WriteLine($"Passed: {student2.IsPassed()}");

```

**Баромад:**  
```
Name: Ali, ID: 101  
Passed: True  

Name: Unknown, ID: 102  
Passed: False  
```

---

### **Вазифа 6: истифодаи Records**  
**Тавсифи вазифа:**  
Рекорди `Employee` созед, ки `Name`, `ID` ва `Salary` дошта бошад. Экземпляри рекорд созед ва онро чоп кунед.  

**Воридот:**  
```csharp
Employee emp1 = new Employee("Ali", 101, 50000);
Console.WriteLine(emp1);
```

**Баромад:**  
```
Employee { Name = Ali, ID = 101, Salary = 50000 }
```

---

### **Вазифа 7: Демонстрацияи Object Initializer**  
**Тавсифи вазифа:**  
Класси `Book` созед, ки тағйирёбандаҳои public `Title`, `Author`, ва `Pages` дошта бошад. Экземпляри классро бо истифода аз object initializer созед.  

**Воридот:**  
```csharp
- ----
```

**Баромад:**  
```
C# Basics by John Doe, 300 pages
```

---

### **Вазифа 8: Истифодаи конструктори параметрӣ ва default**  
**Тавсифи вазифа:**  
Класси `Library` созед, ки тағйирёбандаҳои `name` ва `location` дошта бошад. Конструктори default ва параметрӣ созед.  

**Воридот:**  
```csharp
Library lib1 = new Library();
Library lib2 = new Library("City Library", "Downtown");
lib1.DisplayInfo();
lib2.DisplayInfo();
```

**Баромад:**  
```
Default Library, Default Location  
City Library, Downtown
```

---

### **Вазифа 9: Муқоисаи Records**  
**Тавсифи вазифа:**  
Рекорди `Person` созед. Экземплярҳои он созед, нусхаи тағйирёфта созед ва ду экземплярро муқоиса кунед.  

**Воридот:**  
```csharp
------
```

**Баромад:**  
```
False or True
```

---

### **Вазифа 10: Истифодаи ҳама мавзӯъҳо бо китобҳо дар китобхона**

**Тавсифи вазифа:**  
Барои барномаи идоракунии китобхона, класи `Library` созед, ки хусусиятҳои зеринро дошта бошад:  
- Методҳои:
  - `AddBook(Book book)`: Илова кардани китоб ба китобхона. Агар китоб бо ҳамин ном ва муаллиф вуҷуд дошта бошад, танҳо миқдори онро зиёд мекунад.
  - `RemoveBook(string title)`: Хориҷ кардани як нусхаи китоб аз китобхона. Агар миқдор ба 0 расад, китоб аз рӯйхат хориҷ мешавад.
  - `ListBooks()`: Рӯйхати ҳамаи китобҳо ва нусхаҳои мавҷудро чоп кунад.
  - `CountBooksByTitle(string title)`: Миқдори умумии нусхаҳои китоб бо номи додашударо ҳисоб кунад.
  - `SearchBooks(string keyword)`: Китобҳоро аз рӯи калимаи калидӣ дар `Title` ё `Author` ҷустуҷӯ кунад.

**Талаботҳо:**  
- Китобҳо дар рӯйхат ҳамчун объекти `Book` ифода шаванд, ки дорои property-ҳои зерин бошанд:
  - `Title`: Номи китоб.
  - `Author`: Муаллифи китоб.
  - `Pages`: Шумораи саҳифаҳои китоб.
  - `Quantity`: Миқдори нусхаҳои китоб.

---

**Намунаи воридот:**  
```csharp
Library library = new Library();

// Илова кардани китобҳо
library.AddBook(new Book { Title = "Тоҷикон", Author = "Бобоҷон Ғафуров", Pages = 900, Quantity = 2 });
library.AddBook(new Book { Title = "Адабиёти тоҷик", Author = "Садриддин Айнӣ", Pages = 400, Quantity = 3 });
library.AddBook(new Book { Title = "Тоҷикон", Author = "Бобоҷон Ғафуров", Pages = 900, Quantity = 1 }); // Иловаи нусхаи иловагӣ

// Чопи рӯйхати китобҳо
library.ListBooks();

// Хориҷ кардани нусхаи китоб
library.RemoveBook("Тоҷикон");
library.ListBooks();

// Ҳисоб кардани миқдори умумии нусхаҳои китоб
Console.WriteLine($"Миқдори умумии 'Тоҷикон': {library.CountBooksByTitle("Тоҷикон")}");
```

---

**Намунаи баромад:**  
```
Book "Тоҷикон" added to the library.
Book "Адабиёти тоҷик" added to the library.
Increased quantity of "Тоҷикон" to 3.

Books in Library:
Тоҷикон by Бобоҷон Ғафуров, 900 pages (Copies: 3)
Адабиёти тоҷик by Садриддин Айнӣ, 400 pages (Copies: 3)

Decreased quantity of "Тоҷикон" to 2.

Books in Library:
Тоҷикон by Бобоҷон Ғафуров, 900 pages (Copies: 2)
Адабиёти тоҷик by Садриддин Айнӣ, 400 pages (Copies: 3)

Миқдори умумии 'Тоҷикон': 2
```

---
