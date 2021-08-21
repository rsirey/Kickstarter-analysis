# Kickstarting with Excel

## Overview of Project

### Purpose
The purpose of the analysis is to  draw conclusions on success rates of Kickstarter campaigns across various categories,
 sub categories,  launch dates,countries of origin, goals, and other criteria. 
These conclusions are then to be used to plan future Kickstarter campaigns. The specific focus of this 
analysis is on the theatre category, looking even more closely at the play subcategory. The analysis 

## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date
To analyze the Outcome results based on launch date, a pivot table was created using the entire data set 
using filters of Parent Category and year with outcomes in the column and the conversion date by month 
in the rows. The Parent Category was filtered to only include Kickstarters for the theater. This
gave a clear numeric table of outcomes (successful, failed, canceled) for each month. To better vizualize
these results, a line chart was created to show the trends of success status month to month.

### Analysis of Outcomes Based on Goals
To approach the analysis based on goals, buckets had to be created to better grasp the levels of amounts of goals.
Buckets were created in increments of $5000, ranging from less than $1000 to over $50000. Countifs were used to pull the number
successful, failed, and canceled Kickstarteres in each goal bucket of the play sub category. These number of successful, failed, 
and canceled Kickstarters for each bucket allowed a total to be summed for each bucket. Once the total was summed, a percentage
was calculated to show the percentage of successful, failed, and canceled Kickstarters in the play subcategory. The percentages 
made for a more intutive set of numbers to compare success vs failure. These percentages were then used to created a line chart
showing the success vs failure percentage across the varying buckets of goals set by Kickstarter campaigns.

### Challenges and Difficulties Encountered

## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?
The success of the theater Kickstarters shows a sigficant spike when launched in May and June, but overall, theater Kickstarters
show more success than failure with the exception of a December launch date. Not only are the fewest Kickstarters launched in December,
but the success rate is nearly 1:1, whereas in the peak of success, May, the success rate is over 2:1. Essentially, it can be concluded 
that a theater Kickstarter is likely to find success almost any month, most so when launched in May. The launch month with the lowest
chance for success is, historically, Decemeber.

- What can you conclude about the Outcomes based on Goals?

- What are some limitations of this dataset?

- What are some other possible tables and/or graphs that we could create?
