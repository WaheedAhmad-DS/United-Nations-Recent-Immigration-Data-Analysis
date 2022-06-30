## Table of Contents
* [Project Title & Introduction](#project-title--introduction)
* [Project Motivation](#project-motivation) 
* [Project Objectives](#project-objectives)
* [Technologies Used](#technologies-used)                                       
* [Data Understanding & Preparation](#data-understanding--preparation)      
* [Project Visuals/EDA]()                            
                                                                                 
    * [1.The overall trend of immigration to Germany from 1990 to 2019.](#1the-overall-trend-of-immigration-to-germany-from-1990-to-2019)      
    * [2.The countries that contributed the most and the least towards immigration to Germany.](#2the-countries-that-contributed-the-most-and-the-least-towards-immigration-to-germany)      
    * [3.Syrian civil war effect on Germany.](#3syrian-civil-war-effect-on-germany)        
    * [4.Least and most popular countries where Germans moved to.](#4least-and-most-popular-countries-where-germans-moved-to)     
    * [5.Least and most popular countries where Pakistanis moved to.](#5least-and-most-popular-countries-where-pakistanis-moved-to)  
    * [6.What's the trend of people moving from Pakistan to Germany in comparison to people moving from India and China?](#6whats-the-trend-of-people-moving-from-pakistan-to-germany-in-comparison-to-people-moving-from-india-and-china)
    * [7.Afghan war effect on Pakistan.](#7afghan-war-effect-on-pakistan)
* [Conclusion](#conclusion)  

## Project Title & Introduction               

### Data Analysis of United Nations (UN) International migrant stock 2019. 

The dataset can be found here.<nav><a href="https://www.un.org/en/development/desa/population/migration/data/estimates2/estimates19.asp"> International migrant stock 2019 </a>   

The dataset presents estimates of international migrant by age, sex and origin. Estimates are presented for 1990, 1995, 2000, 2005, 2010, 2015 and 2019 and are available for all countries and areas of the world. The estimates are based on official statistics on the foreign-born or the foreign population.
***
## Project Motivation                                
[(Back to top)](#table-of-contents)   
  
A lot of people migrate every year from one place to other for better living conditions, to find better working places with humane conditions for employees, and to raise their children in a better socio-economic environment. The reasons could vary from personal, professional advancement to just exploring new places, cultures, languages and people. Lately, I also have been thinking about moving back to Europe from where I completed my MS in Astrophysics or probably North American side of the world.     
  
Therefore, I wanted to see if any data is available on immigration and what better data could be there than UN Immigration data. The dataset available was the most recent one at the time of analysis. 
***
## Project Objectives                                
[(Back to top)](#table-of-contents)           
 
The goals of the project were to find insights about the following topics:        
  * Trend of Immigration to and from Germany. 
  * The countries that contributed the most and the least towards immigration to Germany. 
  * Syrian civil war effect on Germany. Germany was in the news for opening its borders for immigrants from Syria.
  * People from developing countries move to developed countries all the time, but did people from developed countries also move to somewhere else? 
  * Where did Pakistanis move? What's the trend from Pakistan to Germany in comparison to India and China? 
  * Afghan war effect on Pakistan. Pakistan was accepting a lot of immigrants from Afghanistan due to war conditions there. 

These were a few of the exciting questions i wanted to find answers to; ***answers proven by data.*** 
***  
## Technologies Used                                     
[(Back to top)](#table-of-contents)                                   

A list of technologies used within the project:
* Python
* Pandas
* Numpy
* Matplotlib
* Seaborn
***
## Data Understanding & Preparation     

The excel file contains different files within itself; I used the total immigrants file, although the data is also available as male and female migrants stock. The first 15 rows were skipped while reading the data. Because it contained general information and column headers started from below.    
  
![alt text](https://github.com/WaheedAhmad-DS/United-Nations-Recent-Immigration-Data-Analysis/blob/main/Images/15%20rows%20skipped.png)     

  * Columns contained the area of origin (country name) and **'Area of destination'**, **'Year'** and **'Total'** immigrants in that year from all countries to area of destination.
  
  * Some columns were dropped and some were renamed. Please see the ipynb notebook.
  
  * Null values either meant that the data was not available or there was 0 (zero) migration from that country to **'Area of destination'** in that particular **'Year'**. Therefore the missing values were replaced by zeros.      
  
  * So after data wrangling part the final data frame looked like this:     
  
![alt text](https://github.com/WaheedAhmad-DS/United-Nations-Recent-Immigration-Data-Analysis/blob/main/Images/Final%20df.png)     
*** 
[(Back to top)](#table-of-contents) 

## Project Visuals/EDA            

To get insights related to particular countries, different data frames were created by applying condition such as **'Area of destination' == 'Germany' or 'Pakistan'** or depending upon the question.      

***Please check the notebook for code examples.***
![alt text](https://github.com/WaheedAhmad-DS/United-Nations-Recent-Immigration-Data-Analysis/blob/main/Images/DF-DE.png)
  ### 1.The overall trend of immigration to Germany from 1990 to 2019.     
  ![alt text](https://github.com/WaheedAhmad-DS/United-Nations-Recent-Immigration-Data-Analysis/blob/main/Images/Overall%20Trend%20of%20Immigration%20to%20Germany.png)
  
  * ***There is an overall increasing trend of people moving to Germany.***  
  
  [(Back to top)](#table-of-contents) 
  
  ### 2.The countries that contributed the most and the least towards immigration to Germany. 
  ![alt text](https://github.com/WaheedAhmad-DS/United-Nations-Recent-Immigration-Data-Analysis/blob/main/Images/Most%20Contributions%20to%20DE%20Immigration.png)
  
  * ***Most of the immigrants are from Turkey. But surprisingly, some EU countries are also there, for example, Austria, Italy, and Poland.*** 
  
  ![alt text](https://github.com/WaheedAhmad-DS/United-Nations-Recent-Immigration-Data-Analysis/blob/main/Images/Least%20Contribution%20to%20DE.png)    
  
  * ***Only few people immigrated to Germany from some African and Central American nations.*** 
  
  [(Back to top)](#table-of-contents) 
  
  ### 3.Syrian civil war effect on Germany.          
  ![alt text](https://github.com/WaheedAhmad-DS/United-Nations-Recent-Immigration-Data-Analysis/blob/main/Images/Syrian%20War%20effect%20on%20DE.png)  
  
  * ***The war was started in 2011. And it can be clearly seen that an exponentially huge amount of immigrants were placed in Germany from 2015 to 2019, in comparison to earlier years.*** 
  
  [(Back to top)](#table-of-contents) 
  
  ### 4.Least and most popular countries where Germans moved to.           
  ![alt text](https://github.com/WaheedAhmad-DS/United-Nations-Recent-Immigration-Data-Analysis/blob/main/Images/From%20DE-%20to%20developed.png)
  
  * ***In 2019, more than 0.5 Millions Germans moved to USA also known as the land of opportunities.*** 
  
  * ***And where they didn't prefer to move is below.***     
  
  ![alt text](https://github.com/WaheedAhmad-DS/United-Nations-Recent-Immigration-Data-Analysis/blob/main/Images/From-DE%20to%20least%20developed.png)   
  
  [(Back to top)](#table-of-contents) 
  
  ### 5.Least and most popular countries where Pakistanis moved to.                  
  ![alt text](https://github.com/WaheedAhmad-DS/United-Nations-Recent-Immigration-Data-Analysis/blob/main/Images/pak-moving-to.png)  
  
  * ***Saudi Arabia was the most popular destination in 2019 for the people from Pakistan . Thousands of Pakistanis migrate for work every year and that is mostly labor migration.***
  
  * ***And where they didn't prefer to move is below.*** 
  
  ![alt text](https://github.com/WaheedAhmad-DS/United-Nations-Recent-Immigration-Data-Analysis/blob/main/Images/Pak-%20to%20-least%20developed.png)
  
  [(Back to top)](#table-of-contents)   
  
  ### 6.What's the trend of people moving from Pakistan to Germany in comparison to people moving from India and China?          
  ![alt text](https://github.com/WaheedAhmad-DS/United-Nations-Recent-Immigration-Data-Analysis/blob/main/Images/Pak-to-DE.png)    
  
  
  ![alt text](https://github.com/WaheedAhmad-DS/United-Nations-Recent-Immigration-Data-Analysis/blob/main/Images/I-C-P%20to%20DE.png)
  
  * ***There is an overall similar growing trend but more people in number have moved from China.***  
  
  [(Back to top)](#table-of-contents) 
  
  ### 7.Afghan war effect on Pakistan.
  ![alt text](https://github.com/WaheedAhmad-DS/United-Nations-Recent-Immigration-Data-Analysis/blob/main/Images/Immigration%20to%20Pak.png) 
  
  * ***The overall trend is of decline, probably because of high inflation rate and Pakistan being a developing country. And also may be because of how media portrays the soft images of different countries*** 
  
  ![alt text](https://github.com/WaheedAhmad-DS/United-Nations-Recent-Immigration-Data-Analysis/blob/main/Images/Afghan%20war.png)
  
  * ***A lot of Afghanis have moved to neighboring countries due to war-torn situations.***
  
  [(Back to top)](#table-of-contents) 
***
## Conclusion  
  A few questions I was interested in have been answered above; however, the limit is sky regarding the analysis of this dataset. There are a lot of areas of destination and areas of origin. So, it depends upon the project goals and objectives i.e. what you want to do with it. A lot can be done with this dataset depending upon the personal or professional interests. For example, the ratio of male to female migrants is another domain of research. Therefore, feel free to use the ipynb notebook available in the repository.  
***
