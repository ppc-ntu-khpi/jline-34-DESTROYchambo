# UI Lab 2 
![](terminal-icon.png)
![](gui-icon.png)

Це одна з робіт, які доповнюють основний цикл лабораторних робіт #1-8 (проект **Banking**, [Netbeans](https://netbeans.org/)) з ООП.  Основна мета цих додаткових вправ - познайомитись з різними видами інтерфейсів користувача та засобами їх створення. Згадувані 'базові' роботи розміщено в [окремому репозиторії](https://github.com/liketaurus/OOP-JAVA) (якщо будете робити завдання на "4" або "5" раджу переглянути [діаграму класів](https://github.com/liketaurus/OOP-JAVA/blob/master/MyBank.png), аби розуміти які методи є у класів).

В ході першої роботи вам пропонується виконати **наступне завдання** - [Робота 2: CLI з jline 3](https://github.com/ppc-ntu-khpi/TUI-Lab2-Starter/blob/master/Lab%202%20-%20CLI/Lab%202.md)
  
**Додаткове завдання** (для тих хто зробив все і прагне більшого): [дивіться тут](https://github.com/ppc-ntu-khpi/TUI-Lab2-Starter/blob/master/Lab%202%20-%20CLI/Lab%202%20-%20add.md)

Всі необхідні бібліотеки містяться у теці [jars](https://github.com/ppc-ntu-khpi/TUI-Lab2-Starter/tree/master/jars). В тому числі - всі необхідні відкомпільовані класи з робіт 1-8 - файл [MyBank.jar](https://github.com/ppc-ntu-khpi/TUI-Lab2-Starter/blob/master/jars/MyBank.jar). Файл даних лежить у теці [data](https://github.com/ppc-ntu-khpi/TUI-Lab2-Starter/tree/master/data).

---
## На "трійку"
1. Завантажте необхідні jar-файли - [jline](https://repo1.maven.org/maven2/org/jline/jline/3.10.0/jline-3.10.0.jar), [jansi](http://repo1.maven.org/maven2/org/fusesource/jansi/jansi/1.17.1/jansi-1.17.1.jar), [MyBank](https://github.com/liketaurus/TUI-Labs/blob/master/jars/MyBank.jar). Останній файл містить всі класи (*Bank, Customer, Account* та ін.) з наших попередніх лаб. *УВАГА! Також ви можете взяти всі три файли прямо з [цього ж репозиторію](https://github.com/liketaurus/TUI-Labs/blob/master/jars)*.
2. Створіть в Netbeans новий проект з назвою TUIdemo (або використайте проект, створений в ході виконання попередньої роботи). *УВАГА! Чекбокс *Create Main Class* треба **очистити** (**не створювати виконуваний клас**)!*
3. Додайте до проекту всі завантажені вами бібліотеки - правою кнопкой на проекті, обрати *Properties*, потім у дереві категорій обрати *Libraries* (другий пункт зверху), натиснути у правій частині вікна кнопку *Add JAR/Folder*, обрати jar-файли, завантажені у п. 1, натиснути *Ok*
4. Додайте до проекту файл **[CLIdemo.java](https://github.com/liketaurus/TUI-Labs/blob/master/Lab%202%20-%20CLI/CLIdemo.java)** з цього репозиторію
5. Вивчіть вихідний код у файлі, впевніться, що ви розумієте як він має працювати
6. Відкрийте консоль (під Linux - *емулятор терміналу*, під Windows - *PowerShell*), перейдіть до теки проекту (під Linux - ```cd NetBeansProjects/TUIDemo/dist```, під Windows - ```cd .\Documents\NetBeansProjects\TUIdemo\dist```). Запустіть проект (```java -jar .\TUIdemo.jar```) - ви маєте побачити запрошення (```bank>```). Натисніть **TAB** аби переглянути доступні команди. Натисніть <kbd>h</kbd> <kbd>TAB</kbd> <kbd>ENTER</kbd> аби переглянути довідку, <kbd>cus</kbd> <kbd>TAB</kbd> <kbd>s</kbd> <kbd>ENTER</kbd> аби переглянути список клієнтів банку, <kbd>Up</kbd> <kbd>Backspace</kbd> <kbd>Space</kbd> <kbd>1</kbd> <kbd>ENTER</kbd> аби переглянути інформацію про клієнта з номером 1, <kbd>Up</kbd> <kbd>2</kbd> <kbd>ENTER</kbd> аби впевнитись, що програма коректно обробляє неправильний номер клієнта, <kbd>e</kbd> <kbd>TAB</kbd> <kbd>ENTER</kbd> для виходу.Продемонстрируйте результат викладачеві.

![image](https://github.com/user-attachments/assets/6574e30c-fa41-482b-b824-01d719d54627)


## На "чотири"
1. Перепишіть код  так, щоб інформація про клієнтів банку та їх рахунки читалась з файлу **test.dat** (робота номер 8, [файл даних](https://github.com/liketaurus/TUI-Labs/blob/master/data/test.dat) також є в цьому ж репозиторію).
2. Запустіть проект, впевніться, що все працює як очікувалось. Продемонстрируйте результат викладачеві.

## На "п'ять"
1. Додайте ще одну команду - **report**, яка має виводити звіт за клієнтами такого ж виду, як у роботі номер 8 (див. CustomerReport).
2. Запустіть проект, впевніться, що все працює як очікувалось. Продемонстрируйте результат викладачеві.

![](https://img.shields.io/badge/Made%20with-JAVA-red.svg)
![](https://img.shields.io/badge/Made%20with-%20Netbeans-brightgreen.svg)
![](https://img.shields.io/badge/Made%20at-PPC%20NTU%20%22KhPI%22-blue.svg) 
[![Gitter](https://badges.gitter.im/PPC-SE-2020/OOP.svg)](https://gitter.im/PPC-SE-2020/OOP?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge)
