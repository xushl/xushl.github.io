## Interactive Charts Make Data Clearer

### Members
- Huanzhang Shen(沈焕彰): 320190940411
- Shenglin Xu(许圣麟): 320190940621
- Zexi He(何泽熹): 320190939991     
### Original Source
https://www.chinadailyhk.com/articles/210/245/84/1532946794238.html
This article describes the direction of education reform in Hong Kong, and we were intrigued by a visualization depicting the length of study and life satisfaction of Hong Kong students. We wanted to use it as a starting point to tell the story behind the visualization.

### Abstract

As one of the world's leading metropolises in terms of economy, Hong Kong has a peculiar phenomenon of high student commitment and low satisfaction in education. A visualization showing this phenomenon was published on a website of China Daily Hong Kong, and this essay attempts to modify this visualization using the technique of interactive charts to make it more legible and to introduce the reader to some cultural background about this phenomenon.

### Introduction
Hong Kong is a modern international metropolis. Its economy, culture and education are internationally renowned. However, the quality of students' study life in Hong Kong isn't as good as everyone generally believes. Because of the unique cultural background, parents in Hong Kong tend to generally want their children to be excellent learners and to excel in competition with others of their age.

As a result, many students have to face tremendous academic stress, and most parents do not have adequate and practical methods and knowledge to help their children relieve the stress. Despite their dedication to become a good student, Hong Kong students are not happy with their lives.

In this issue, we believe that the use of information visualization makes it easy for everyone to understand how the length of study and life satisfaction of students in each region compare. A clear and concise visualization would allow readers to quickly understand the magnitude of the plight faced by students in Hong Kong.

<img src="C:\Users\86136\Desktop\Project_2.jpg" style="zoom: 80%;" />

We chose this chart from a news site that briefly compares the correlation between the average length of study and life satisfaction for students in Hong Kong and students in some other regions using a scatter plot. 

### Details about the Original Chart

 we cite is from a news article on the China Daily Hong Kong website, and it shows the magnitude of the problem well. While Hong Kong students devote more time to their studies than students in most of the regions in the data, they tend to reap lower life satisfaction.
Specifically, this chart shows the current situation of Students in Hong Kong and its comparison with students in other OECD (Which stands for Organization for Economic Cooperation and Development, is an international governmental organization with 38 member countries) countries using a scatter plot. 

#### Chart We Reproduced

<img src="C:\Users\86136\Desktop\复现图片.png"  /> 

This chart is not simple, but quite easy to understand. 

- It has an x-axis representing the average number of hours students study per week and a y-axis representing students' life satisfaction (). 
- The data for students in each region are aggregated into a value that corresponds to a specific point in the scatter plot after some average-like processing.
-  In order to distinguish the data source of each data point, an abbreviation about the region is written in the data point. 
-  The reader can consult the legend to find out the full name of the region corresponding to each abbreviation. 
- We can see that the points in the figure are divided into two parts by color, and there is a red arrow at the HK point. Readers can be attracted by these visual elements and quickly realize the focus of this picture. This allows readers to better understand what this picture is trying to express
- In a nutshell, the coordinate corresponding to each point can reflect the current study pressure and balance state of study life of students in the country or region to a certain extent.

According to the data points in the graph, we can clearly see that most of the regions are concentrated in the upper left corner of the graph. This means that students in other regions tend to have a higher level of life satisfaction for a shorter amount of study time. Even if students in individual regions such as Italy and Russia study longer, their life satisfaction is quite higher than in Hong Kong.

In fact, many data show that this phenomenon is not only happening in Hong Kong. Students in Mainland China, Japan and other East Asian regions may be experiencing the same plight. How to promote the reform of education so that students can receive a happy and sound education is a major problem for them.

Admittedly, this chart is very intuitive to readers, but obviously it can do better.

### Improvements We Made(可能会加点图)

##### 1. Design a Better Labels

 In the original figure, the label of the Y axis is rotated with many explanatory words.

Obviously, this does not make users quickly understand what it means. So we decided to simplify the label and put it above the Y axis. Users can quickly notice it. At the same time, we also added a further explanation of the y-axis label at the bottom of the figure.

##### 2. Use Contrast Color
Two colors are used in the original figure to distinguish the data: cyan and blue. However, their contrast is not obvious, which tends to confuse the reader about the different data points. As a modification, we use the more contrasting dark blue and red, which are more eye-catching.

We believe that no matter how the visualization is done, when we need to reflect the contrast, we should use colors with larger distinctions whenever possible.

##### 3. Remove Redundant Elements

First, we remove the redundant grid, which we believe will only distract the reader's attention in this image.

Second, we remove the red arrow head attached to the data point "Hong Kong". We believe that the contrast between Hong Kong and the rest of the data points with light and dark tones is sufficient to distinguish the data. Extra elements would make the graph inconsistent.

In a general sense, we believe that redundant elements should be removed whenever possible. They make the diagram full of various elements that are not necessarily important. In fact, the human brain cannot remember so many elements, and too many elements only make the reader lose interest in the visualization.

##### 4. Make the Chart Interactive

Most importantly, we removed the complex legend used in the original chart to correspond to the country with its abbreviation. Actually, one of the main features of this visualization is its rather complex legend, which makes it difficult for the reader to understand the data in a straightforward way. If readers are curious about specific data for a particular region, they need to look up the corresponding data points through this complex legend. 

However, we believe that the graph is primarily intended to give the reader an idea of how Hong Kong compares to some sample countries, rather than to allow the reader to find out what the student life satisfaction situation is like in the region they are interested in. That is, the reader is less likely to need to look for the full name from the abbreviation than to check what the full name corresponding to the abbreviation is. 

 A website could use a more modern way of displaying charts to make it more convenient and easy for readers to understand the data. In fact, the combination of interactive technology and charts can make charts more exciting and clear to understand. With interactivity, charts become more dynamic. Users can click and move the cursor with more interesting animations. And, with the right settings, users can go from any node of the chart to the source of the data or to other charts.

In general, interactive charts provide a more vivid experience to users than static charts. At the same time, interactive charts also offer the possibility to make it easier to distribute data points too densely/scattered by zooming in/out of the chart.

However, when using interactive techniques, we also need to pay attention to the source of the chart. It is not wise to make interactive modifications to charts on traditional media because we cannot render html pages on a single sheet of paper.

### Final Look

Let's try to see the final chart, which becomes clear and simple, yet efficient. This is the beauty of visualization and the new breakthrough that interactive technology brings us.

<iframe 
height=600   
width=80% 
src="https://xushl.github.io/project2" 
allowfullscreen
</iframe>

### Conclusion

We are exposed to data visualization all the time in our daily lives. In the case we have chosen, for example, an accurate and concise visualization that allows the general public (not just the people involved) to understand the seriousness of the situation may be helpful to every member of the public community. After all, education, as an important part of the public sector, has a significant impact on almost everyone.

That's why the use of appropriate visualizations to make data more clearly presentable is an important topic for us mappers to consider. If visualizations are drawn using inappropriate methods, as in some of the cases we have seen in this case, they can make it difficult for readers to read or lose interest in the story behind the data.

We believe that the right modifications can make visualizations more efficient. In this case, the main solution we used was to use interactive techniques to make the visualization more vivid and straightforward.

Interaction techniques are amazing in that they can make the reader relate to seemingly "unchanging" data in a whole new way. But we should also be aware of the limitations of interactivity - without the right vehicle, making a chart interactive can be counterproductive.