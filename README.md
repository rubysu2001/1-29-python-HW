# 1-29HW_python

def list_arr(num):
  for i in range (len(num)):
      for j in range (len(num)-i-1):
        if num[j] < num[j+1]:
          num[j] , num[j+1] = num[j+1] , num[j]
  return num


arr = input("")
num = [int(n) for n in arr.split()]
print(list_arr(num))
