# python basic codes:-
==========================

# a program to find perfect number<pre>
temp=0  
num=int(input("enter the number  : "))  
for i in range(1,num//2+1):  
    if(num%i==0):  
        temp=i+temp  
if(temp==num):  
    print("the number is perfect ")  
else:  
    print("not perfect")</pre>



# armstrong number  :-<pre>
size=0  
num=int(input("enter the number  : "))  
data=user=num  
while(num!=0):  
    num=num//10  
    size=size+1  
print("size is ", size)  
///num=0
temp=0  
for i in range(1,size+1):  
    temp=data%10  
    num=num+temp**size  
    data=data//10  
if(num==user):  
    print("armstrong number")  
else:  
    print("not armstrong")  </pre>
    
# reverse string without change in words:-<pre>
a=input("enter the string to reverse : ")  
data=a.split()  
new = data[ : : -1]  
result=" ".join(new)  
print(result)  </pre>

# program to count vowel and consonents in string<pre>
a=input("enter the string : ")  
vow=0  
con=0  
sp=0  
data=a.lower()  
for i in data:  
    if(i=='a' or i=='e' or i=='i' or i=='o' or i=='u'):  
        vow=vow+1  
    elif(i==" "):  
        sp=sp+1  
    else:  
        con=con+1  
print("the num of vowel is ", vow)  
print("the num of cons is ", con)  
print("the num of space is ", sp)</pre>

# python list comprehension<pre>

if __name__ == '__main__':  
    student = []  
    for _ in range(int(input("Enter number of students: "))):  
        name = input("Enter name: ")  
        score = float(input("Enter score: "))  
        student.append([name, score])  
    value = sorted(set([score for name, score in student]))  
    second_lowest = value[1]  
    names = sorted([name for name, score in student if score == second_lowest])  
    for name in names:  
        print(name)
</pre>



