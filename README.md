
inputStr = input()
value="abcdefgh"
a=0
for i in range(1,9):
   for j in value:
      if (inputStr[0]=="a" or inputStr[0]=="h") and (inputStr[1]=="1" or inputStr[1]=="8"):
         a=1
      elif (inputStr[0]=="a" or inputStr[0]=="h") and (inputStr[1]==str(i+1)):
         a=2
      elif (inputStr[0]==j) and (inputStr[1]=="1" or inputStr[1]=="8"):
         a=4
      elif (inputStr[0]==value[i-1]) and (int(inputStr[1])==i+1):
         a=3
if a==1:
   print("Corner")
elif a==2 or a==4:
   print("Border")
else:
   print("Inside")
