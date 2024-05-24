Tamara Dimchevska 223158

2.Control Flow Graph:
![CFG](https://github.com/TamaraDimcevska/-SI_2024_lab2_223158/assets/166861848/ea38ce18-6976-4557-a502-e9caaa7bcc3c)

3.Цикломатска комплексност:
Цикломатската комплексност на кодот е 10, ја добив преку формулата P+1, каде P е бројот на предикатни јазли. Во овој случај бројот на предикатни јазли е 9,па цикломатската комплексност изнесува 10.

4.Тест случаи според критериумот Every branch:
Item("Кабел", "0123", 150, 5.0), payment = -100
Item("Телефон", "1234", 200, 10.0), payment = 150
Item("Лаптоп", "ABC", 1000, 20.0), payment = -800
Item("Книга", "A123", 200, 10.0), payment = 100
Item("Пенкало", "5234", 400, 15.0), payment = 300

5.Тест случаи според критериумот Multiple Condition:
T && T && T
item.getPrice() >= 300, item.getDiscount() > 0, item.getBarcode().charAt(0) == '0'
T && T && F
item.getPrice() >= 300, item.getDiscount() > 0, item.getBarcode().charAt(0) != '0'
T && F && T
item.getPrice() >= 300, item.getDiscount() <= 0, item.getBarcode().charAt(0) == '0'
T && F && F
item.getPrice() >= 300, item.getDiscount() <= 0, item.getBarcode().charAt(0) != '0'
F && T && T
item.getPrice() < 300, item.getDiscount() > 0, item.getBarcode().charAt(0) == '0'
F && T && F
item.getPrice() < 300, item.getDiscount() > 0, item.getBarcode().charAt(0) != '0'
F && F && T
item.getPrice() < 300, item.getDiscount() <= 0, item.getBarcode().charAt(0) == '0'
F && F && F
item.getPrice() < 300, item.getDiscount() <= 0, item.getBarcode().charAt(0) != '0'
