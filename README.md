### Часть 1 https://github.com/Kokunov777/User_interfce
### часть 3 

 # Лабораторная работа 2: Разработка лексического анализатора (сканера)

## Цель работы
Изучить назначение и принципы работы лексического анализатора в структуре компилятора. Спроектировать алгоритм (диаграмму состояний) и выполнить программную реализацию сканера для выделения лексем из входного текста. Интегрировать разработанный модуль в ранее созданный графический интерфейс языкового процессора.

## Сведения об авторе
- **ФИО**: kokunov Andrey
- **Группа**: АВТ 313
- **Дата**: 2026 год

## Постановка задачи
Разработать лексический анализатор (сканер) в соответствии с индивидуальным вариантом задания, интегрировать его в приложение из лабораторной работы №1 и обеспечить наглядный вывод результатов.

## Вариант задания
**Вариант 5**: Объявление комплексного числа с инициализацией на языке Rust

## Диаграмма состояний
<img width="572" height="885" alt="image" src="https://github.com/user-attachments/assets/372be896-1504-4d6d-94d4-2cc33bc7f51f" />
<img width="472" height="539" alt="image" src="https://github.com/user-attachments/assets/71310039-1354-450d-85e2-64dc6305e038" />


## Тестовые примеры
### Пример 1: 
**Вход:** `let complex_num2 = num::complex::Complex::new(3.1, -4.2);`
<img width="538" height="897" alt="image" src="https://github.com/user-attachments/assets/e5e9ee1e-59e3-4ce2-ba8e-1025f31b2c9e" />



### Пример 2: Строка с недопустимым символом
**Вход:** `let x = @;`

<img width="471" height="428" alt="image" src="https://github.com/user-attachments/assets/bb9869d6-63c3-4af8-8529-c9a2b8e129bb" />

**Ошибки:**

<img width="476" height="193" alt="image" src="https://github.com/user-attachments/assets/6caa84cd-7c65-4d16-bace-c5f89fd060bb" />


### Пример 3: Многострочный пример
**Вход:**
```
let a = num::complex::Complex::new(1, 2);
let b = 3.14;
```
<img width="512" height="1131" alt="image" src="https://github.com/user-attachments/assets/626fa7cb-ce96-44e2-9c55-085bd4221d68" />

