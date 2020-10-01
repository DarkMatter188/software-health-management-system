# A simple Health Management system
#Keeps track of food and exercises performed by you
#  Exersise 5
def getdate():
    import datetime
    return datetime.datetime.now()
var=str(getdate())
print("1: Harry",
      "2: Rohan",
      "3: Hammond")
print("Enter the name of person by entering above choice number:",end=" ")
x1=int(input())
if x1==1:
    print("Enter 1 to get Diet or 2 to get Exersise for Harry:",end=" ")
    x2=int(input())
    if x2==1:
        f1=open("Harry_Diet.txt","r+")
        print("Press 1 for locking or 2 for retrieving for Diet:",end=" ")
        y1=int(input())
        if y1==1:
            print("Enter the food you ate ",end=" ")
            x3=input()
            f1.write(var)
            f1.write(" :")
            f1.write(x3)
        if y1==2:
            print(f1.read())
    if x2==2:
        f2=open("Harry_Exersise.txt","r+")
        print("Enter 1 to lock or 2 to retrieve Exercise:",end=" ")
        a1=int(input())
        if a1==1:
            print("Write the exercise performed by you:",end=" ")
            a2=input()
            f2.write("var :")
            f1.write(a2)
        if a1==2:
            print(f2.read())

# print("Enter the name of person by entering above choice number:",end=" ")
# l1=int(input())
elif x1==2:
    print("Enter 1 to get Diet or 2 to get Exersise for Rohan:",end=" ")
    l2=int(input())
    if l2==1:
        f2=open("Rohan_Diet.txt","r+")
        print("Press 1 for locking or 2 for retrieving for Diet:",end=" ")
        l1=int(input())
        if l1==1:
            print("Enter the food you ate ",end=" ")
            l3=input()
            f2.write(var)
            f2.write(" :")
            f2.write(l3)
        if l1==2:
            print(f2.read())
    if l2==2:
        f3=open("Rohan_Exersise.txt","r+")
        print("Enter 1 to lock or 2 to retrieve Exercise:",end=" ")
        v1=int(input())
        if v1==1:
            print("Write the exercise performed by you:",end=" ")
            v2=input()
            f3.write(var)
            f3.write("\n")
            f3.write(v2)
        if v1==2:
            print(f3.read())


elif x1==3:
    print("Enter 1 to get Diet or 2 to get Exersise for Hammad:",end=" ")
    l2=int(input())
    if l2==1:
        f4=open("Hammad_Diet.txt","r+")
        print("Press 1 for locking or 2 for retrieving for Diet:",end=" ")
        l1=int(input())
        if l1==1:
            print("Enter the food you ate ",end=" ")
            l3=input()
            f4.write(var)
            f4.write(" :")
            f4.write(l3)
        if l1==2:
            print(f2.read())
    if l2==2:
        f5=open("Hammad_Exersise.txt","r+")
        print("Enter 1 to lock or 2 to retrieve Exercise:",end=" ")
        v1=int(input())
        if v1==1:
            print("Write the exercise performed by you:",end=" ")
            v2=input()
            f5.write(var)
            f5.write("\n")
            f5.write(v2)
        if v1==2:
            print(f5.read())
