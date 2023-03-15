import json
import time
with open('scena.json', 'r', encoding='utf-8') as scena_file:
    scena = json.load(scena_file)
sch = 0
k_scena = scena["Ключи"]
otv = 10
place = ''
while place == '':
    if otv == 0:
        break
    for el in scena[k_scena[sch]]:
        print(el)
        time.sleep(3)
    if sch == 1 or sch == 3 or sch == 4 or sch == 6 or sch == 8 or sch == 9:
        place = 'Конец!'
        break
    elif k_scena[sch] == "Далее":
        print('Выбирай')
        print(f'1. {k_scena[sch + 1]}; 2. {k_scena[sch + 2]}; 3. {k_scena[sch + 3]}')
        print(f'0. Хочу закончить')
        otv = int(input())
    else:
        print('Выбирай')
        print(f'1. {k_scena[sch + 1]}; 2. {k_scena[sch + 2]}')
        print(f'0. Хочу закончить')
        otv = int(input())
    sch += otv
