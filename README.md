import math
def add(x, y):
    return x + y
def subtract(x, y):
    return x - y
def multiply(x, y):
    return x * y
def divide(x, y):
    if y == 0:
        return "Ошибка: деление на ноль"
    return x / y
def power(x, y):
    return x ** y
print("Выберите операцию:")
print("1. Сложение")
print("2. Вычитание")
print("3. Умножение")
print("4. Деление")
print("5. Возведение в степень")
choice = input("Введите номер операции (1/2/3/4/5): ")
num1 = float(input("Введите первое число: "))
num2 = float(input("Введите второе число: "))
if choice == '1':
    print(f"Результат: {add(num1, num2)}")
elif choice == '2':
    print(f"Результат: {subtract(num1, num2)}")
elif choice == '3':
    print(f"Результат: {multiply(num1, num2)}")
elif choice == '4':
    print(f"Результат: {divide(num1, num2)}")
elif choice == '5':
    print(f"Результат: {power(num1, num2)}")
else:
    print("Ошибка: некорректный ввод")
