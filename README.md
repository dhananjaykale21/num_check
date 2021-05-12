# num_check
# eat sleep rave  repeat
N="Eat sleep rave repeat"
def fun(N):
    count=0
    count1=0
    count2=0
    v="aeiou"
    
    for i in N:
        if(i.isspace()):
            count1=count1+1
    for i in N:
        if not (i.isalnum() or i.isspace()):
            count=count+1
    for i in v:
        if(i in N):
            count2=count2+1
    if not (N[0].isalnum() or N[-1].isalnum()):
        return "A"
    elif (N[3].isdigit()):
        return "B"
    elif (count==3):
        return "C"
    elif (count1==3):
        return "D"
    elif(count2==5):
        return "E"
    else:
        return "X"
print(fun(N))                                
-----------------------------------------
Q #wrtite python that accept input string from input_list,list2 
as parameter and return early stop based on the logic below
def num_check(input_list1,input_list2):
    output_list =[]
    for i in range(0,len(input_list1)):
        #first
        if input_list1[i] in input_list2:
            output_list.append(input_list1[i])
        #second condition
        elif input_list1[i]**2 in input_list2:
            output_list.append(input_list1[i])
        #third condition
        elif str(input_list1[i])[-1]==str(input_list2[i])[-1]:
            output_list.append(input_list1[i])
        #fourth condition
        else:
            num = str(input_list1[i])
            prod = 1
            for n in num:
                prod = prod *int(n)
            if prod in input_list2:
                output_list.append(input_list1[i])
    return output_list
print(num_check([26,17,25,35,39,63],[26,671,11,21,14,28]))




--------------------------

Q #wrtite python that accept input string from input_list,list2 
as parameter and return early stop based on the logic below
def num_check(input_list1,input_list2):
    output_list =[]
    for i in range(0,len(input_list1)):
        #first
        if input_list1[i] in input_list2:
            output_list.append(input_list1[i])
        #second condition
        elif input_list1[i]**2 in input_list2:
            output_list.append(input_list1[i])
        #third condition
        elif str(input_list1[i])[-1]==str(input_list2[i])[-1]:
            output_list.append(input_list1[i])
        #fourth condition
        else:
            num = str(input_list1[i])
            prod = 1
            for n in num:
                prod = prod *int(n)
            if prod in input_list2:
                output_list.append(input_list1[i])
    return output_list
print(num_check([26,17,25,35,39,63],[26,671,11,21,14,28]))



--------------------------------------------------
#password@#&*?


password="Itz_Me_h1ere@"
strength=10
v="aeiou"
alp="QWERTYUIOPLKJHGFDSAZXCVBNM"
count=0
count1=0
count2=0
count3=0
for i in password:
    for j in v:
        if(i==j):
            count+=1
for i in password:
    if(i in "@#&*?"):
        count1+=1
for i in password:
    for j in alp:
        if(i==j):
            count2+=1
for i in password:
    if(i.isdigit()):
        count3+=1
for i in password:
    
    if(i.isdigit()):
        count3+=1
if(count3>=1):
    strength+=3
if(count>=1):
    strength+=2
if(count1>=1):
    strength+=2
if(count2>=1):
    strength+=3
if(len(password)>6):
    strength+=2
else:
    strength-=1
if(strength==10):
    strength="not a good password"
print(strength)
    
--------------------------------------------------


a#given two list if l1==l2 then output a 
#elseprint "E"


L1=[12,23,45,67,89]
L2=[12,23,45,67,67]
output=""
count=0
count1=0
s=0
if(L1==L2):
    output="A"
for i in L1:a
    for j in L2:
        if(i==j):
            count1+=1
for i in L1:
    s+=i
    for j in L2:
        if(j==s):
            count+=1
if(count1==2):
    output="B"
for i in L1:
    for j in L2:
        if(i%10==j%10):
            output="C"
        
if(s in L2):
    output="D"
if(output==""):
    output="E"
print(output)
    
    
  --------------------------
  
  input_string="Aayusha123456"
out=""

name=input_string[-6:]
number=input_string[-6:]
su=0

if(name[0]==name[-1]):
    out+=str(len(name))
if(name[0]==name[1]):
    out+="a"
    
if(number[-2]==number[-1]):
    out+=number[-1]
if(out==""):
    out+="F"
for i in number:
    su+=int(i)
if(su%2==0):
    out+=str(su)
print(output)
--------------------------------------------


#given a string "i lov3e myself"

str="I lo6ve myself"
output=""
def fun(str):
    count=0
    count1=0
    count2=0
    a=str.split()
    b=a[1]
    
    for i in str:
        if not(i.isalnum() or i.isspace()):
            count+=1
    for i in b:
        if(i.isdigit()):
            count1+=1
    for i in str:
        if(i in ","):
            count2+=1
    if(count==3):
        return "A"
    elif (count1>=1):
        return "B"
    elif(len(str)>50):
        return "C"
    elif(count2>0):
        return "D"
    elif (str[0].islower()):
        return "E"
    else:
        return "-1"
print(fun(str))
        
 -----------------------------------------
 
 
 
            
    
    
    
