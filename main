""" List Comprehension: Odd numbers """
#Use anonymous filter function to find odd numbers in range of 10 (0-9) and print them
if __name__ == "__main__":
	print('Odds 0-9:', [i for i in range(10) if i % 2])


""" List Comprehension: All Possible Combinations  """
#Print all possible combinations from two lists where i + j + k != n
if __name__ == "__main__":
	x = int(input())
	y = int(input())
	z = int(input())
	n = int(input())

	print([[i,j,k] for i in range (x + 1) for j in range(y + 1)
	for k in range(z + 1) if i + j + k != n])


""" Arrays: Runner-up score """
#Find and print the runner-up score
if __name__ == '__main__':
    n = [2,3,6,6,5]

	m = max(n)
    b = ([x for x in n if x != m])
    print(max(b))

    #A = []
    #for i in n:
    #    A.append(i)
    #A.sort()

	#m = max(A)
    #B = ([x for x in A if x != m])
    #print(max(B))


""" Arrays: Lowest value """
#Find the lowest int in an array. Same as min()
if __name__ == '__main__':
    values = [5, 7, 2, 8, 9, 1]
    lowest = values[0]

    for i in range(len(values)):
        if (values[i] < lowest):
            lowest = values[i]

    print("The lowest value is: ", lowest)


""" Array: Highest Value """
#Find the highest int in an array. Same as max()
if __name__ == '__main__':
    values = [5, 7, 2, 8, 9, 1]
    highest = values[0]

    for i in range(len(values)):
        if (values[i] > highest):
            highest = values[i]

    print("The highest value is: ", highest)


""" Nested Lists: Second lowest score """
#Get second lowest scores in nested list
if __name__ == '__main__':
    nameScoreList = []
    name = ["Harry", "Barry", "Tina", "Bob", "x"]
    score = [80, 60, 70.2, 70.1, 70.1]
    nameScoreList2 = []
    secondHighest = []

    #Get user inputs
    for _ in range(len(name)):

        #Make a nested list with names and scores
        nameScoreList = [i for i in zip(name,score)]

    nameScoreList.sort()
    #Get the min score
    getScores = ([i[1] for i in nameScoreList])
    mn = min(getScores)

    #Make new list excluding the lowest score
    nameScoreList2 = ([x for x in nameScoreList if x[1] != mn])

    #Get the min score
    getScores2 = ([i[1] for i in nameScoreList2])
    newmn = min(getScores2)

    #Make a new list excluding items without lowest score
    nameScoreList3 = ([i for i in nameScoreList2 if i[1] == newmn])

    nameScoreList3.sort()
    #Get the names from the list
    namesOrdered = ([i[0] for i in nameScoreList3])
    for n in namesOrdered:
        print(n)


""" Recursion: Factorial function """
#Recursive factorial function
def factorial(n):
	"""
	Input: Int n
	Output: factorial n * n - 1
	"""

	if n ==1:
		return 1
	else:
		return n * factorial(n -1)
	print(factorial(4))


""" Dictionaries: Average scores """
#In a dictionary of students and their scores, print the average
#of a chosen student's scores correct to two decimal places
if __name__ == '__main__':
    n = int(input())
    student_marks = {}
    #nameScore = {}
    for _ in range(n):
        name, *line = input().split()
        scores = list(map(float, line))
        student_marks[name] = scores
    query_name = input()

    sums = 0
    for j in student_marks[query_name]:
        sums += j
    avgs = sums / len(scores)
    print("%.2f" % avgs)


""" Sets: Differences  """
#From user input, get two sets of numbers. Find the difference, then
#print the number of entries that are the same between the two sets.
if __name__ == "__main__":
    n1 = int(input())
    set1 = set(map(int, input().split()))
    n2 = int(input())
    set2 = set(map(int, input().split()))

    diff = set([])
    diff = set1.difference(set2)
    print(len(diff))


""" Sets: Symmetric Differences """
#From user input, get two sets of numbers. Find the symmetric difference, then
#print the number of entries that are different between the two sets.
if __name__ == '__main__':
    n1 = int(input())
    set1 = set(map(int, input().split()))
    n2 = int(input())
    set2 = set(map(int, input().split()))

    diff = set([])
    diff = set1.symmetric_difference(set2)
    print(len(diff))


