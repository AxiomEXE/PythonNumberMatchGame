# PythonNumberMatchGame
Number Matching Game Using Python

```
#!/usr/bin/python3

import random, time

digits = input('How many numbers do you want to guess? ')
digits = int(digits)

sequence = []

for i in range(0, digits):
	sequence.append(random.randint(0,9))
print(sequence)

time.sleep(5)
for i in range (0, 50):
	print('')

for i in range(0, digits):
	print('Enter number here: ' +str(i))
	num = int(input())
	if num == sequence[i]:
		print('Correct')
	else: 
		print('WRONG!')
		break

print(sequence)	

```
