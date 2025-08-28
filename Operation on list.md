# Operation on list

#### *Create a list*


```python
list1=[10,20,30,40]
list2=["Bala",18,"Logesh",20]
print("The list element is:",list)
print("The list element of different values:",list2)
```

    The list element is: [10, 20, 30, 40]
    The list element of different values: ['Bala', 18, 'Logesh', 20]
    

#### *Insert element*


```python
list1=[10,20,30,40]
list2=["Bala",18,"Logesh",20]
list1.insert(2,60)
list2.insert(2,"Jeyasheelan")
print("After Insert of the element:",list1)
print("After Insert of the element:",list2)
```

    After Insert of the element: [10, 20, 60, 30, 40]
    After Insert of the element: ['Bala', 18, 'Jeyasheelan', 'Logesh', 20]
    

#### *Append element*


```python
list1=[10,20,30,40]
list2=["Bala",18,"Logesh",20]
list1.append(40)
list2.append("Jeyasheelan")
print("After Append:",list1)
print("After Append:",list2)
```

    After Append: [10, 20, 30, 40, 40]
    After Append: ['Bala', 18, 'Logesh', 20, 'Jeyasheelan']
    

#### *Update element*


```python
list1=[10,20,30,40]
list2=["Bala",18,"Logesh",20]
list1[1]=99
list2[2]="Jeyasheelan"
print("After Update:",list1)
print("After Update:",list2)
```

    After Update: [10, 99, 30, 40]
    After Update: ['Bala', 18, 'Jeyasheelan', 20]
    

#### *Delete element by index & value*


```python
list1=[10,20,30,40]
del list1[0]
print("After deletion (By index):",list1)
list2=[10,20,30,40]
list2.remove(40)
print("After deletion (By value):",list2)

```

    After deletion (By index): [20, 30, 40]
    After deletion (By value): [10, 20, 30]
    

#### *Concatenate with another list*


```python
list1=[10,20,30,40]
list2=["Bala",18,"Logesh",20]
concatenate=list1+list2
print("Concatenated list:",concatenate)
```

    Concatenated list: [10, 20, 30, 40, 'Bala', 18, 'Logesh', 20]
    

#### *Length of the list*


```python
list1=[10,20,30,40]
print("The lengthh of the list is:",len(list1))
```

    The lengthh of the list is: 4
    

#### *Copy the list*


```python
list1=[10,20,30,40]
copy_list=list1.copy()
print("Copied list:",copy_list)
```

    Copied list: [10, 20, 30, 40]
    

# Operation on tuple

#### *Create a tuple*


```python
tuple=(10,20,30,40,50)
print(tuple)
```

    (10, 20, 30, 40, 50)
    

#### *Print a element by indexing*


```python
tuple=(10,20,30,40,50)
print("The element of the tuple is:",tuple)
```

    The element of the tuple is: (10, 20, 30, 40, 50)
    

#### *Slicing a element*


```python
tuple=(10,20,30,40,50)
print("After slicing a element:",tuple[1:4])

```

    After slicing a element: (20, 30, 40)
    

#### *Concatenate a tuple with another tuple*


```python
tuple1=(1,2,3)
tuple2=(4,5,6)
con=tuple1+tuple2
print("Concatenate of tuple:",con)
```

    Concatenate of tuple: (1, 2, 3, 4, 5, 6)
    

#### *Repetation*


```python
t=(10,20)
print("Repetation of the tuple:",t*3)

```

    Repetation of the tuple: (10, 20, 10, 20, 10, 20)
    

#### *Membership*


```python
t=(10,20,30)
print(20 in t)
```

    True
    

#### *Length*


```python
t=(10,20,30,40)
print("The length of the tuple is:",len(t))
```

    The length of the tuple is: 4
    

#### *Min & Max*


```python
tuple=(1,5,7,3,9)
print("The maximum number of the tuple is:",max(tuple))
print("The lowest number of the tuple is:",min(tuple))
```

    The maximum number of the tuple is: 9
    The lowest number of the tuple is: 1
    

#### *Count*


