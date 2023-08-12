# 🛠️ YogaWellness 🛠️ 
YogaWellness is an application built on DAML that manages interactions between potential members and the yoga center owner.

### I. Overview 
This project was created by using the `empty-skeleton` template. 

YogaWellness is an application built on DAML that manages interactions between potential members and the yoga center owner. 
Potential members create enquiries and selecting options for callbacks, free sessions, and joining proposals. Yoga center owners review proposals and accept memberships.


### II. Workflow
1.	Potential member submits an enquiry for a yoga membership program by providing personal detils and yoga plan (YogaEnquiry contract is created).
2.	YogaEnquiry: The potential member can execute the choice to request a callback.
3.	YogaEnquiry: The potential member can execute the choice to book a free trial session.
4.	YogaEnquiry: The potential member can execute the choice to show interest in joining (YogaMembershipEnrollment is created).
5.	YogaMembershipEnrollment: Owner of the yoga center can see the interested member's enrollment proposal.
6.	YogaMembershipEnrollment: Owner of the yoga center can accept th enrollment proposal (YogaMembership contract is created)

### III. Challenge(s)
* YogaMembership contract requiring two signatories. It is handle using propose-accept model.

### IV. Compiling & Testing
To compile and test, run the pre-written script in the `Test.daml` under /daml OR run:
```
$ daml start
```

Test coverage report
```
$ daml test --show-coverage
