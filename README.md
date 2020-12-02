
pas = [line.rstrip('\n') for line in open("pass.txt")]
x = 0
 
for i in range(len(pas)):
    numbers = pas[i].split()[0].split("-") 
    char = pas[i].split()[1].strip(":") 
    passi = pas[i].split()[2] 
    minnum = int(numbers[0]) 
    maxnum = int(numbers[1]) 
    if passi.count(char) >= minnum and passi.count(char) <= maxnum:
      print(passi)
      x += 1
print("The are", x, "valid passwords")

---------------------------------------------------------- P1

pas = [line.rstrip('\n') for line in open("pass.txt")]
x = 0




for i in range(len(pas)):
    numbers = pas[i].split()[0].split("-") 
    char = pas[i].split()[1].strip(":") 
    passi = pas[i].split()[2] 
    firstnum = int(numbers[0])-1 
    secondnum = int(numbers[1])-1 
    if passi[firstnum] != passi[secondnum] and (passi[firstnum] == char or passi[secondnum] == char):
        x += 1
 
print("The are", x, "valid passwords")

-------------------------------------------------------- P2



