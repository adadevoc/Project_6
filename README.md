# Project_6



import random

def sort(arr):
    n = len(arr)
    for i in range(n-1):
        for j in range(0, n-i-1):
            if arr[j] > arr[j + 1]:
                arr[j], arr[j + 1] = arr[j + 1], arr[j]
            print("{} {}".format(arr[i],arr[j]))

numbers=[]
for i in range(100):
    numbers.append(int((random.random()*100)))
sort(numbers)
