# Python_Lesson1
# Треугольник существует только тогда, когда сумма любых двух его сторон больше третьей. 
# Дано a, b, c - стороны предполагаемого треугольника. 
# Требуется сравнить длину каждого отрезка-стороны с суммой двух других. 
# Если хотя бы в одном случае отрезок окажется больше суммы двух других, то треугольника с такими сторонами не существует. 
# Отдельно сообщить является ли треугольник разносторонним, равнобедренным или равносторонним.


a = int(input(f'Сторона a : '))
b = int(input(f'Сторона b : '))
c = int(input(f'Сторона c : '))
if a == b == c:
    print('треугольник равносторонний')
    
elif a > b > c:
    print('треугольник разносторонний')
elif a == b or a == c or b == c: 
    print ('треугольник равнобедренный')
else:
    print('это не тругольник')

# Напишите код, который запрашивает число и сообщает является ли оно простым или составным. 
# Используйте правило для проверки: “Число является простым, если делится нацело только на единицу и на себя”. 
# Сделайте ограничение на ввод отрицательных чисел и чисел больше 100 тысяч.
MINIMAL = 0
MAXIMAL = 100000
number= float(input(f'Введите число от {MINIMAL} до {MAXIMAL}: '))
if number // number == 1 and number // 1 == number:
    print('введенное число простое')
else:
    print('число составное')

