# Итак, это мои ответы на билеты по проге 2020

## 1. Компиляция и интерпретация. Особенности синтаксиса языка в последних версиях.

### [Compilation](https://www.geeksforgeeks.org/compilation-execution-java-program/)

### Java editions

Java SE = Standard Edition. This is the core Java programming platform. It contains all of the libraries and APIs that any Java programmer should learn (java.lang, java.io, java.math, java.net, java.util, etc...).

Java EE = Enterprise Edition. From Wikipedia:

> The Java platform (Enterprise Edition) differs from the Java Standard Edition Platform (Java SE) in that it adds libraries which provide functionality to deploy fault-tolerant, distributed, multi-tier Java software, based largely on modular components running on an application server.

In other words, if your application demands a very large scale, distributed system, then you should consider using Java EE. Built on top of Java SE, it provides libraries for database access (JDBC, JPA), remote method invocation (RMI), messaging (JMS), web services, XML processing, and defines standard APIs for Enterprise JavaBeans, servlets, portlets, Java Server Pages, etc...

Java ME = Micro Edition. This is the platform for developing applications for mobile devices and embedded systems such as set-top boxes. Java ME provides a subset of the functionality of Java SE, but also introduces libraries specific to mobile devices. Because Java ME is based on an earlier version of Java SE, some of the new language features introduced in Java 1.5 (e.g. generics) are not available.

## 2. Приложения. Жизненный цикл. Передача параметров.

### [Types of Java Program](https://www.quora.com/What-are-the-types-of-Java-Program)

### [Life cycle](https://www.startertutorials.com/corejava/life-cycle-java-program.html)

### [Parameters](https://docs.oracle.com/javase/tutorial/java/javaOO/arguments.html)

## 3. Классы. Инкапсуляция. Поля. Статические поля.

### [Classes and Objects](https://www.tutorialspoint.com/java/java_object_classes.htm)

### Encapsulation

In object-oriented programming, encapsulation refers to the bundling of data with the methods that operate on that data, or the restricting of direct access to some of an object's components

### Static fields

Static variables or fields belong to the class, and not to any object of the class. A static variable is initialized when the class is loaded at runtime. Non-static fields are instance fields of an object. They can only be accessed or invoked through an object reference. The value of static variable remains constant throughout the class. The value of Non-static variables changes as the objects has their own copy of these variables.

```
class a

{

   static int n1=5, n2=6;

   static

   {

       System.out.println("A class static block");

   }

   static void m()

   {

       System.out.println("A class method");

   }

}

class b

{

   int n3=50;

   char n4='a';

   void m1()

   {

       System.out.println("B class method");

   }

   public static void main(String args[])

   {
       // static variables are accessed directly by giving the class reference in other class

       System.out.println(a.n1);

       System.out.println(a.n2);

       a.m();

       b obj=new b();//non-static variables are accessed with the help of class object

       System.out.println(obj.n3);

       System.out.println(obj.n4);

       obj.m1();

   }

}
```

## 4. Методы. Локальные переменные. Методы с переменным количеством аргументов. Статические методы.

### [Methods](https://www.tutorialspoint.com/java/java_methods.html)

### [Local variables](https://www.dummies.com/programming/java/local-variables-in-java/)

### [Varargs](https://docs.oracle.com/javase/1.5.0/docs/guide/language/varargs.html)

### [Everything about static keyword](https://www.javatpoint.com/static-keyword-in-java)

## 5. Примитивные типы данных и операции над ними. Приведение типов. Классы-оболочки.

### [Primitive data types](https://docs.oracle.com/javase/tutorial/java/nutsandbolts/datatypes.html)

### [Type casting](https://www.w3schools.com/java/java_type_casting.asp)

### [Wrapper class](https://www.javatpoint.com/wrapper-class-in-java)

## 6. Условные конструкции. Циклы.

### [Control flow statements](https://docs.oracle.com/javase/tutorial/java/nutsandbolts/flow.html)

## 7. Классы: наследование, полиморфизм. Конструкторы. Приведение типов.

### [Inheritance](https://docs.oracle.com/javase/tutorial/java/IandI/subclasses.html)

## 8. Иерархия классов исключительных ситуаций. Генерация и обработка исключительных ситуаций.

### [Excepions](https://www.tutorialspoint.com/java/java_exceptions.htm)

## 9. Интерфейсы. Абстрактные классы. Сравнение.

### [Abstract class vs Interface](https://beginnersbook.com/2013/05/abstract-class-vs-interface-in-java/)

## 10. Пакеты. Модификаторы доступа к полям, методам, классам (public, …)

