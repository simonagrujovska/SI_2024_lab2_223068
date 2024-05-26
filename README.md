# Втора лабораториска вежба по Софтверско инженерство
## Симона Грујовска 223068
### Control Flow Graph
![SI_223068](https://github.com/simonagrujovska/SI_2024_lab2_223068/assets/166875334/69c70634-b05e-4db1-bbb6-0afc6a2b866a)
### Цикломатска комплексност
Цикломатската комплексност на овој код е 10, истата ја добив преку формулата  за предикатни јазли 
P(број на предикатни јазли)+1, во овој случај има 9 предикатни јазли + 1 = 10
### Тест случаи за Multiple Condition критериумот за условот if (item.getPrice() > 300 && item.getDiscount() > 0 && item.getBarcode().charAt(0) == '0').

![Screenshot 2024-05-26 204546](https://github.com/simonagrujovska/SI_2024_lab2_223068/assets/166875334/e4c264b6-2538-460b-b329-241940bd76eb)

### Објаснување на тест случаи за Multiple Condition критериумот:

allItems = [Item(Name = ABCD, Barcode = 012345, Price = 333, Discount = 0.5)], payment = 111

Со овој тест условите во if условот би биле true && true && true и програмата ќе продолжи да се извршува во if условот.

allItems = [Item(Name = ABCD, Barcode = 34567, Price = 333, Discount = 0.5)], payment = 111

Со овој тест условите во if условот би биле true && true && false и програмата нема да продолжи да се извршува во if условот.

allItems = [Item(Name = ABCD, Barcode = 34567, Price = 333, Discount = -1)], payment = 111

Со овој тест условите во if условот би биле true && false && false и програмата нема да продолжи да се извршува во if условот.

allItems = [Item(Name = ABCD, Barcode = 34567, Price = 222, Discount = -1)], payment = 111

Со овој тест условите во if условот би биле false && false && false и програмата нема да продолжи да се извршува во if условот.

