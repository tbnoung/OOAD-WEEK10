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
![](http://www.plantuml.com/plantuml/img/XP112eCm44NtSmgNxS8Bk13lqTMGV2IGH9aPKmevl7OXegMuVc_-WndKM6n9aLvjtxX5RKeGXPJWe5t3yonJmMCdJs9deR3XHoPoWYz876B8etxKaEYgjVs9TnblebjBaVsHFXTghRVt7X46ylYpGSCMsDwm0W00)
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

@enduml
