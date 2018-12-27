# Rbn.py
# Monitering bank activity 

minimum = 1000000

name1 = 'x5hh8'

stone = int(input("Has " + name1 + " put 1m stone into the bank? "))

if stone == 1:

	print(name1 + " Has put 1m stone into the bank")

else:

	resultstone1 = minimum - stone

	print(name1 + " owes " + resultstone1 + "!")

wood = int(input("Has " + name1 + " put 1m wood into the bank? "))

if wood == 1:

	print(name1 + " Has put 1m wood into the bank")

else:

	resultwood1 = minimum - wood 

	print(name1 + " owes " + resultwood1 + "!") 

ore = int(input("Has " + name1 + " put 1m ore into the bank? "))

if ore == 1:

	print(name1 + " Has put 1m ore into the bank")

else:

	resultore1 = minimum - ore

	print(name1 + " owes " + resultore1 + "!")

gold = int(input("Has " + name1 + " put 1m gold into the bank? "))

if gold == 1:

	print(name1 + " Has put 1m gold into the bank")

else:

	resultgold1 = minimum - gold

	print(name1 + " owes " + resultgold1 + "!")

Details1 = stone + ", " + wood + ", " + ore + " and " + gold

print(Details1)
