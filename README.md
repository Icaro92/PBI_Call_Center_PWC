# Call Center Dashboard
<p align = "center">
  <img src="https://github.com/Icaro92/PBI_AW/assets/58118599/59538c9b-fa24-4a14-8be9-6b389ed1dd13" width="600" alt="Call_Center_Dash">

## Objectives

This Dashboard aims to provide transparency and insight into the data received at a Call Centre. It provides an accurate overview of trends in customer and agent behavior.
KPIs included are:
  * Overall Customer Satisfaction
  * Overall calls Answered/Abandoned
  * Calls by time
  * Average Speed of Answer
  * Agent's performance quadrant: Average handle time vs. calls answered

You can access the dashboard in the link below:
  * [Call-Center Dasboard](https://app.powerbi.com/view?r=eyJrIjoiMjU3ZTA1ZDItOWFkYS00ZjkzLThjNmQtNzkzNWY2Y2I3OGE4IiwidCI6IjAyODQyZDljLWVhNTAtNGVkNy1iMWY1LWI2MDIwOGIwM2YzNyJ9)

## Data Source

This project was based on the [PwC in Switzerland](https://www.theforage.com/simulations/pwc-ch/power-bi-cqxg) job simulation from The Forage. The simulation provided data and directions into what was expected for the analysis.

## Business Request 
Claire, the Call Centre Manager at PhoneNow requested our services in the e-mail below. She's having trouble visualizing her call center data and wants an accurate overview of long-term customer and agent behavior trends. She even provided a few KPIs:  

<p align = "left">
  <img src="https://github.com/Icaro92/PBI_AW/assets/58118599/13a84a03-1fa6-4b94-955c-48e4dda7aa4f" width="600" alt="Claire Business Request">

## Power BI Data Transformation

To provide accurate data and make the visualizations meaningful, a few Measures were created using DAX:

* #_# of answered_ = Calculate(DISTINCTCOUNT('Sheet1 (2)'[Call Id]),Filter('Sheet1 (2)','Sheet1 (2)'[Answered (Y/N)]="Y"))
* #_# of resolved_ = Calculate(distinct('Sheet1 (2)'[Call Id]),Filter('Sheet1 (2)','Sheet1 (2)'[Resolved]="Y"))
* #_Target Value Satisfaction_ = 4.5

## The Dashboard

The finished dashboard provides a powerful overview of both Customer and Agent behavior through KPIs such as Calls Answered, Issues Resolved, Average speed of answer, amount of monthly calls NPS, and agent statistics. 

You can find the dash in the link below:
 * [Call-Center Dasboard](https://app.powerbi.com/view?r=eyJrIjoiMjU3ZTA1ZDItOWFkYS00ZjkzLThjNmQtNzkzNWY2Y2I3OGE4IiwidCI6IjAyODQyZDljLWVhNTAtNGVkNy1iMWY1LWI2MDIwOGIwM2YzNyJ9)

