### **Разбор задачи**

Эта задача стала продолжением работы со строковыми методами — на этот раз с преобразованием в нижний регистр.

**Что нужно было сделать**
- Имеем резюме с заглавными буквами в нескольких строках
- Нужно привести все к нижнему регистру
- Не изменяя исходные переменные `title`, `degree`, `career`
- Использовать метод `toLowerCase()`

**Как я решал**

Применил `toLowerCase()` к каждой выводимой строке. Для строк с конкатенацией использовал скобки, чтобы метод применялся ко всему выражению.

**Проверил себя по пунктам**
- Исходные переменные остались неизменными
- Ко всем четырем выводам применен `toLowerCase()`
- Для составных строк правильно сгруппированы операции
- Метод корректно обработал все заглавные буквы

**Где можно затупить**
- Применить метод только к части выражения (без скобок)
- Перепутать порядок вывода строк

**Финальный код**
```java
public class Solution {
    public static void main(String[] args) {
        String title = "Senior Lead Principal Software Engineer Data Architect";
        String degree = "In college, I Majored in Political Science and Minored in Religious Studies.";
        String career = "Experienced Team Leader with strong Organizational Skills and a Successful career in Management.";
        
        System.out.println("RESUME".toLowerCase());
        System.out.println(("TITLE: " + title).toLowerCase());
        System.out.println(("DEGREE: " + degree).toLowerCase());
        System.out.println(("CAREER: " + career).toLowerCase());
    }
}
```

**Что понял**
1. **Метод toLowerCase()** — преобразует строку в нижний регистр
2. **Симметрия методов** — toLowerCase() и toUpperCase() работают аналогично
3. **Группировка выражений** — скобки обязательны для сложных конкатенаций

Решение прошло проверку. Похоже, методы работы со строками постепенно становятся привычным инструментом.
