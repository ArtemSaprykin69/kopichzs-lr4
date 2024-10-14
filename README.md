sort_odd_rows(arr1, arr2): 
     
    def sort_row(row):         return sorted(row, key=abs) 
 
     
    for i in range(len(arr1)):         if i % 2 != 0:             arr1[i] = sort_row(arr1[i]) 
 
     
    for i in range(len(arr2)):         if i % 2 != 0:             arr2[i] = sort_row(arr2[i]) 
 
    return arr1, arr2 
 
 
arr1 = [[1, 2, 3], [4, 5, 6], [7, 8, 9]] 
arr2 = [[10, 11, 12], [13, 14, 15], [16, 17, 18]] 
 
arr1, arr2 = sort_odd_rows(arr1, arr2) 
 
print("Массив 1:") for row in arr1:     print(row) 
 
print("Массив 2:") for row in arr2: 
    print(row) 
