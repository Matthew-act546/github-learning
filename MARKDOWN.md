# THIS IS A H1 IN HTML HEADER
## THIS IS A H2
### THIS IS H3 
#### THIS IS H4 
##### THIS IS H5
###### THIS IS H6
I'm a paragraph
<br>
<br>
**I'm Bold text**
<br>
*I'm italic text*
<br>
~~I'm strike through text~~
<br>
**I'm *mixed text* ~~etc etc~~**

**Creating an ordered list**
1. [HTML](https://en.wikipedia.org/wiki/HTML)
    1. HYPERTEXT MARKUP LANGUAGE
1. [CSS](https://en.wikipedia.org/wiki/CSS)
    1. CASCADING STYLESHEET
1. [JAVASCRIPT](https://en.wikipedia.org/wiki/JavaScript)


**Creating unordered list**
- [Adding Inline codeblock](#adding-inline-codeblock)
- [Adding Multi-line codeblock](#adding-multi-line-codeblock)
- [Text citation](#text-citation)



---

## Adding Inline codeblock

Ternary Operator if statement: `var age = (age > 17) ? ("Congrats now you're not a minor") : ("you are a minor")`

## Adding Multi-line codeblock
This guessing game code unfinished: 
``` py
import random

#asking the user...
"""print("\nGuessing Game!\ntype guessing game to play")"""
gets = str(input())

line = "\n________________________\n"

def error():
	line = "\n___________________________________________\n"
	print( line + "Error\nCheck if there's a problem to your input" + line)

#conditional statement
if gets == "1" or gets == "Guessing Game":
	print("Choose a guessing level game\nby number example 2(Normal)")
	print("1. Easy")
	print("2. Normal")
	print("3. Hard")
	print("4. Customize")
	print("5. Adventure")
	print("6. help")
	choosing = int(input("->"))

	if type(choosing) == str:
		print(line + "Error " +line)
	elif choosing == 1:
		up_to = 5
		rand_num = str(random.randint(1, up_to))
		print("Welcome to the easy level where you\ngoing to guess is up to 5 Game!")
		print(rand_num)
		guess_easy = str(input("\nWhat is your guess number?\n->"))
		int_guess_easy = int(guess_easy)
		if guess_easy == rand_num:
			print("Congratulations!!!\nYou're right!")
		elif int_guess_easy >= 6:
			print(line + "sorry this easy level is just up to 5This number '" + guess_easy +"' \nbig number for easy level" + line)
		elif int_guess_easy <= 0:
			print(line + "This number '" + guess_easy+ "' not acceptable" + line)
		elif guess_easy != rand_num:
			print(line + "YOU ARE WRONG!\nThe Answer is '"+ str(rand_num) + "'\nbetter luck next time" + line)
		else:
			error()
	
	elif choosing == 2:
		print("Welcome to normal level where you\ngoing to guess is up to 15")
		up_to = 15 
		rand_num = str(random.randint(1, up_to))
		print(rand_num)
		print("\nWhat is your guess number?")
		guess_normal = input("->")
		int_guess_normal = int(guess_normal)
		if guess_normal == rand_num:
			print("CONGRATULATIONS YOU WIN!")
		elif int_guess_normal <= 0:
			print(line + "This number '" + guess_normal+ "' not acceptable" + line)
		elif guess_normal != rand_num:
			print(line + "YOU ARE WRONG!\nThe Answer is '"+ str(rand_num) + "'\nbetter luck next time" + line)
		else:
			error()
	
	

	elif choosing == 3:
		print("wow")

else:
	error()
```

---
## Text citation
> Don’t say it can not be done, rather say,
you don’t know how to do it yet.
>>Do not pursue money. He who pursues money will never achieve it. Serve! If you serve as best as you can, you will not be able to escape money.
>
> <cite>–- Tomas Bata</cite> 

[![ERROOR](./pic.jpg)](https://www.merriam-webster.com/dictionary/handsome) 


| First Name | Last Name | close or not |
| :------ | :------ | :------| 
| Dave | Oribiada | Close |
| jonric | reyna | close |
| angelica | credo | close |

<details>
<summary>What is in Header?</summary>
Header is the top of the code in web development or html file.

The following attributes in Header is: 
- title
- meta
- viewport
- style or stylesheets
</details>