### [Packages](https://www.tutorialspoint.com/java/java_packages.htm)

### [Access modifiers](https://www.javatpoint.com/access-modifiers)

## 11. Использование final. Правила именования полей, методов, классов, пакетов.

### [Final keyword](https://www.javatpoint.com/final-keyword)

### [Java naming convensions](https://www.javatpoint.com/java-naming-conventions)

## 12. Массивы. Алгоритмы обработки массивов. Цикл for-each.

### [Arrays](https://www.tutorialspoint.com/java/java_arrays.htm)

## 13. Строковые типы.

### [Strings](https://docs.oracle.com/javase/tutorial/java/data/strings.html)

## 14. Параметризованные классы, интерфейсы, методы. Ограничения использования.

### [Generics](https://www.tutorialspoint.com/java/java_generics.htm)

## 15. Перечисления.

### [https://docs.oracle.com/javase/tutorial/java/javaOO/enum.html](https://docs.oracle.com/javase/tutorial/java/javaOO/enum.html)

## 16. События. Модель обработки событий. Слушатели и адаптеры.

### [Event handling](https://www.tutorialspoint.com/swing/swing_event_handling.htm)

## 17. Обзор библиотеки компонентов JFC Swing.

### [Swing](https://www.javatpoint.com/java-swing)

## 18. Технология Model – View – Controller. Компоненты JList, JTree, JTable.

### [MVC](https://stackoverflow.com/questions/5217611/the-mvc-pattern-and-swing#5217977)

## 19. Способы компоновки.

### [Layouts](https://docs.oracle.com/javase/tutorial/uiswing/layout/visual.html)

## 20. Вложенные и внутренние классы. Анонимные классы.

### [Inner class](https://www.tutorialspoint.com/java/java_innerclasses.htm)

### [Anonymous class](https://docs.oracle.com/javase/tutorial/java/javaOO/anonymousclasses.html)

## 21. Структуры данных: коллекции. Цикл for-each.

### [Collections](https://www.javatpoint.com/collections-in-java)

## 22. Структуры данных: карты.

### [Map](https://www.tutorialspoint.com/java/java_map_interface.htm)

## 23. Стандартные алгоритмы обработки коллекций.

### [Algorithms](https://docs.oracle.com/javase/tutorial/collections/algorithms/index.html)

## 24. Итераторы и компараторы.

### [Iterator](https://www.tutorialspoint.com/java/java_using_iterator.htm)

### [Comparator](https://www.tutorialspoint.com/java/java_using_comparator.htm)

## 25. Задачи XML и HTML. Преимущества и недостатки.

### [XML vs HTML](https://www.javatpoint.com/html-vs-xml)

## 26. Структура XML-документа. Комментарии, текстовые блоки.

### [XML structure](https://www.tutorialspoint.com/xml/xml_documents.htm)

## 27. Структура XML-документа. Пространства имен.

### [XML - Namespaces](https://www.tutorialspoint.com/xml/xml_namespaces.htm)

## 28. Разбор XML. Технология DOM.

### [DOM](https://www.tutorialspoint.com/java_xml/java_dom_parser.htm)

## 29. Разбор XML. Технология SAX.

### [SAX](https://www.tutorialspoint.com/java_xml/java_sax_parser.htm)

## 30. XML-схемы. Простые типы. Проверка корректности XML.

### [Validation](https://www.tutorialspoint.com/xml/xml_validation.htm)

## 31. XML-схемы. Сложные типы. Проверка корректности XML.

### [XML Syntax](https://www.tutorialspoint.com/xml/xml_validation.htm)

## 32. WWW. Понятие URI. Типичная структура узла.

### WWW

The World Wide Web, commonly known as the Web, is an information system where documents and other web resources are identified by Uniform Resource Locators, which may be interlinked by hypertext, and are accessible over the Internet

### [URI](https://en.wikipedia.org/wiki/Uniform_Resource_Identifier)

## 33. Рекомендации для проектирования сайта.

## 34. Структура HTML-документа. Заголовок HEAD.

### [HTML Intro](https://www.w3schools.com/html/html_intro.asp)

## 35. HTML: заголовки, абзацы, списки.

## 36. HTML: таблицы, изображения, гиперссылки.

## 37. HTML-формы. Методы POST и GET.

## 38. Стили в HTML.

### [HTML styles](https://www.w3schools.com/html/html_styles.asp)

## 39. Текстовый формат обмена данными JSON. 

### [JSON](https://www.tutorialspoint.com/json/json_overview.htm)
