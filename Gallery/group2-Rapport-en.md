# Analysis of Mobile Application Usage Habits

## Project Link
This project was carried out by Viet Anh NGUYEN and Sofia MABROUK.

## Context and Motivation
Today, we are all addicted to our smartphones, often unaware of the time spent on applications. Through our visualizations, we provide a detailed analysis of application usage patterns throughout the day over a duration of 11 months for an individual. Our goal is not to stigmatize smartphone use but rather to emphasize the importance of conscious use of technology. We aim to empower users by providing a comprehensive yet precise view of their interactions with technology.

## Target Audience
We primarily target three categories of individuals:

### Developers
This visualization provides developers with a unique perspective on how users interact with an application at different times of the day. This information can assist them in making design adjustments to optimize the user experience, more accurately meeting users' needs and habits.

### Marketing
From a marketing perspective, this analysis can be very insightful. Understanding usage patterns at different times allows more effective targeting of advertising campaigns. This helps maximize advertising impact by delivering content at the optimal times to engage users.

### Behavioral Science Researchers
In the realm of research, our visualization can be a valuable resource for behavioral science researchers. It provides an in-depth exploration of behavioral patterns related to the digital world, paving the way for comprehensive studies on the relationship between individuals and their phones.

## Chosen Data Sources
For data collection, our initial goal was to extract our own application usage data. However, no application allowed us to obtain data over a one-year period; all applications provided data only from the first day of download (just for the month of December). Faced with this limitation, we conducted a search on Google Scholar, Chrome, and Kaggle.

