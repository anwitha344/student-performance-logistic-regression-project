# student-performance-logistic-regression-project
This project analyzes and predicts the academic performance of secondary school students using the UCI Student Performance dataset (Math class). The dataset contains demographic, social, and academic attributes for 395 students, including features such as study time, past failures, family support, absences, and grades.
The main goal of the project is to predict whether a student will pass or fail the course based on these factors using logistic regression 

## Getting the data 
I did this by directly visiting the website and downloading the csv file 
https://archive.ics.uci.edu/dataset/320/student+performance
I chose to use only the math file 

## Analyising the data 
Using pandas and matplotlib i analysed and visualised the data to unrstand the data im working with 
### 1. Data set shape:
   index,school,sex,age,address,famsize,Pstatus,Medu,Fedu,Mjob,Fjob,reason,guardian,traveltime,studytime,failures,schoolsup,famsup,paid,activities,nursery
0,GP,F,18,U,GT3,A,4,4,at_home,teacher,course,mother,2,2,0,yes,no,no,no,yes
1,GP,F,17,U,GT3,T,1,1,at_home,other,course,father,1,2,0,no,yes,no,no,no
2,GP,F,15,U,LE3,T,1,1,at_home,other,other,mother,1,2,3,yes,no,yes,no,yes
3,GP,F,15,U,GT3,T,4,2,health,services,home,mother,1,3,0,no,yes,yes,yes,yes
4,GP,F,16,U,GT3,T,3,3,other,other,home,father,1,2,0,no,yes,yes,no,yes

### 2. checking for any missing values
   missing count
school        0
sex           0
age           0
address       0
famsize       0
Pstatus       0
Medu          0
Fedu          0
Mjob          0
Fjob          0
reason        0
guardian      0
traveltime    0
studytime     0
failures      0
schoolsup     0
famsup        0
paid          0
activities    0
nursery       0
higher        0
internet      0
romantic      0
famrel        0
freetime      0
goout         0
Dalc          0
Walc          0
health        0
absences      0
G1            0
G2            0
G3            0
dtype: int64

### 3. Checking further information about each column and plotting the correlation matrix 
Value counts for school:
school
GP    349
MS     46
Name: count, dtype: int64

Value counts for sex:
sex
F    208
M    187
Name: count, dtype: int64

Value counts for address:
address
U    307
R     88
Name: count, dtype: int64

Value counts for famsize:
famsize
GT3    281
LE3    114
Name: count, dtype: int64

Value counts for Pstatus:
Pstatus
T    354
A     41
Name: count, dtype: int64

Value counts for Mjob:
Mjob
other       141
services    103
at_home      59
teacher      58
health       34
Name: count, dtype: int64

Value counts for Fjob:
Fjob
other       217
services    111
teacher      29
at_home      20
health       18
Name: count, dtype: int64

Value counts for reason:
reason
course        145
home          109
reputation    105
other          36
Name: count, dtype: int64

Value counts for guardian:
guardian
mother    273
father     90
other      32
Name: count, dtype: int64

Value counts for schoolsup:
schoolsup
no     344
yes     51
Name: count, dtype: int64

Value counts for famsup:
famsup
yes    242
no     153
Name: count, dtype: int64

Value counts for paid:
paid
no     214
yes    181
Name: count, dtype: int64

Value counts for activities:
activities
yes    201
no     194
Name: count, dtype: int64

Value counts for nursery:
nursery
yes    314
no      81
Name: count, dtype: int64

Value counts for higher:
higher
yes    375
no      20
Name: count, dtype: int64

Value counts for internet:
internet
yes    329
no      66
Name: count, dtype: int64

Value counts for romantic:
romantic
no     263
yes    132
Name: count, dtype: int64

###


