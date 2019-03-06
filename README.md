# Medicare Part D Prescribers:
## STA 141B Final Project
#### By: Liam Kussman

According to a variety of news sources, such as the [Huffington Post](https://www.huffingtonpost.com/entry/the-high-cost-of-prescription-drugs-in-the-united-states_us_59a606aae4b0d81379a81c1f), the price of prescription drugs per capita is higher in the U.S. than in any other country in the world.  During my personal experience working as an Actuarial Intern for the Marsh & McLennan Agency, a private health insurance broker, I learned that it was industry wide practice to assume a **8-12% rise in prescription drug costs per person every year** when forecasting future plan costs.  This is roughly equivalent to assuming that the cost of prescriptions per person to double every **6 - 9 years**.  As someone with a lot less experience in the health insurance field than my peers, I found it extreme to assume that costs of prescriptions increased so drastically every year.

Thus, for my final project, I decided to look at the Medicare Part D [prescriber data provided publicly by the CMS (Center for Medicare Services) from 2013 - 2015](https://www.cms.gov/Research-Statistics-Data-and-Systems/Statistics-Trends-and-Reports/Medicare-Provider-Charge-Data/Part-D-Prescriber.html). In case you don't know, Medicare is a federal health insurance program for the elderly (those over 65), some young people with disabilities, and those with End-Stage Renal (Kidney) disease.  Medicare coverage is split across 4 different lines of coverage, explained well by the graphic from https://www.gatewayhealthplan.com/medicare/learn-about-medicare/medicare-basics below (to my understanding Part A is free, but individuals must pay a small premium to enroll in Part B, C, or D):

![Source: https://www.gatewayhealthplan.com/medicare/learn-about-medicare/medicare-basics](https://www.gatewayhealthplan.com/portals/0/Images/1.2.1%20Medicare%20Basics%20V2A.JPG?ver=2017-04-17-134729-810)

The CMS provdies data for each provider (e.g. Doctor, Nurse, Specialist, etc.) who prescribes drugs to patients enrolled in the Part D segement of Medicare. For each provider and each drug, the dataset provides the total number of prescriptions that were dispensed and the total drug cost (includes any taxes or fees). Due to the large number of combinations of doctors and drugs, each year's data file is quite large (over 3 GB), thus I use large data methods to get a handle and work on the data (see more in `Data Processing.ipynb`). 

In my analysis (**See `Data Analysis.ipynb`**), I hope to address/answer the following questions:

* What is the cost distribution by state? Does this make sense intuitively?
* Are there any patterns in outlying prescribers?  Does it appear that any of these prescribers are blatantly committing fraud?
* Is there a significant cost difference in generic drugs versus brand name drugs?
* Does the average cost of drugs increase by 8-12% per year (as assumed in the private insurance market)?  What seems to be driving this increase?
