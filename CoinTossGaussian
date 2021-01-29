import numpy as np
import random
from random import randrange
import matplotlib.pyplot as plt

#pick a random number between 0 and 1, which we can call "flip"
def flip():
    result=randrange(2)
    return result
#set n= number of throws, iterations= number of times you repeat the procedure
n=400
total=np.arange(n)
iterations=4000

#create an empty storage list
store_list=[]

#iterate through trials and throws
for j in range (iterations):
    for i in range(0,n):
        total[i]=flip()
        i+=1
    np.count_nonzero(total == 1)
    store_list.append(np.count_nonzero(total == 1))
    #print(np.count_nonzero(total == 1)) (uncomment if you want to see output)

#print your output
plt.hist(store_list, bins = 100)
plt.show()

# THE FOLLOWING CODE IS A FROM https://www.geeksforgeeks.org/random-gauss-function-in-python/
#This code is to compare your output with a traditional gaussian function
nums = []
mu = 100
sigma = 50
for i in range(10000):
    temp = random.gauss(mu, sigma)
    nums.append(temp)
plt.hist(nums, bins = 100)
plt.show()
