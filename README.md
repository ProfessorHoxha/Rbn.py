# Rbn.py
# Monitering bank activity 

def logs():

	f = open("BANK_LOGS.txt", "a")

	minimum = 1000000
	maxmin = 4000000

	name1 = 'x5hh8'

	print("======================================================================================")

	stone = int(input("Has " + name1 + " put 1m stone into the bank? "))

	resultstone1 = minimum - stone

	if stone == 1:

		print(name1 + " Has put 1m stone into the bank")

	else:

		print(name1 + " owes " + str(resultstone1) + " stone!")

	wood = int(input("Has " + name1 + " put 1m wood into the bank? "))

	resultwood1 = minimum - wood

	if wood == 1:

		print(name1 + " Has put 1m wood into the bank")

	else:

		print(name1 + " owes " + str(resultwood1) + " wood!")

	ore = int(input("Has " + name1 + " put 1m ore into the bank? "))

	resultore1 = minimum - ore

	if ore == 1:

		print(name1 + " Has put 1m ore into the bank")

	else:

		print(name1 + " owes " + str(resultore1) + " ore!")

	gold = int(input("Has " + name1 + " put 1m gold into the bank? "))

	resultgold1 = minimum - gold

	if gold == 1:

		print(name1 + " Has put 1m gold into the bank")

	else:

		print(name1 + " owes " + str(resultgold1) + " gold!")

	Details1 = stone + wood + ore + gold

	Detail1 = int(maxmin) - (int(stone) + int(wood) + int(ore) + int(gold))

	if Details1 == 4:

		print(name1 + " Has payed off this weeks bank deposit!")

		print("======================================================================================")

	else:

		print(str(Detail1) + " is what " + str(name1) + "owes altogether!")

		print("======================================================================================")

	logs1 = (name1 + "\n" + Details1  + "\n" + Detail1 + "\nSecondary confirmation: \n" + stone + resultstone1 + "\n" + wood + resultwood1 + "\n" + ore + resultore1 + "\n" + gold + resultgold1 + "\n EXIT"

	f.write(logs1)

	f.close()

logs()	
