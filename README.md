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

