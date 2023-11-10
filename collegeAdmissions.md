# Relational algebra

- College(cName,state,enrollment) cName
- Student(sID,sName,GPA,sizeHS) sID
- Apply(sID,cName,major,decision) (sID,cName,major)

<https://dbis-uibk.github.io/relax/calc/local/uibk/local/0>

<https://jordanbell.info/relax/calc/local/uibk/local/0>

```
group: collegeAdmissions

College = {
cName, state, enr
'NYU', 'NY', 55000
'Stanford', 'CA', 17000
'MIT', 'MA', 11000
'Penn', 'PA', 14000
'UCLA', 'CA', 44000
'Chicago', 'IL', 16000
}

Student = {
    sID:number, sName:string, GPA:number, HS:number
    1001, "Alex Johnson", 3.8, 400
    1002, "Maria Rodriguez", 3.6, 600
    1003, "Liu Wei", 3.9, 550
    1004, "Sophie Clark", 3.5, 300
    1005, "Raj Patel", 4.0, 450
    1006, "Emma Jones", 3.7, 500
    1007, "David Smith", 3.4, 350
    1008, "Isabella Garcia", 3.85, 420
    1009, "Michael Brown", 3.6, 520
    1010, "Sara Alizadeh", 3.95, 250
}

Apply = {
    sID:number, cName:string, major:string, decision:string
    1001, 'NYU', 'CS', 'Accept'
    1001, 'Stanford', 'CS', 'Accept'
    1001, 'MIT', 'CS', 'Reject'
    1002, 'NYU', 'Business', 'Reject'
    1002, 'MIT', 'Business', 'Accept'
    1003, 'NYU', 'Business', 'Accept'
    1003, 'Stanford', 'Business', 'Reject'
    1003, 'MIT', 'Business', 'Reject'
	1005, 'MIT', 'EE', 'Reject'
    1005, 'NYU', 'EE', 'Reject'
    1005, 'Stanford', 'EE', 'Reject'
    1005, 'UCLA', 'EE', 'Accept'
    1006, 'NYU', 'Business', 'Accept'
    1006, 'UCLA', 'Business', 'Accept'
    1006, 'Chicago', 'Business', 'Reject'
	1007, 'Penn', 'EE', 'Accept'
    1007, 'Penn', 'Business', 'Accept'
    1007, 'NYU', 'Business', 'Reject'
    1007, 'Chicago', 'Business', 'Reject'
    1008, 'Stanford', 'CS', 'Reject'
	1008, 'UCLA', 'CS', 'Accept'
    1008, 'MIT', 'CS', 'Accept'
    1009, 'NYU', 'Business', 'Reject'
    1009, 'UCLA', 'Business', 'Accept'    
    1009, 'Chicago', 'Business', 'Reject'
    1010, 'NYU', 'Business', 'Reject'
    1010, 'Penn', 'Business', 'Accept'
    1010, 'Chicago', 'Business', 'Reject'
}
```

