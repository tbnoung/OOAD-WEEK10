# OOAD-WEEK10
Sequence Diagram

# 1
![](http://www.plantuml.com/plantuml/img/SoWkIImgAStDuU8ABKujKj2rKmYkB2v9pRLIyCbFpypJ08dc9UQcwXGa5XUNvnUbQ79nGLGew08LWwIXIXK2YlAJKukB5SeJYnMAIvD1xBHIeC5S3gbvAI0h0000)
##Code
@startuml

User -> System: Login(Username,password)

System --> User: Login Process was successful

@enduml

#2
![](http://www.plantuml.com/plantuml/img/XP0n2iCm34LtdI9ZEsHhbmmXz-Wax4yns4wG59U23zzaA6qQIkRt-0zfK6EnEKMwjNtZPhKnGHHIWeDs3K-JZ0MdDpaJEmk53JkPo0bMa3Z4aE_wL4EYNwtjDxpBU10TMehiF-bjeTRBjTR32Oy80tdycVa2kzE69RyywGK0)
##Code
@startuml

[-> customerservices: approve(customer)

activate customerservices

create mailingsystem

customerservices->mailingsystem:new

customerservices->mailingsystem:send

activate mailingsystem

|||

customerservices->mailingsystem:delete

deactivate mailingsystem

deactivate customerservices

@enduml
#3
![](http://www.plantuml.com/plantuml/img/SoWkIImgAStDuGejJYrAJip9IIrIqBLJ24vDB4hEi59mhKXDBYr9LU1AJ2x9B4i4iY0oN10AeTGrBpqpBzNGgXWYZQOSAik5mjErWzfIK9HQa5YKgf2JMPp1XJ0PuIAhuepySeXqIYgwIp14O9OvfEQb07q60000)
##Code
@startuml

Usercaller -> Search: Execute 

activate Search

Search -> SearchEngine1:search

activate SearchEngine1

SearchEngine1->Search:prepare lish

Search ->Usercaller:show lish

deactivate Search

deactivate SearchEngine1

@enduml

#4
![](http://www.plantuml.com/plantuml/img/PP1D2WCX38Ntdi8Bp0LS3BCfT2yzWDKm1FmfIIpqzhMZqg5T1NdVUybpOt4aDKLbfGR8efTLCoJCZWnaAZ5o5vJpWaydC6KrviVXIoK6RP17p2NYZlS8NrT7r22RPv1c1x4zwOeiXLudPgumSEHXjEAaiWhmctiwPZOnkXT8xV7lcoq6lQppdjiZD9t05mgiDiYXVSyR)
##Code
@startuml

Student -> seminar:enrollstudent

activate seminar

seminar -> course :isStudentEligible

activate course

course -> Student:getSeminarHistory

course -> seminar :eligibilStatus

deactivate course

seminar -> Student : enrollmentStatus

deactivate seminar

Student->Student:Updaterecords

@enduml
