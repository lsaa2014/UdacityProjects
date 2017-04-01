# Summary
Titanic Data contains demographics and passenger information from 891 of the 2224 passengers and crew on board the Titanic.
This visualization shows the relationship between the fare and age of passengers. Most passengers embarked at Southampton and Cherbourg. 
Passengers from Cherbourg who payed a ticket higher than 400 were among the survived. Female survived than male and those who payed the most expensive ticket had more chance to survive.            

# Design
The Titanic data was obtained from <a href="https://www.kaggle.com/c/titanic/data"> Kaggle </a>. I used these variables:
- Age (Age in years) will be on the x-axis
- Fare (Passenger fare) will be on the y-axis
- Port of Embarkation (C = Cherbourg, Q = Queenstown, S = Southampton) will be represented by color encoding using different color for eac
- Sex, (female or male) will be represented by color encoding using different color for each.      

I choose the scatterplot to represent the relationship between age and fare based on the port of embarkation and gender.
Using Dimple.js, I created the first plot after removing the missing value as we can see
<a href="http://bl.ocks.org/lsaa2014/97e390dab1b74f9cd9915c3324c7237d"> here </a>. After the first two feedback, I mapped 
the columns Embarked (S:Southampton, C:Cherbourg, Q:Queenstown) and Survived (1:'Yes', 0: 'No') so that they could be more readable.
I also added some narration see <a href="http://bl.ocks.org/lsaa2014/38ec5a937eb84b17442e20033fad5ffa"> here </a>.
After the third feedback, I decided to filter the data and choose only those who survived and I removed the storyboard and left the legend as is. The final plot could be visualized <a href="http://bl.ocks.org/lsaa2014/bb2663e96cc13e858b77c13ba0ea2b31"> here </a>.

## Feedback
#### Feedback #1
<blockquote>
<p>
Add more descripton to narrate a story. Instead of abbreviations in the first graph as S,C,Q please do elaborate so that the buttons 
looks good. The y-axis could also be normalized in the first graph as it shows different values for different categories. 
The value of y-axis should be consistent.
</p>
</blockquote>

#### Feedback #2
<blockquote>
<p>
Your visualization is very nice.
Some feedbacks:
What do 0 and 1 stand for? I think you can add some text to describe that legend.
What do S, Q and C stand for?
Animation is awesome. However, the transition is too fast. I suggest you let people click on S,C and Q and the animation kicks in after pressing these buttons. Same thing happens with female and male.
</p>
</blockquote>

#### Feedback #3
<blockquote>
<p>
nice work!
So here is my feedback after having a short look at it:
- nice introduction text and story. I am not really getting the last conclusion though ("Female survived than male")
- I wanted to check your conclusion number 2 and therfore pause the animation at Cherbourg. It seems to automatically resume after about 5sec? It is just a bit short for me
- When reading the subtitle, I would expect to only see data about people that survived not the people that didn't.
I think it would also make it a bit easier to understand (1 less variable). Besides that, the Yes/No was not immediately clear to me. I think it's better to call it Survived/Not-Survived
- The relationship between age and fare looks indeed weak. For me it would be interesting to know some statistic about the relationship (r squared for example)
- I don't like it that the values on the axes are changing in the animation. It makes it hard to compare fares between port of embarkation. It might partly be cause by some outliers I guess.
Someone is aged 120+ and there is a fare of 1000+, shouldn't this be removed? 
</p>
</blockquote>

## Reference
- http://dimplejs.org/examples_index.html
- http://stackoverflow.com
- https://leanpub.com/D3-Tips-and-Tricks/read
