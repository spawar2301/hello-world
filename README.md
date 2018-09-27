# hello-world
first program
def student_id(col):
    if col>20 or col <5:
        return 'Fail'
    else:
        return 'Pass'
    

def patient_id(col):
    if col==0 or col <0:
        return 'Fail'
    else:
        return 'Pass'

def gender(col):
    if col>20 or col <5:
        return 'Fail'
    else:
        return 'Pass'
    
def age_years(col):
    if col>20 or col <5:
        return 'Fail'
    else:
        return 'Pass'
    
def age_months(col):
    if col>20 or col <5:
        return 'Fail'
    else:
        return 'Pass'
    
def date_inclusion(col):
    if col>20 or col <5:
        return 'Fail'
    else:
        return 'Pass'

df2=pd.DataFrame()
a=df1['age_years'].apply(age_years)

df1=pd.read_csv(path)
df1.describe()
df1.info()

for i in range(len(df1.columns)):
    if df1.columns[i]=='student_id':
        df2['student_id']=df1['student_id'].apply(student_id)
        
    elif df1.columns[i]=='patient_id':
        df2['patient_id']=df1['patient_id'].apply(patient_id)
    
    elif df1.columns[i]=='gender':
        df2['gender']=df1['gender'].apply(gender)
    
    elif df1.columns[i]=='age_years':
        df2['age_years']=df1['age_years'].apply(age_years)
     
    elif df1.columns[i]=='age_months':
        df2['age_months']=df1['age_months'].apply(age_months)
    
    else: 
        df2['date_inclusion']=df1['student_id'].apply(date_inclusion)
