import string
class HashFunction:
	people = 0

	def __init__(self,arr):
		self.arr = arr
		HashFunction.people += len(arr)
	def add(self):
		alphabet = list(string.ascii_lowercase)
		for i in self.arr:
			temp = str(i[0])
			hashvalue = alphabet.index(temp.lower())
			if hashmap[hashvalue] != None:
				hashmap[hashvalue] = list([hashmap[hashvalue]])
				hashmap[hashvalue].append(i)
			else:
				hashmap[hashvalue] = i
		print(hashmap)

	def length(self):
		print(HashFunction.people)

	def delete(self,word):
		i = str(word[0])
		alphabet = list(string.ascii_lowercase)
		hashvalue = alphabet.index(i.lower())
		if isinstance(hashmap[hashvalue],list):
			if word in hashmap[hashvalue]:
				hashmap[hashvalue].remove(word)
		else:
			if hashmap[hashvalue] == word:
				hashmap[hashvalue] = None
		print(hashmap)

	def exist(self,word):
		i = str(word[0])
		alphabet = list(string.ascii_lowercase)
		hashvalue = alphabet.index(i.lower())
		if isinstance(hashmap[hashvalue],list):
			if word in hashmap[hashvalue]:
				print('The word is in slot ' + str(hashvalue))
			else:
				print('The word you are looking fo does not exist')

		else:
			if hashmap[hashvalue] == word:
				print('The word is in slot ' + str(hashvalue))
			else:
				print('The word you are looking fo does not exist')

if __name__ == "__main__":
	hashmap = {}
	for i in range(26):
		hashmap[i] = None
	test = ['Jack','Jones','abby']
	x = HashFunction(test)
	x.add()
	x.delete('Jack')
	x.delete('abby')
	x.exist('Jones')
