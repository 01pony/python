# python-bingo
def n(num1,num2):
    if num1<num2:
        print ('too small')
        return False
    elif num1>num2:
        print ('too big')
        return False
    else :
        print ('BINGO!')
        return True

from random import randint
num = randint(1,11)
print('Guess how old is me in 1-11.')
bingo = False
while bingo == False:
    answer = int(input())
    bingo = n(answer,num)