The search was relatively lengthy because we specifically sought datasets covering an extended period to gather sufficient information. Ultimately, we identified the dataset at [Kaggle](https://www.kaggle.com/datasets/arul08/mobile-usage-dataset-individual-person/data), offering mobile application usage data for an individual over a period of 7 months. This rich dataset allowed us to create compelling visualizations and identify interesting patterns.

## Data Preprocessing and Languages Used
For data preprocessing, we used the Python language:

""" conda create --name M2_DataViz python=3.8

conda activate M2_DataViz

pip install -r requirements.txt

"""

## Visualizations
Our visualizations were created in JavaScript using primarily the D3 library.

### First Visualization
The first visualization is a bubble chart designed to illustrate the temporal evolution of mobile application usage habits. The idea of creating this bubble chart originated after discovering a visualization by Mr. Nathan YAU: [A Day in the Life of Americans](https://flowingdata.com/2015/12/15/a-day-in-the-life-of-americans/). This caught our attention, and we decided to create a similar visualization to engage our visitors. The main objective was to provide a creative and visual approach to make temporal data on app usage habits more attractive and understandable. Another project that inspired us and deserves mention is that of our colleagues, Lyon 1 students Anthony Bardou, Hugo Polloli, Tristan Syrzisko, and Théo Rabut: [Visualization Project](https://abardou.github.io/viz-habits/#/visualisation). The data on which the visualizations were created is similar to ours (mobile app usage data). We found this very interesting and it encouraged us to stick to our idea and continue working with this data to create a project worthy of these two works.

The visualization highlights different types of applications, represented by distinct bubbles. The animation of the visualization allows the user to observe how the usage of applications evolves over time. This provides a dynamic perspective on how certain applications become more frequently used at specific times of the day and how overall habits change over time, displayed on the clock to the left of the bubble chart. There is also a small image above the clock that simplifies the user's view based on the time of day (morning, evening, night), offering a more user-friendly experience. Three buttons (Fast, Stop, and Normal) indicate options to control the animation speed and stop it to get a better view of the clusters if necessary. This creative approach allows the user to better understand patterns and changes in the usage of applications over time. The use of animation facilitates the perception of temporal trends interactively.

### Second Visualization
The second visualization, complementary to the first, offers a heat map (inspired by tp 4) illustrating the rate of application usage over time. Unlike the bubble chart, it does not convey the temporal evolution of habits. It includes a slider that allows the user to explore the visualization interactively, offering a detailed view of temporal variations. This slider is also connected to a bar chart, making it easy to detect usage peaks throughout the day. With this feature, the user can quickly identify moments when certain apps are most used. By adjusting the slider, the user can visually compare app usage at different times of the day. These two visualizations have highlighted interesting patterns, such as the fact that from 7 a.m. to 9 a.m., the data owner tends to primarily use Instagram (probably upon waking up), then uses the phone to make calls from 9:30 a.m. to 10:30 a.m., and also during the lunch break (1 p.m. to 2 p.m.). But the most interesting patterns are observed at night, especially from 9 p.m. The user tends to use Instagram, WhatsApp, and the phone to make calls. This seems logical as, at this time, people usually tend to rest after a long day of work and scroll through social media or call family and friends.

### Third Visualization
Regarding the third visualization, it focuses on a comparative analysis of application usage during the week versus the weekend. A bar chart was developed to illustrate the daily usage of each application, clearly distinguishing weekdays from weekends. A pie chart accompanies the bar chart to compare the average usage time during weekdays and weekends. This visualization reveals that although the average usage times are similar (~300 min) during a weekday and a weekend day, application preferences differ. On weekdays, users prefer applications that can be interrupted at any time (like Instagram, WhatsApp, YouTube), while the weekend, with more available time, is marked by the use of applications requiring a longer duration, such as games or watching movies on platforms like Disney Plus.

### Fourth Visualization
Finally, as the last visualization, we created a line chart. This visualization provides an overall view of the duration of application usage over a period of 7 months. Some relevant observations have been identified from this data. Instagram is the most used application throughout the period, followed in the ranking by WhatsApp, YouTube, and phone calls. An interesting pattern appears with the use of gaming applications, which peaks during the months of May and June, followed by a break until September, then a return to these applications. This can be attributed to the summer holidays where people prefer to enjoy the good weather and family rather than playing games. On the other hand, applications like Goodreads or food delivery apps do not generate much interest from the user. The visualization is complemented by interactive features, including highlighting lines when hovering, allowing a more detailed exploration of usage patterns.

## Work Organization
Living close to each other and having done all our projects together, my teammate and I had the opportunity to mostly work in-person, even during school holidays. This allowed us to discuss and implement our ideas in real-time. When new ideas emerged, we discussed them directly or used Discord in the few instances where we were not in the same place for asynchronous communication. Each time a team member had a new idea, we discussed it together, and it was integrated into the project as it developed. This approach facilitated effective collaboration and smooth communication throughout the process of creating our project, saving us a lot of time.
## Visualizations
Our visualizations were created in JavaScript using primarily the D3 library.

### First Visualization
The first visualization is a bubble chart designed to illustrate the temporal evolution of mobile application usage habits. The idea of creating this bubble chart originated after discovering a visualization by Mr. Nathan YAU: [A Day in the Life of Americans](https://flowingdata.com/2015/12/15/a-day-in-the-life-of-americans/). This caught our attention, and we decided to create a similar visualization to engage our visitors. The main objective was to provide a creative and visual approach to make temporal data on app usage habits more attractive and understandable. Another project that inspired us and deserves mention is that of our colleagues, Lyon 1 students Anthony Bardou, Hugo Polloli, Tristan Syrzisko, and Théo Rabut: [Visualization Project](https://abardou.github.io/viz-habits/#/visualisation). The data on which the visualizations were created is similar to ours (mobile app usage data). We found this very interesting and it encouraged us to stick to our idea and continue working with this data to create a project worthy of these two works.

The visualization highlights different types of applications, represented by distinct bubbles. The animation of the visualization allows the user to observe how the usage of applications evolves over time. This provides a dynamic perspective on how certain applications become more frequently used at specific times of the day and how overall habits change over time, displayed on the clock to the left of the bubble chart. There is also a small image above the clock that simplifies the user's view based on the time of day (morning, evening, night), offering a more user-friendly experience. Three buttons (Fast, Stop, and Normal) indicate options to control the animation speed and stop it to get a better view of the clusters if necessary. This creative approach allows the user to better understand patterns and changes in the usage of applications over time. The use of animation facilitates the perception of temporal trends interactively.

### Second Visualization
The second visualization, complementary to the first, offers a heat map (inspired by tp 4) illustrating the rate of application usage over time. Unlike the bubble chart, it does not convey the temporal evolution of habits. It includes a slider that allows the user to explore the visualization interactively, offering a detailed view of temporal variations. This slider is also connected to a bar chart, making it easy to detect usage peaks throughout the day. With this feature, the user can quickly identify moments when certain apps are most used. By adjusting the slider, the user can visually compare app usage at different times of the day. These two visualizations have highlighted interesting patterns, such as the fact that from 7 a.m. to 9 a.m., the data owner tends to primarily use Instagram (probably upon waking up), then uses the phone to make calls from 9:30 a.m. to 10:30 a.m., and also during the lunch break (1 p.m. to 2 p.m.). But the most interesting patterns are observed at night, especially from 9 p.m. The user tends to use Instagram, WhatsApp, and the phone to make calls. This seems logical as, at this time, people usually tend to rest after a long day of work and scroll through social media or call family and friends.

### Third Visualization
Regarding the third visualization, it focuses on a comparative analysis of application usage during the week versus the weekend. A bar chart was developed to illustrate the daily usage of each application, clearly distinguishing weekdays from weekends. A pie chart accompanies the bar chart to compare the average usage time during weekdays and weekends. This visualization reveals that although the average usage times are similar (~300 min) during a weekday and a weekend day, application preferences differ. On weekdays, users prefer applications that can be interrupted at any time (like Instagram, WhatsApp, YouTube), while the weekend, with more available time, is marked by the use of applications requiring a longer duration, such as games or watching movies on platforms like Disney Plus.

### Fourth Visualization
Finally, as the last visualization, we created a line chart. This visualization provides an overall view of the duration of application usage over a period of 7 months. Some relevant observations have been identified from this data. Instagram is the most used application throughout the period, followed in the ranking by WhatsApp, YouTube, and phone calls. An interesting pattern appears with the use of gaming applications, which peaks during the months of May and June, followed by a break until September, then a return to these applications. This can be attributed to the summer holidays where people prefer to enjoy the good weather and family rather than playing games. On the other hand, applications like Goodreads or food delivery apps do not generate much interest from the user. The visualization is complemented by interactive features, including highlighting lines when hovering, allowing a more detailed exploration of usage patterns.

## Work Organization
Living close to each other and having done all our projects together, my teammate and I had the opportunity to mostly work in-person, even during school holidays. This allowed us to discuss and implement our ideas in real-time. When new ideas emerged, we discussed them directly or used Discord in the few instances where we were not in the same place for asynchronous communication. Each time a team member had a new idea, we discussed it together, and it was integrated into the project as it developed. This approach facilitated effective collaboration and smooth communication throughout the process of creating our project, saving us a lot of time.

## Esquisses
![Première Esquisse](image/image1.jpg)
![Deuxième Esquisse](image/image2.jpg)
![Troisième Esquisse](image/image3.jpg)
![Quatrième Esquisse](image/image4.jpg)
![Dernière Esquisse](image/image5.jpg)