""" Regex: UID """
#Validate UID to include at least 10 uppercase letters, lowercase letters,
#or digits. It also must have at least 3 digits and 2 uppercase letters.
#Finally, no two characters can repeat.

# Enter your code here. Read input from STDIN. Print output to STDOUT
import re

def main():
    t = int(input())
    for _ in range(t):
        uid = input()
        checkUID(uid)

def checkUID(uid):
    if re.search(r'^[A-Za-z0-9]{10}$', uid) and \
    re.search(r'([0-9].*){3}', uid) and \
    re.search(r'([A-Z].*){2}', uid) and \
    not re.search(r'(.).*\1', uid):
        print('Valid')
    else:
        print('Invalid')

main()


""" Lists: List functions """
#Take a command and some params and perform the designated actions on a list l
#Input int N, a number of params to enter
if __name__ == '__main__':
    #Declare and init variables
    N = int(input())
    l = list()
    params = list()

    #For the number of params N, split on space, take params[0] as command
    #and perform the designated action with params that are not cmd
    for _ in range(N):
        params = input().split(" ")
        cmd = params[0]

        if cmd == ("insert"):
            l.insert(int(params[1]), int(params[2]))
        elif cmd == ("remove"):
            l.remove(int(params[1]))
        elif cmd == ("append"):
            l.append(int(params[1]))
        elif cmd == ("pop"):
           l.pop()
        elif cmd == ("sort"):
            l.sort()
        elif cmd ==("reverse"):
            l.reverse()
        elif cmd == ("print"):
            print(l)


""" Tuples: Hash the Tuple """
#Given n number of int inputs, add them to a tuple t, then print the hash of that tuple.
if __name__ == '__main__':
	#Declare and init variables
	n = int(input())
	integer_list = map(int, input().split())
	t = ()

	#For the length of n, concatenate the value of integer_list to tuple t
	for i in range(n):
		t += tuple(integer_list)

	#Print the hash of the tuple t
	print(hash(t))


""" Strings: Find overlapping substring """
#Find all overlapping occurences of a sub string
def count_substring(string, sub_string):
    counter = 0
    start = 0

    while True:
        #Search string left to right
        #start = location where the match starts. Range = (1, len(string))
        start = string.find(sub_string, start) + 1
        if start > 0:
            #If start location of match is > 0 (anywhere in string), increment counter
            counter += 1
        else:
            #When start = 0 (no more matches), return counter total
            return counter

if __name__ == '__main__':
    string = input().strip()
    sub_string = input().strip()

    count = count_substring(string, sub_string)
    print(count)


""" Regex and Strings: Find formatting types """
#Check if alphanumeric, alpha, digit, lowercase, and uppercase characters exist
#in a string. For each, if True, print "True". If False, print "False".
import re

if __name__ == '__main__':
    s = input()

    #Check for alphanumeric characters
    if re.search(r'[a-zA-Z0-9]', s):
        print("True")
    else:
        print("False")

    #Check for alpha characters
    if re.search(r'[a-zA-Z]', s):
        print("True")
    else:
        print("False")

    #Check for digits
    if re.search(r'[0-9]', s):
        print("True")
    else:
        print("False")

    #Check for lowercase letters
    if re.search(r'[a-z]', s):
        print("True")
    else:
        print("False")

    #Check for uppercase letters
    if re.search(r'[A-Z]', s):
        print("True")
    else:
        print("False")


""" Strings: Wrap text """
#Wrap a string of text at a given number of characters (max_width) and print
#each on a new line
import textwrap

def wrap(string, max_width):
    result = textwrap.fill(string, max_width)
    return result

if __name__ == '__main__':
    string, max_width = input(), int(input())
    result = wrap(string, max_width)
    print(result)


""" Sets: Find the average of a set """
#Use sum() and len() to average the values of a set and return the average
def average(array):
    array = set(array)
    s = 0
    l = len(array)
    s = sum(array)
    avg = s / l
    return avg