```python
t=(1,2,4,6,2,7,8,2,1,7)
num=t.count(2)
print("The number of element present in tuple is:",num)
```

    The number of element present in tuple is: 3
    

# Operation on Set

#### *Create a set*


```python
set={1,2,3,4,5}
print("set element:",set)
```

    set element: {1, 2, 3, 4, 5}
    

#### *Adding An Element*



```python
set={1,2,3,4,5}
set.add(6)
print("After adding an element:",set)
```

    After adding an element: {1, 2, 3, 4, 5, 6}
    

#### *Removing An Element*


```python
set={1,2,3,4,5}
set.remove(2)
print("After Remove:",set)
```

    After Remove: {1, 3, 4, 5}
    

#### *Union (A∪B)*


```python
set1={1,2,3,4}
set2={3,4,5,6}
print("Union:",set1|set2)
```

    Union: {1, 2, 3, 4, 5, 6}
    

#### *Intersection (A∩B)*


```python
set1={1,2,3,4}
set2={3,4,5,6}
print("Intersection:",set1&set2)
```

    Intersection: {3, 4}
    

#### *Difference (A-B)*


```python
set1={1,2,3,4}
set2={3,4,5,6}
print("Difference:",set1-set2)
```

    Difference: {1, 2}
    

#### *Symmetric Difference (A△B)*


```python
set1={1,2,3,4}
set2={3,4,5,6}
print("Symmetric Difference:",set1-set2)
```

    Symmetric Difference: {1, 2}
    

#### *Set Relations*


```python
set1={1,2,3}
set2={1,2,3,4,5}
print("Set1 is subset of Set2:",set1.issubset(set2))
print("Set2 is subset of Set1:",set2.issubset(set1))
print("Set2 is superset of Set1:",set2.issuperset(set1))
print("Set1 is disjoint with{6,7}:",set1.isdisjoint({6,7}))
```

    Set1 is subset of Set2: True
    Set2 is subset of Set1: False
    Set2 is superset of Set1: True
    Set1 is disjoint with{6,7}: True
    

#### *Length*


```python
set={1,2,3,4,5}
print("Length:",len(set))
```

    Length: 5
    

# Operations on Dictionary

#### *Create a Dictionary*


```python
dict={"Name":"Bala","Age":19,"City":"Thanjavur"}
print("Dictionary:",dict)
```

    Dictionary: {'Name': 'Bala', 'Age': 19, 'City': 'Thanjavur'}
    

#### *Accessing Element*


```python
dict={"Name":"Bala","Age":19,"City":"Thanjavur"}
print("Name:",dict["Name"])
```

    Name: Bala
    

#### *Updating*


```python
dict={"Name":"Bala","Age":19,"City":"Thanjavur"}
dict["Age"]=20
print("After upating age:",dict)
```

    After upating age: {'Name': 'Bala', 'Age': 20, 'City': 'Thanjavur'}
    

#### *Adding element*


```python
dict={"Name":"Bala","Age":19,"City":"Thanjavur"}
dict["College"]="PMIST"
print("After adding:",dict)
```

    After adding: {'Name': 'Bala', 'Age': 19, 'City': 'Thanjavur', 'College': 'PMIST'}
    

#### *Removing Elements*



```python
dict={"Name":"Bala","Age":19,"City":"Thanjavur"}
dict.pop("City")
print("After pop:",dict)
```

    After pop: {'Name': 'Bala', 'Age': 19}
    

#### *Loop Through Dictionary*


```python
dict={"Age":19,"City":"Thanjavur"}
print("Keys:")
for i in dict.keys():
    print(i)
```

    Keys:
    Age
    City
    

#### *Dictionary Methods*


```python
dict={"Name":"Bala","Age":19,"City":"Thanjavur"}
print("Keys:",dict.keys())
print("Values:",dict.values())
print("Items:",dict.items())
```

    Keys: dict_keys(['Name', 'Age', 'City'])
    Values: dict_values(['Bala', 19, 'Thanjavur'])
    Items: dict_items([('Name', 'Bala'), ('Age', 19), ('City', 'Thanjavur')])
    
