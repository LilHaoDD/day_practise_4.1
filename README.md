# day_practise_4.1

#BMI的判断
height,weight = eval(input('请输入你的身高（米）和体重（kg）[逗号隔开]:'))
bmi = weight/height**2
print('BMI值是：{:.2f}'.format(bmi))
who,dom='',''
if bmi<18.5:
    who = '偏瘦'
elif bmi < 25:
    who = '正常'
elif bmi < 30:
    who = '偏胖'
else:
    who = '偏胖'
if bmi<18.5:
    dom = '偏瘦'
elif bmi < 24:
    dom = '正常
elif bmi < 28:
    dom = '偏胖'
else:
    dom = '肥胖'
print('你在国际标准下是{}，在中国的标准下是{}'.format(who,dom))'

a=(24<=28<25)
print(a)

import random
a=random.random()
b=random.randint(1,10)
c=random.uniform(1,10)
d=random.randrange(1,50,2)
e=random.choice(range(100))
ls = list(range(10))
print(ls)
f=random.shuffle(ls)
print(ls)
print(e)
print(d)
print(c)
print(b)
print(a)

#seed 使用
from random import *
a=random()
print(a)
seed(12)
print('{},{},{}'.format(randint(0,10),randint(0,10),randint(0,10)))
seed(15)
print('{},{},{}'.format(randint(0,10),randint(0,10),randint(0,10)))
seed(12)
print('{},{},{}'.format(randint(0,10),randint(0,10),randint(0,10)))

#practice
from random import *
ls1=[]
for i in range(10):
    a=randint(1,100)
    ls1.append(a)
b=randrange(1,100,2)
c=sample('abcdefghij',4)
ls = ['apple','pear','peach','orange']
d=choice(ls)
print(ls1,b,c,d)

#求Π
import random
import math
n = 0
a = eval(input('请输入点数='))
for i in range(a):
    x = random.random()
    y = random.random()
    dist = math.sqrt(x ** 2 + y ** 2)
    if dist <= 1.0:
        n += 1
pai = 4 * n / a
print(pai)