if __name__ == '__main__':
    n = int(input())
    arr = list(map(int, input().split()))
    result = average(arr)
    print(result)


""" Sets: Symmetric Difference """
#Find the symmetric difference between two sets of numbers and print them each
#on a new line
if __name__ == "__main__":
    n1 = int(input())
    set1 = set(map(int, input().split()))

    n2 = int(input())
    set2 = set(map(int, input().split()))

    sdiff = set([])
    sdiff = set1.symmetric_difference(set2)
    sdiff = sorted(sdiff)

    for i in sdiff:
        print(i)


""" Sets: Find values from array in disjointed sets """
#Find values in an array in either setA or setB. If the value is in setA,
#add a point to the happiness score. If the value is in setB, subtract a point
#from the happiness score. Otherwise, add zero points. Print the total
#happiness at the end.
if __name__ == "__main__":

    n = list(map(int, input().split()))
    vals = list(map(int, input().split()))
    setA = set(map(int, input().split()))
    setB = set(map(int, input().split()))
    happiness = 0

    for i in range(len(vals)):
        if vals[i] in setA:
            happiness += 1
        elif vals[i] in setB:
            happiness -= 1
        else:
            happiness += 0

    print(happiness)


""" Sets: Add items and count unique entries """
#Add number of items according to n, then count the number of unique entries
#Set already strips duplicates, so printing the len of set s prints the number
#of unique values
if __name__ == "__main__":

    n = int(input())
    s = set([])

    for i in range(n):
        s.add(input())

    print(len(set(s)))


""" Sets: Modify sets with methods """
#Allow user to input n, the length of a set && s, the set values && sn, the number
#of commands they will enter. Perform operations on the set given a number of
#commands. After the commands are performed, sum the remaining values in s.
if __name__ == "__main__":
	n = int(input())
	s = set(map(int, input().split()))
	sn = int(input())
	params = list()

	for _ in range(sn):
		params = input().split(" ")
		cmd = params[0]

		if cmd == ("remove"):
			s.remove(int(params[1]))
		elif cmd == ("pop"):
			s.pop()
		elif cmd == ("discard"):
			s.discard(int(params[1]))

	print(sum(s))

""" Recursion """
#Find the product of two numbers recursively
# a * b = a + (a * (b - 1))
def mult_rec(a, b): # @param 5,4
    """
    Input: a, b, positive ints
    Return: product of a, b
    """
    if b == 1:
        return a
    else:
        return a + mult_rec(a, b - 1)

print (mult_rec(5, 4))
print ()

#Standard Factorial
# n! = n(n -1) * n(n - 2) * n(n - 3) ... * 1
def factorial(n): # @param 4
    """
    Input: n, a positive int
    Return: factorial n * (n - 1)
    """
    if n == 1:
        return 1
    else:
        return n * factorial(n - 1) # @return 4 * 3 * 2 * 1 = 24

print (factorial(4)) # print (24)
print ()

#Recursive Towers of Hanoi
def printMove(fr, to):
    """
    Input: fr and to, positive ints
    Print: fr and to in a message to keep track of moves
    """
    print(('move from ' + str(fr) + ' to ' + str(to)))

def towers(size, fr, to, spare):
    """
    Input: size, fr, to, spare, all positive ints
    Return: None
    """
    if size == 1:
        printMove(fr, to)
    else:
        towers(size - 1, fr, spare, to)
        towers(1, fr, to, spare)
        towers(size - 1, spare, to, fr)

print (towers(4, 3, 1, 2))
print ()

#Standard Fibonacci
#Fibonacci number: Each number is the sum of the two previous numbers
#Starts at 0 + 1. Count starts at first sum, counting starts at 0, so fib(10) = 89
def fib(x):
    """
    Input: x, an int >= 0
    Return: Fibonacci of x
    """
    if x == 0 or x == 1:
        return 1
    else:
        return fib(x - 1) + fib(x - 2)

print (fib(6))
print ()

