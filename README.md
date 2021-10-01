# Pewlett-Hackard-Analysis

## Overview of Project
**Explain the purpose of the new analysis.**

In this analysis, we will create a Retirement Titles table which will include the current employees who were born between January 1, 1952 and Deecember 31, 1955. This will determine which employees will be retiring soon and which posistions will need to be filled.



## Results
**Provide a bulleted list with four major points from the two analysis deliverables. Use images as support where needed.**

* There are around 90,000 retiring titles that would need to be replaced with new employee
* The highest number of employees that will retire are the ones having "Senior Engineer" title and "Senior Staff title" and the lowest number of employees retired is the "Managers"
* There is a high number of Engineers retiring as the one who hold a senior position, or assistant position.

![retired_titles](https://github.com/roxhensa02/Pewlett-Hackard-Analysis/blob/main/Data/Retiring_titles.PNG)

* The number of mentors in the company is very low, especially the qualified Engineers.

![mentorship_eligibility](https://github.com/roxhensa02/Pewlett-Hackard-Analysis/blob/main/Data/Mentorship_Eligibility.PNG)



## Summary

**Provide high-level responses to the following questions, then provide two additional queries or tables that may provide more insight into the upcoming "silver tsunami."**

**How many roles will need to be filled as the "silver tsunami" begins to make an impact?**

The number of roles that needs to be filles is approxitmally 90,000 roles, which is a very high number
* Senior Engineer: 29,414
* Senior Staff: 28,254
* Engineer: 14,222
* Staff: 12,243
* Technique Leader: 4,502
* Assistant Engineer: 1,761
* Manager: 2

**Are there enough qualified, retirement-ready employees in the departments to mentor the next generation of Pewlett Hackard employees?**

**Query:** select count(title), title
from mentorship_eligibility
group by title
order by count(title) desc;

 After running the querie to group the mentors in the company by their role, we can determine that there is not enough qualified mentors in the company.
The number of mentors in the company are as below:
* Senior Staff: 414
* Enginier: 411
* Staff: 310
* Senior Engineer: 285
* Technique Leader: 77
* Assistant Engineer: 52

After analyzing the number of retiring employees and the mentors left, the company needs to place an urgent project on firing new people and training the excisting employees and the new hires.
