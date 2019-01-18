# Rbn.py
# Monitering bank activity 
# Rbn alphebet; (stone,wood,ore,gold)

import time


def RBN_BANK():

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

	elif Details1 < 4:

		print(name1 + " still needs to deposit some more recourses but has been logged")

	else:

		print(str(Detail1) + " is what " + str(name1) + " owes altogether!")

		print("======================================================================================")

	if Details1 == 4:

		logs1 = (name1 + " Has payed off this weeks bank deposit! EXIT ", time.asctime())

		f.write(str(logs1))

		f.close()

	elif stone == 0 and Details1 == 3:

	#everything except stone; (wood,ore,gold)

		logs2 = (name1 + " Has payed off everything except " + str(resultstone1) + "stone! EXIT", time.asctime())

		f.write(str(logs2))

		f.close()

	elif wood == 0 and Details1 == 3:

	#everything except wood; (stone,ore,gold)

		logs3 = (name1 + " Has payed off everything except " + str(resultwood1) + "wood! EXIT", time.asctime())

		f.write(str(logs3))

		f.close()

	elif ore == 0 and Details1 == 3:

	#everything except ore; (stone,wood,gold)

		logs4 = (name1 + " Has payed off everything except " + str(resultore1) + "ore! EXIT", time.asctime())

		f.write(str(logs4))

		f.close()

	elif gold == 0 and Details1 == 3:

	#everything except gold; (stone,wood,ore)

		logs5 = (name1 + " Has payed off everything except " + str(resultgold1) + "gold! EXIT", time.asctime())

		f.write(str(logs5))

		f.close()

	elif stone == 0 and wood == 0 and Details1 == 2:

	#everything except stone and wood; (ore,gold)

		logs6 = (name1 + " Has payed off everything except " + str(resultstone1) + "stone and " + str(resultwood1) + "wood! EXIT", time.asctime())

		f.write(str(logs6))

		f.close()

	elif stone == 0 and ore == 0 and Details1 == 2:

	#everything except stone and ore; (wood,gold)

		logs7 = (name1 + " Has payed off everything except " + str(resultstone1) + "stone and " + str(resultore1) + "ore! EXIT", time.asctime())

		f.write(str(logs7))

		f.close()

	elif stone == 0 and gold == 0 and Details1 == 2:

	#everything except stone and gold; (wood,ore)

		logs8 = (name1 + " Has payed off everything except " + str(resultstone1) + "stone and " + str(resultgold1) + "gold! EXIT", time.asctime())

		f.write(str(logs8))

		f.close()

	elif wood == 0 and ore == 0 and Details1 == 2:

	#everything except wood and ore; (stone,gold)

		logs9 = (name1 + " Has payed off everything except " + str(resultwood1) + "wood and " + str(resultore1) + "ore! EXIT", time.asctime())

		f.write(str(logs9))

		f.close()

	elif wood == 0 and gold == 0 and Details1 == 2:

	#everything except wood and gold; (stone,ore)

		logs10 = (name1 + " Has payed off everything except " + str(resultwood1) + "wood and " + str(resultgold1) + "gold! EXIT", time.asctime())

		f.write(str(logs10))

		f.close()

	elif ore == 0 and gold == 0 and Details1 == 2:

	#everything except ore and gold; (stone,wood)

		logs11 = (name1 + " Has payed off everything except " + str(resultore1) + "ore and " + str(resultgold1) + "gold! EXIT", time.asctime())

		f.write(str(logs11))

		f.close()

	elif wood == 0 and ore == 0 and gold == 0 and Details1 == 1:

	#everything except wood, ore and gold; (stone)

		logs12 = (name1 + " Has payed off everything except " + str(resultwood1) + "wood, " + str(resultore1) + "ore and " + str(resultgold1) + "gold! EXIT", time.asctime())

		f.write(str(logs12))

		f.close()

	elif ore == 0 and stone == 0 and gold == 0 and Details1 == 1:

	#everything except ore, stone and gold; (wood)

		logs13 = (name1 + " Has payed off everything except " + str(resultore1) + "ore, " + str(resultstone1) + "stone and " + str(resultgold1) + "gold! EXIT", time.asctime())

		f.write(str(logs13))

		f.close()

	elif stone == 0 and wood == 0 and gold == 0 and Details1 == 1:

	#everything except stone, wood and gold; (ore)

		logs14 = (name1 + " Has payed off everything except " + str(resultstone1) + "stone, " + str(resultwood1) + "wood and " + str(resultgold1) + "gold! EXIT", time.asctime())

		f.write(str(logs14))

		f.close()

	elif stone == 0 and wood == 0 and ore == 0 and Details1 == 1:

	#everything except stone, wood and ore; (gold)

		logs15 = (name1 + " Has payed off everything except " + str(resultstone1) + "stone, " + str(resultwood1) + "wood and " + str(resultore1) + "ore! EXIT", time.asctime())

		f.write(str(logs15))

		f.close()
	
RBN_BANK()