#Efficient Fibonacci using dict with recursion
#Fibonacci number: Each number is the sum of the two previous numbers
#Starts at 0 + 1. Count starts at first sum, counting starts at 0, so fib(10) = 89
def fib_efficient(n, fibDict):
    """
    Input: n, a positive int. fibDict, a dictionary
    Return: Fibonacci of n
    """
    if n in fibDict:
        return fibDict[n]
    else:
        ans = fib_efficient(n - 1, fibDict) + fib_efficient(n - 2, fibDict)
        fibDict[n] = ans
        return ans

fibDict = {1:1, 2:2}
print(fib_efficient(8, fibDict))


""" Sets: Union """
#Find the number of students in two sets that have at least one subscription to
#a newspaper.
if __name__ == "__main__":
    n1 = int(input())
    set1 = set(map(int, input().split()))
    n2 = int(input())
    set2 = set(map(int, input().split()))

    u = set([])
    u = set1.union(set2)
    print(len(u))

""" Sets: Intersection """
#Find the number of students in two sets who have subscriptions to
#both newspapers.
if __name__ == "__main__":
    n1 = int(input())
    set1 = set(map(int, input().split()))
    n2 = int(input())
    set2 = set(map(int, input().split()))

    i = set([])
    i = set1.intersection(set2)
    print(len(i))


""" Sets: Update with set commands """
#Take user input to determine n, the number of items in a set; s, the values
#in the set; nCmd, the number of commands to be entered; cmd, the command; i, the
#length of the command inputs; and s2, the second set of numbers to update,
#intersect, or difference with set 1.
if __name__ == "__main__":
	n = int(input())
	s = set(map(int, input().split()))
	nCmd = int(input())

	for i in range(nCmd):
		cmd, i = input().split()
		s2 = set(map(int, input().split()))

		if cmd == ("update"):
			s.update(s2)
		elif cmd == ("intersection_update"):
			s.intersection_update(s2)
		elif cmd == ("difference_update"):
			s.difference_update(s2)
		elif cmd == ("symmetric_difference_update"):
			s.symmetric_difference_update(s2)

	print(sum(s))

""" Sets: Find a unique value that does not repeat """
#This looks like an elegant solution, but doubles quadratic complexity and
#therefore doesn't work well on large datasets. This solution must iterate
#over the entire list multiple times.
if __name__ == "__main__":
    k = int(input())
    l = list(map(int, input().split()))

    c = [x for x in l if l.count(x) != k]

    print(c.pop())

#The better solution: take the list as input, put all unique values in a set, put
#all duplicates in a set, then take the difference of the two sets to find the
#unrepeated element between them. Pop print to avoid another for loop for printing.
if __name__ == "__main__":
    k = 5
    l = list(map(int, input().split()))
    allItems = set()
    duplicates = set()

    for i in l:
        if i not in allItems:
            allItems.add(i)
        else:
            duplicates.add(i)

    print(allItems.difference(duplicates).pop())



""" Sets: Subset True or False """
#Take t sets of input and determine for each set a and set b if set a is a
#subset of b
if __name__ == "__main__":
    t = int(input())

    for _ in range(t):
        na = int(input())
        a = set(map(int, input().split()))
        nb = int (input())
        b = set(map(int, input().split()))

        if a.issubset(b):
            print("True")
        else:
            print("False")


""" Sets: Strict Supersets """
#Find out if a is a superset of n sets of b
if __name__ == "__main__":
    a = set(map(int, input().split()))
    n = int(input())
    s = [] #Make an array to hold all the set comparisons like a database

    for _ in range(n):
        b = set(map(int, input().split()))

        if a.issuperset(b):
            s.append("True")
        else:
            s.append("False")

	#If "False" does not appear in s, a is a strict superset of n sets of b
    if "False" not in s:
        print("True")
    #Otherwise, at least one entry in s is "False" and a is not a strict superset
	#of all n sets of b
	else:
        print("False")




"""  Itertools: Cartesian Products """
#Find and print the Cartesian products of two lists
from itertools import product

if __name__ == "__main__":
    a = list(map(int, input().split()))
    b = list(map(int, input().split()))
    p = list(product(a, b))

    print(" " .join(map(str, p)))




""" Strings: ASCII Art Patterns """
#Print a HackerRank logo with thickness based on user input (int)

thickness = int(input()) #This must be an odd number
c = 'H'

