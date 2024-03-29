## Interactive Visualizations Make Data Clearer

##### The Project2 Report of Group24

you can read this report in our [github page](https://xushl.github.io/InteractiveVisualizations).

### Members

- Huanzhang Shen(沈焕彰): 320190940411
- Shenglin Xu(许圣麟): 320190940621
- Zexi He(何泽熹): 320190939991     


### Abstract
Visualizing data is a task that we see everywhere in our daily lives. However, it is not easy to present the data properly to the readers. For websites or some modern media, the use of interactive charts may make visualization more efficient.

To introduce this, we have selected an information visualization from China Daily HK. It presents a particular phenomenon in Hong Kong education: high student engagement and low satisfaction with education.

We will analyze and modify this visualization to make it more in line with some good visualization guidelines. Most importantly, we will turn it into an efficient interactive visualization.

### Original Source
The original source is from https://www.chinadailyhk.com.
As presented in the abstract, the [article](https://www.chinadailyhk.com/articles/210/245/84/1532946794238.html) describes the direction of education reform in Hong Kong, and we were intrigued by a visualization depicting the length of study and life satisfaction of Hong Kong students. We wanted to use it as a starting point to carry our other works.

### Introduction of the Backstory and Basic Analysis
Hong Kong is one of the most developed cities in China. Its economy, culture and education are internationally renowned. However, the quality of students' study life in Hong Kong isn't as good as everyone generally believes. Because of the unique cultural background, parents in Hong Kong tend to generally want their children to be excellent learners and to excel in competition with others of their age.

As a result, many students have to face tremendous academic stress, and most parents do not have adequate and practical methods and knowledge to help their children relieve the stress. Despite their dedication to become a good student, Hong Kong students are not happy with their lives.

This visualization attempts to use a scatter plot to compare the learning engagement and life satisfaction of students in Hong Kong with the corresponding situation in other OCED countries. We think it would be very wise indeed to use information visualization here. The information visualization makes it easy for everyone to understand how the length of study and life satisfaction of students in each region compare. A clear and concise visualization would allow readers to quickly understand the magnitude of the plight faced by students in Hong Kong.

<img src="https://www.chinadailyhk.com/attachments/image/71/4/112/394699_111343/394699_111343_800_auto_jpg.jpg" style="zoom: 100%;" />

<center>Fig1. The Chart from Original Source</center>

You may think that this chart has basically accomplished its mission, but we still think that it could probably be better. In short, it is not efficient and has many distracting and confusing elements. However, before we talk about how to make it better, maybe we need to analyze how it is a visualization.

### Details about the Original Chart
As we have mentioned repeatedly, this original visualization is from a news article on the China Daily Hong Kong website, and it shows the magnitude of the problem. While Hong Kong students devote more time to their studies than students in most of the regions in the data, they tend to reap lower life satisfaction.

Specifically, this chart shows the current situation of Students in Hong Kong and its comparison with students in other OECD (Which stands for Organization for Economic Cooperation and Development, is an international governmental organization with 38 member countries) countries using a scatter plot. 

We will first reproduce it using matplotlib and introduce you to the basic structure of this chart.

##### The Structure of Original Chart
<img src="./original.png" style="zoom: 40%;" /> 

<center>Fig2. The Replicated Chart</center>

As you can see, this chart is not simple, but quite easy to understand. It has the following basic structure:

- It has an x-axis representing the average number of hours students study per week and a y-axis representing students' life satisfaction. 
- The data for students in each region are aggregated into a value that corresponds to a specific point in the scatter plot after some average-like processing.
- In order to distinguish the data source of each data point, an abbreviation about the region is written in the data point. 
- The reader can consult the legend to find out the full name of the region corresponding to each abbreviation. 
- We can see that the points in the chart are divided into two parts by color. Apart from that, there is a red arrow at the HK point. Readers can be attracted by these visual elements and quickly realize the focus of this chart. This allows readers to better understand what this chart is trying to express
- In a nutshell, the coordinate corresponding to each point can reflect the current study pressure and balance state of study life of students in the country or region to a certain extent.

##### Corresponding Analysis, and Background
According to the data points in the chart, we can clearly see that most of the regions are concentrated in the upper left corner of the chart. This means that students in other regions tend to have a higher level of life satisfaction for a shorter amount of study time. Even if students in individual regions such as Italy and Russia study longer, their life satisfaction is quite higher than in Hong Kong.

We regret to inform you that, many data show that this phenomenon is not only happening in Hong Kong. Students in Mainland China, Japan and other East Asian regions may be experiencing the same plight. How to promote the reform of education so that students can receive a happy and sound education is a major problem for them. In fact, this is exactly why we have chosen such a visualization to modify. It reveals a rather serious problem and, as a result, it takes on the greater responsibility of making it all clear to the reader.

Admittedly, we have to praise that this visualization is very intuitive to readers, but obviously it can do better. Now, we will show you our approach.

### Improvements We Made

##### 1. Design a Better Labels
In the original chart, the label of the Y axis is rotated with many explanatory words. Obviously, this does not make users quickly understand what it means. 

<img src=".\1.png" style="zoom: 60%;" />

<center>Fig3. The Original Labels</center>


So we decided to simplify the label and put it above the Y axis. Users can quickly notice it. At the same time, we also added a further explanation of the y-axis label at the bottom of the chart.

<img src=".\2.png" style="zoom: 66%;" />

<center>Fig4. The Improved Labels</center>

##### 2. Use Contrast Color
Two colors are used in the original chart to distinguish the data: cyan and blue. However, their contrast is not obvious, which tends to confuse the reader about the different data points. As a modification, we use the more contrasting dark blue and red, which are more eye-catching. In addition, the contrast between cyan and white text is not obvious, so we use a darker blue to highlight this contrast, as in the follow image:



<img src=".\5.png" style="zoom: 30%;" />

<center>Fig5. Words on Different Colored Backgrounds</center>

We believe that no matter how the visualization is done, when we need to reflect the contrast, we should use colors with larger distinctions whenever possible.

##### 3. Remove Redundant Elements
First, we remove the redundant grid, which we believe will only distract the reader's attention in this chart.

Second, we remove the red arrow head attached to the data point "Hong Kong". The different colors are enough to allow the reader to distinguish the difference between the two kinds of data points. Extra elements would only make the chart inconsistent.

In a general sense, we believe that redundant elements should be removed whenever possible. They make the chart full of various elements that are not necessarily important. In fact, the human brain cannot remember so many elements, and too many elements only make the reader lose interest in the visualization.

##### 4. Make the Chart Interactive
Most importantly, we have replaced the complex legends in the original charts with fun and interactive tip boxes. Actually, one of the main features of this visualization is its rather complex legend, which makes it difficult for the reader to understand the data in a straightforward way. If readers are curious about specific data for a particular region, they need to look up the corresponding data points through this complex legend. 

<img src="./3.png" alt="image" style="zoom:60%;" />

<center>Fig6. The Original Legends</center>

However, we thought that the chart is primarily intended to give the reader an idea of how Hong Kong compares to some sample countries, rather than to allow the reader to find out what the student life satisfaction situation is like in the region they are interested in. That is, the reader is less likely to need to look for the full name from the abbreviation than to check what the full name corresponding to the abbreviation is. 

Actually, a website could use a more modern way of displaying charts to make it more convenient and easy for readers to understand the data. The combination of interactive technology and visualization may can make charts more exciting and clear to understand. With interactivity, visualizations become more dynamic, users can click and move the cursor with more interesting animations. And, with the right settings, users can get everything they want to know with a single click.

<img src="./4.png" alt="image-20211201203150230" style="zoom:67%;" />

<center>Fig7. The Interactive Legends</center>

In general, interactive visualization provide a more vivid experience to users than static visualizations. But we need to be reminded that when we use visualization techniques, we still need to be aware of the source of the charts. It is not wise to make interactive modifications to charts on traditional media because we cannot render html pages on a single sheet of paper.

### Final Look
Let's try to see the final visualization, which becomes clear and simple, yet efficient. This is the beauty of visualization and the new breakthrough that interactive technology brings us.

<iframe 
height=520  
width=80% 
src="./improved_graph.html" 
allowfullscreen
</iframe>

<center>Fig8. The Final Visualization </center>

### Conclusion
We are using data visualization all the time in our daily lives. In the case we have chosen, for example, an accurate and concise visualization is very necessary. After all, as members of the community, we have an obligation to let everyone know that a group of people are in such a difficult situation. On a personal note, we, a group of students, also see the value in making more people aware of the pressures students face.

That's why the use of appropriate visualizations to make data more clearly presentable is an important topic for us authors to consider. If visualizations are drawn using inappropriate methods, as in some of the cases we have seen in this case, they can make it difficult for readers to read or lose interest in the story behind the data.

We believe that the right modifications can make visualizations more efficient, and also allows the story behind the visualization to be more accurately communicated to the reader. In this case, the main solution we used was to use interactive techniques to make the visualization more vivid and straightforward. Perhaps you will be as excited as we are when you first click on the data points on the chart.

Interaction techniques are amazing in that they can make the reader relate to seemingly "unchanging" data in a whole new way. As the personal use of electronic devices gradually become more and more, perhaps it will bring a radical new change to the visualization technology. But we have to warn you: interactive charts still have their limitations - without the right vehicle, making a chart interactive can be counterproductive.