import csv
import sys

f = open("sample.csv")




x=0
m=0
u=0
z=0
b=0
k=0
x1=0
m1=0
u1=0
z1=0
b1=0
s=0



for row in csv.reader(f):
   if(row[1])=="IT" :
       x=x+1

   if(row[1])=="HR" :
      m=m+1

   if(row[1])=="FR" :
       u=u+1

   if(row[1])=="PR" :
       z=z+1

   if(row[1])=="L&R" :
       b=b+1

   if(row[1])=="ADV" :
       k=k+1



print "Total Applicants:"
print "\n"
print "IT:",x,
print "\n"

print "HR:",m,
print "\n"

print "FR:",u,
print "\n"

print "PR:",z,
print "\n"

print "L&R:",b,
print "\n"

print "ADV:",k,
print "\n"

f = open("sample.csv")
for row in csv.reader(f):
   if(row[2])=="2017" :
       x1=x1+1
       
   if(row[2])=="2018" :
      m1=m1+1

   if(row[2])=="2019" :
       u1=u1+1

   if(row[2])=="2020" :
       z1=z1+1

   if(row[2])=="2021" :
       b1=b1+1


print "\n"
print "2017:",x1,
print "\n"

print "2018:",m1,
print "\n"

print "2019:",u1,
print "\n"

print "2020:",z1,
print "\n"

print "2021:",b1,
print "\n"
print "\n"



y=raw_input("Please select a preference: ")
g=raw_input ("Please select a graduation year: ")


f = open("sample.csv")
for row in csv.reader(f):
   if(row[2])==g and (row[1])==y :
       s=s+1


print "Number of applicants:",s,

r=input("")