#Top Cone
for i in range(thickness):
    print((c*i).rjust(thickness-1)+c+(c*i).ljust(thickness-1))

#Top Pillars
for i in range(thickness+1):
    print((c*thickness).center(thickness*2)+(c*thickness).center(thickness*6))

#Middle Belt
for i in range((thickness+1)//2):
    print((c*thickness*5).center(thickness*6))

#Bottom Pillars
for i in range(thickness+1):
    print((c*thickness).center(thickness*2)+(c*thickness).center(thickness*6))

#Bottom Cone
for i in range(thickness):
    print(((c*(thickness-i-1)).rjust(thickness)+c+(c*(thickness-i-1)).ljust(thickness)).rjust(thickness*6))


#Print a ridiculous welcome doormat
n, m = map(int, input().split())

for i in range(n // 2):
    pattern = (".|." * ((2 * i) + 1)).center(m, "-")
    print("".join(pattern))

print ("WELCOME".center(m, '-'))

for i in range(n // 2):
    reversepattern = (".|." * ((2 * (n // 2 - i - 1)) + 1)).center(m, "-")
    print("".join(reversepattern))

#With a list comprehension
n, m = map(int, input().split())
pattern = [(".|." * (2 * i + 1)).center(m, "-") for i in range(n//2)]
print("\n".join(pattern + ["WELCOME".center(m, '-')] + pattern[::-1]))


""" Strings: Formatting """
#For int n entered by user, print the decimal, octal, hex, and binary values of
#each number with each column the length of n as a binary. Right align all vals.
def print_formatted(number):
    counter = 1
    for i in range(n):
        count = counter
        length = len("{0:b}".format(n))
        decimal = f"{count:d}"
        octal = f"{count:o}"
        hexadecimal = f"{count:X}"
        binary = f"{count:b}"
        print(f"{decimal:{length}} {octal:{length}} {hexadecimal:{length}} {binary:{length}}")
        counter += 1

if __name__ == '__main__':
    n = int(input())
    print_formatted(n)

""" Strings: ASCII Art """
#Print a ridiculous alphabet rangoli
import string

def print_rangoli(size):
    alpha = string.ascii_lowercase
    pattern = []

    for i in range(size):
        s = '-'.join(alpha[i:size])
        pattern.append((s[::-1] + s[1:]).center(4 * size - 3, "-"))
    print("\n".join(pattern[:0:-1] + pattern))

if __name__ == '__main__':
    n = int(input())
    print_rangoli(n)

""" Strings: Capitalize Function """
#Capitalize the first letter in each word
name = "jane  roberts"

nameCapped = " ".join(i.capitalize() for i in name.split(" "))
print(nameCapped)


""" Strings: Minion Game """
#Mine (not efficient enough apparently)
def minion_game(s):
    vowels = "AEIOU"
    kevin = []
    stuart = []

    for i, j in enumerate(s):
        if j in vowels:
            for k in range(len(s[i:])):
                kevin.append(s[i:i + k + 1])
        else:
            for k in range(len(s[i:])):
                stuart.append(s[i:i + k + 1])

    kevinPoints = getPoints(s, kevin)
    stuartPoints = getPoints(s, stuart)

    if kevinPoints > stuartPoints:
        print("Kevin", kevinPoints)
    elif stuartPoints > kevinPoints:
        print("Stuart", stuartPoints)
    else:
        print("Draw")

def getPoints(s, substring):
    points = [pnt for pnt in substring if pnt in s]
    return len(points)

if __name__ == '__main__':
    #Get user input s, a string
    s = input().strip()
    minion_game(s)



#Efficient solution
def minion_game(s):
	vowels = "AEIOU"
	kevinPoints = 0
	stuartPoints = 0

	for i in range(len(s)):
		if s[i] in vowels:
			kevinPoints += (len(s) - i)
		else:
			stuartPoints += (len(s) - i)

	if kevinPoints > stuartPoints:
		print("Kevin", kevinPoints)
	elif stuartPoints > kevinPoints:
		print("Stuart", stuartPoints)
	else:
		print("Draw")

if __name__ == '__main__':
    #Get user input s, a string
    s = input().strip()
    minion_game(s)

""" Strings: String Groups """
#Split a given string into k groups. Remove duplicates and print groups.
if __name__ == '__main__':
    k = 3
    string = "AABCAAADA"

    #My version
    items = [set(string[i:i+k]) for i in range(0, len(string), k)]
    for i in items:
        print("".join(i))

    #Pass version
    for i in range(0, len(string), k):
        s = ""
        for j in string[i:i+k]:
            if j not in s:
                s += j
        print(s)

""" collections.Counter: Selling shoes """
#Get
#x, a number of shoe sizes
#shoeSizes, a Counter object
#n, the number of attempted purchases
#size, price: User inputs desired shoe size and price
#If the shoe exists, add the price to income. Otherwise, the purchase doesn't
#take place.
from collections import Counter

if __name__ == "__main__":
    #Declare variables
    x = int(input())
    shoeSizes = Counter(map(int, input().split()))
    n = int(input())
    income = 0

    #For each n, take size and price input.
    #If size exists in shoeSizes, remove it and increment income with the price
    for i in range(n):
        size, price = map(int, input().split())
        if shoeSizes[size]:
            shoeSizes[size] -= 1
            income += price

    print(income)

""" Itertools: Permutations """
#Given a string s and int k, print all sorted permutations of s with len k
#Note: s must be sorted before putting perms in a list and using permutations
#and k must be cast as an integer
from itertools import permutations

if __name__ == "__main__":
    s, k = input().split()
    perms = list(permutations(sorted(s), int(k)))

    for i in perms:
        print("".join(i))

""" Itertools: Combinations """
#Given a string s and int k, print all sorted combinations of s inclusive with len k
from itertools import combinations

if __name__ == "__main__":
    s, k = input().split()
    s = sorted(s)
    k = int(k)

    for i in range(1, k+1):
        for j in combinations(s, i):
            print("".join(j))

""" Itertools: Combinations with replacement """
#Given a string s and int k, print all sorted replacement combinations of s with len k
from itertools import combinations_with_replacement

if __name__ == "__main__":
    s, k = input().split()
    perms = list(combinations_with_replacement(sorted(s), int(k)))

    for i in perms:
        print("".join(i))

""" Itertools: Groupby """
#Given a string s, print an item from list of s and count of consecutive appearances
from itertools import groupby

if __name__ == "__main__":
    s = input()
    groups = []

    for key, group in groupby(list(s)):
        g = ("({}, {})".format(len(list(group)), key))
        groups.append(str(g))
    print(" ".join(groups))

    """
	More Pythonic solution
    groups = groupby(s)
    print([(key, sum(1 for i in group)) for key, group in groups])
    """

""" DefaultDict """
#Enter n, the len for group a and m, the len for group b. For every word from
#group b that appears in group a, print the location in the dict. Otherwise, if
#the word in a does not exist in group b, print -1.

from collections import defaultdict

if __name__ == "__main__":
	n, m = map(int, input().split())
	a = defaultdict(list)
	b = []

	for i in range(0, n):
		a[input()].append(i + 1)

	for k in range(0, m):
		b.append(input())

	for x in b:
		if x in a:
			print(' '.join(map(str, a[x])))
		else:
			print(-1)

""" Namedtuple """
#Get n columns of data from user input and map it to a namedtuple.
#Find and print the average of the total students' marks (total/n).
from collections import namedtuple

if __name__ == "__main__":
	n = int(input())
	cols = ",".join(input().split(' '))
	StudentMarks = namedtuple('StudentMarks', cols)
	total = 0

	for i in range(n):
		inp = input().strip().split()
		getMarks = StudentMarks(*inp)
		total += int(getMarks.MARKS)

	avgMarks = total/n
	print(f'{avgMarks:.2f}')

""" Calendar """
#Given a date from user input (MM DD YYYY), print the weekday of that date.
import calendar

if __name__ == "__main__":

	date_input = input()
	month, day, year = map(int, date_input.split(' '))
	weekday = calendar.weekday(year, month, day)
	dayname = calendar.day_name[weekday]

	print(dayname)
