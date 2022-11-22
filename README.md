# csci-101-102-labs
def load_file(file_name):
  with open (file_name, 'r') as file:
    word_list = []
    for i in file:
      i = i[:-1]
      word_list.append(i)
  return word_list
  
def update_string(og_string,new_string,index):
  first_half = og_string[:index]
  second_half = og_string[index+1:]
  new_word = first_half + new_string + second_half
  print(f'OUTPUT {new_word}')
  
def find_word_count(list, word):
  count = 0
  for i in list:
    occurences = i.count(word)
    count = count + occurences
  print(count)

def score_finder(names,scores,target_name):
  count = 0
  location = 'x'
  target_name.lower()
  for i in names:
    n = i.lower()
    if n == target_name:
      location = count
    count += 1
  if str(location) in '012345689':
    print(f'OUTPUT {players[location]} got a score of {scores[location]}')
  else:
    print('OUTPUT player not found')
   
def union(list1,list2):
  for i in list2:
    list1.append(i)
  print(list1)
  
def intersect(list1,list2):
  newlist = []
  for i in list1:
    if i in list2:
      newlist.append(i)
  print(newlist)
  
def not_in(list1,list2):
  newlist = []
  for i in list1:
    if i not in list2:
      newlist.append(i)
  print(newlist)
  
import math 
def is_prime(num):
  state = 'True'
  if num <= 1:
    state = 'False'
  upper_lim = int(math.sqrt(num) + 1)
  for i in range(2, upper_lim):
    if num % i == 0:
      state = 'False'
  print(state)
