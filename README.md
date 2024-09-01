# #Угдайка даты рождения
import time
import turtle


def mounts(x):
    if x == '01': return 'январь'
    elif x == '02': return 'февраль'
    elif x == '03': return 'март'
    elif x == '04': return 'апрель'
    elif x == '05': return 'май'
    elif x == '06': return 'июнь'
    elif x == '07': return 'июль'
    elif x == '08': return 'август'
    elif x == '09': return 'сентябрь'
    elif x == '10': return 'октябрь'
    elif x == '11': return 'ноябрь'
    elif x == '12': return 'декабрь'
for i in 'Здравствуйте дамы и господа!':
    print(i, end='')
    time.sleep(0.1)
print()
for i in range(3):
    for i in range(3):
        print('.',end = '')
        time.sleep(0.2)
    print('⌛')
    time.sleep(0.1)
time.sleep(1)
for i in 'Хочу предложить вам поучавствовать в фокусе!':
    print(i, end='')
    time.sleep(0.1)
print()
for i in range(10):
    time.sleep(0.3)
    print('.',end = '')
time.sleep(1)
print()
for i in 'Готовы ли вы':
    print(i,end = '')
    time.sleep(0.4)
for i in range(5):
    print('?',end = '')
    time.sleep(0.4)
print('')
print('Скажите "Да или "Нет"')
s = input().lower()
if s == 'да':
    for i in 'Отлично, начнем!':
        print(i,end = '')
        time.sleep(0.1)
    time.sleep(1)
else:
    print('Ох',end='')
    for i in range(5):
        print('.',end = '')
        time.sleep(0.3)
    print()
    for i in 'К сожалению, но вы отказались.':
        print(i,end = '')
        time.sleep(0.1)
    time.sleep(1)
    print()
    print('Спасибо за внимание!')
    exit()
time.sleep(0.5)
print()
for i in 'Для начала, умножте день своего  рождения на 2':
    print(i, end='')
    time.sleep(0.2)

print()
for i in range(5):
    print('⌛',end = '')
    time.sleep(0.3)
time.sleep(1)
print()
print('Продолжаем?')
div1 = input()
if div1.lower() == 'да':
    pass
else:
    print('Отлично, вы отказались.')
    exit()

time.sleep(0.5)
for i in 'Замечательно!':
    print(i, end='')
    time.sleep(0.1)
print()
for i in range(5):
    print('⌛',end = '')
print()

for i in 'Далее получившееся число, сложи с пятеркой и после умножь на 50':
    print(i, end='')
    time.sleep(0.3)
print()
for i in 'Осталось последнее':
    print(i, end='')
    time.sleep(0.2)

print()

for i in 'К результату прошлых действий, прибавь месяц своего рождения и наблюдай магию!!':
    print(i, end='')
    time.sleep(0.1)


print()
for i in range(5):
    print('⌛',end = '')
    time.sleep(0.3)
time.sleep(1)
print()

for i in 'Напиши мне число, которое получилось после всех расчетов ':
    print(i, end='')
    time.sleep(0.1)
print()
num = input()

result = int(num) - 250
result = str(result)
print()
for i in range(5):
    print('⌛',end = '')
    time.sleep(0.3)
time.sleep(1)
print()
for i in "А вот что у нас получилось в итоге":
    print(i, end='')
    time.sleep(0.2)
print()
for i in f"День твоего рождения:{int(result[0:2])}, а месяц:{mounts(result[2:])}":
    print(i, end='')
    time.sleep(0.1)
print()
time.sleep(0.5)
print()
time.sleep(1)
print('\n'.join(' '.join(*zip(*row)) for row in ([["♥" if row==0 and col%3!=0 or row==1 and col%3==0 or row-col==2 or row+col==8 else " " for col in range(7)] for row in range(6)])))
