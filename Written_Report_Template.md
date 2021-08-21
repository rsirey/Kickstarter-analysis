# Kickstarting with Excel

## Overview of Project

### Purpose
The purpose of the analysis is to draw conclusions on success rates of Kickstarter campaigns across various categories,
sub categories, launch dates, countries of origin, goals, and other criteria. 
These conclusions are then to be used to plan future Kickstarter campaigns. The specific focus of this 
analysis is on the theater category, looking even more closely at the play subcategory. The analysis is intended for playwrite, Louise,
to have more successful campaigns in the future as her most recent play came close, but short of its fundraising goal. 

## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date
To analyze the outcome results based on launch date, a pivot table ![Outcomes_launchdate_PT.png](resources/Outcomes_launchdate_PT.png) was created using the entire data set 
using filters of Parent Category and year with outcomes in the column and the conversion date by month 
in the rows. The Parent Category was filtered to only include Kickstarters for the theater. This
gave a clear numeric table of outcomes (successful, failed, canceled) for each month. To better vizualize
these results, a line chart was created to show the trends of success status month to month.

### Analysis of Outcomes Based on Goals
To approach the analysis based on goals, buckets had to be created to better grasp the levels of amounts of goals.
Buckets were created in increments of $5000, ranging from less than $1000 to over $50000. The Countifs() were used to pull the number
successful, failed, and canceled Kickstarteres in each goal bucket of the play sub category. These number of successful, failed, 
and canceled Kickstarters for each bucket allowed a total to be summed for each bucket. Once the total was summed, a percentage
was calculated to show the percentage of successful, failed, and canceled Kickstarters in the play subcategory. The percentages 
made for a more intutive set of numbers to compare success vs failure. These percentages were then used to created a line chart
showing the success vs failure percentage across the varying buckets of goals set by Kickstarter campaigns.

### Challenges and Difficulties Encountered
In conducting this analysis, the Excel side was not too challenging. I ran into  some challenges with knowing which categories to put in
which areas of the pivot chart. Luckily, this is easy enough to use trial and error to find the best combination. The Countifs() were also a more 
involved function, but once I flushed out any spelling and spacing issues, the data pulled successfully. 

Github took some time to figure out, and I feel like I am not moving fluently through it yet, but it seems like something that will come with time
and repetition. Right now, I am most comfortable with uploading files by hand, but would like to get more comfortable with Gitpush.

## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?

The success of the theater Kickstarters shows a sigficant spike when launched in May and June, but overall, theater Kickstarters
show more success than failure with the exception of a December launch date. Not only are the fewest Kickstarters launched in December,
but the success rate is nearly 1:1, whereas in the peak of success, May, the success rate is over 2:1. Essentially, it can be concluded 
that a theater Kickstarter is likely to find success almost any month, most so when launched in May. The launch month with the lowest
chance for success is, historically, Decemeber.

- What can you conclude about the Outcomes based on Goals?

After conducting the Outcomes based on Goals analysis, it is appears that Kickstarters launched in the play subcaterogy see little to no
success in the $45,000 goal range and higher. There are varying levels of success in the amounts lower, however once reaching that threshold,
very few launches met their goal.

- What are some limitations of this dataset?

Limitations of the data set include not knowing who launched them, or if induviduals launched more than one. Knowing if certain induviduals saw 
more success than others over multiple launches could reveal a new trend in predicting future success of launches. It would also be useful to know
if the goal of the Kickstarter ended up being an accurate amount to fund the project. We are able to see if goals potentially correlated with outcomes,
but was the kickstarter actually successful if it raised its goal, but that amount was not enough to actually fund the project? Lastly, it would be useful
to know if there are shared backers between proejects in a geographical area.

The data also appears to have significant outliers, which make the Outcomes Based on Goals analysis misleading to an extent.

- What are some other possible tables and/or graphs that we could create?

An additional graph, or rather a repalcement would be for the second analysis. The line chart showing the success rate per goal bucket
does not take into account the face that the buckets had a wide range of number of Kickstarters total. For instance, the 1000 to 4999 bucket had a total 
of 534 launches, while the 35000-39999 only had 6, but there success rates are only separated by 5.99%. This chart is misleading in that it 
appears launches in the higher goal range have almost the same chance of success as the lower goal range, when in reality, there is not
enough data in the high range to support that. I think a bar graph with the number of total projects in each bucket and where each bar is broken into 
color blocks representing successful, failed, and canceled, would be more beneficial. This would show not only the success rate of each bucket, but the
number of proejcts available in the data set to calculate those success rates. 
