# Kaggle_Vietnam_Bombing

This project required using Pig scripts in a Hadoop environment on a large dataset.  The task was to ask a 3 questions about a large dataset and answer them using the Apache Pig language.

With the following analysis, I demonstrate how data-driven analysis requires domain knowledge and investigation. A Data Analysis is driven by questions and research into a topic.

## Background

I downloaded a kaggle data set containing declassified U.S. military bombing operation data from the Vietnam War. The data was declassified in 2000 by President Clinton. I wanted to analyze accuracy of reported events using Apache Hadoop and Pig.

## Analysis 

According to history.com[1],

“Operation Rolling Thunder was the codename for an American bombing campaign during the Vietnam War. U.S. military aircraft attacked targets throughout North Vietnam from March 1965 to October 1968. This massive bombardment was intended to put military pressure on North Vietnam’s communist leaders and reduce their capacity to wage war against the U.S.-supported government of South Vietnam. Operation Rolling Thunder marked the first sustained American assault on North Vietnamese territory and represented a major expansion of U.S. involvement in the Vietnam War.

“The sustained bombing of North Vietnam lasted for more than three years, with occasional brief interruptions. Johnson finally halted the campaign on October 31, 1968, in order to pursue a negotiated settlement with the Communists.

### QUESTION 1: I want to know, between March 1965 and October 1968: What was the average daily mission count by the US against North Vietnam?

ANSWER 1:

year	avgdailymissioncount
1965	2072.7419354838707
1966	13296.838709677419
1967	19156.064516129034
1968	21984.870967741936

### QUESTION 2: How do these numbers compare to the missions before and after Operation Rolling Thunder?

ANSWER 2: The remainder of 1968 shows a dramatic decline in bombing operations. This is expected since President Nixon order a halt to the operations on October 31, 1968. Obviously, they were not entirely “halted” and they picked up dramatically again in 1989.

year	avgdailymissioncount
1968	3137.8064516129034
1969	17398.354838709678
1970	24592.516129032258
1971	15651.290322580646
1972	19459.41935483871
1973	8004.5161290322585
1974	3377.451612903226
1975	913.8064516129032

According to the same Article on History.com:
“By the time the last American combat troops left Vietnam in 1973, the U.S. military had dropped some 4.6 million tons of bombs on Vietnam, destroying a large percentage of the nation’s towns and villages and killing an estimated 2 million Vietnamese people.”

### QUESTION 3: How does this estimate compare to the kaggle bombing data set?
ANSWER 3:
tonsbombsdropped
3034157.7075

It's possible that the numbers don't match because the 4.6 million-figure includes the classified missions that were not in the Kaggle dataset.

## References

[1] http://www.history.com/topics/vietnam-war/operation-rolling-thunder

Data Source:
https://www.kaggle.com/usaf/vietnam-war-bombing-operations
