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
