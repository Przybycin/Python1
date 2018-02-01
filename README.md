# Python1
Playing around with Python

/* breaking a while loop prematurely */

i = 0
while 1 == 1:
  print(i)
  i = i + 1
  if i >= 5:
    print("Breaking")
    break
    
  print("Finished")
  

// example ///


i = 5
  print(i)
  i = i - 1
  if i <= 2:
    break  // will print out 3 numbers //
    
/* continue loop, loops from top to bottom and repeats */

i = 0
while True:
  i = i + 1
  if i == 2:
    print("Skipping 2")
    continue
  if i == 5:
    print("Breaking")
    break
  print(i)
  
print("Finished")  /* Result = 1, 
                               Skipping 2, 
                               3, 
                               4, 
                               Breaking, 
                               Finished */

/* Lists (AKA Arrays) */

words = ["Hello", "world", "!"]
print(words[0])
print(words[1])
print(words[2])  /* Result = Hello
                             world
                             !
                             >>> */
                             
// Another example //

nums = [5, 4, 3, 2, 1,] 
print(nums[1]) /* Result = 4, from left to right will be 0, 1, 2, 3, 4
                                                         5, 4, 3, 2, 1 and [2] alone contains only 1 object */
                                                         
/* Lists can be nested within other lists... due to the fact that there is no multidimensional array option */

number = 3
things = ["string", 0, [1,2, number], 4.56]
print(things[1])
print(things[2])
print(things[2][2])  /* Result = 0
                                 [1, 2, 3]
                                 3  */
                                        
/* strings can be indexed like lists... */

str = "Hello world!"
print(str[6])  /* Result = w  */

/* in addition, the item at a certain index in a list can be reassigned... */

nums = [7, 7, 7, 7, 7]
nums[2] = 5
print(nums)  /* Result = [7, 7, 5, 7, 7]  remember to start counting at 0, left to right!  */

// multiplying strings etc... //

nums = [1, 2, 3]
print(nums + [4, 5, 6])
print(nums * 3)  /* Result = [1, 2, 3, 4, 5, 6]
                             [1, 2, 3, 1, 2, 3, 1, 2, 3] */

/* To check if an item is in a list, the "in" operator is used. It returns True if the item occurs one or more times in the list, and False if it doesn't... */

words = ["ham", "eggs", "ham", "sausage"]
print("ham" in words)
print("eggs" in words)
print("mushroom" in words)  /* Results = True 
                                         True
                                         False  */
                                         
/* To check if an item is NOT in a list, use the "not" operator... */

nums = [1, 2, 3]
print(not 4 in nums)
print(4 not in nums)
print(not 3 in nums)
print(3 not in nums)  /* Result = True 
                                  True
                                  False
                                  False  */
                                  
/* The append method adds an item to the end of an existing list... */

nums = [1, 2, 3]
nums.append(4)
print(nums)  /*  Result = [1, 2, 3, 4]  */

/* The "len" function will display the number of items in a list... */

nums = [1, 2, 5, 3, 4]
print(len(nums))  /*  Result = 5  */

/* The "insert" method is similar to append, though it allows you to insert a new item in any position of the list, not just at the end... */

words = ["Python", "fun"]
index = 1
words.insert(index, "is")
index = 2
words.insert(index, "very")
index = 3 
words.insert(index, "p.s the quotation marks are not an attempt at irony")
print(words)  /*  Result = ['Python', 'is', 'very', 'fun', 'p.s the quotation marks are not an attempt at irony']  */

/* The "index" method finds the first occurrence of a list item and returns its position... */

letters = ['p', 'q', 'r', 's', 'p', 'u']
print(letters.index('r'))
print(letters.index('p'))
print(letters.index('z'))  /*  Result = 2
                                        0
                                        ValueError: 'z' is not in list  */
                                        
/* Other useful functions include:  max(list) Returns the list items with the maximum value
                                    min(list) Returns the list items with the minimum value
                                    list.count(obj) Returns a count of how many times an item occurs in a list
                                    list.remove(obj) Removes an object from a list
                                    list.reverse() Reverses objects in a list  */
                                    
// Range //
