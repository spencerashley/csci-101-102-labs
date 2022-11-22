# csci-101-102-labs
def load_file(file_name):
  with open (file_name, 'r') as file:
    word_list = []
    for i in file:
      i = i[:-1]
      word_list.append(i)
  return word_list
