# “RePsyched” — recycling made easy

Sorting trash can be a complicated process in Berlin — especially for those who are new to the city. Even if you’ve figured out the color-coded recycling bin system in your backyard, items like batteries, textiles or electronics will require you to visit specific locations around the city in order to dispose of them the proper, environmentally-conscious way.

RePsyched is your comprehensive guide to recycling in Berlin. It’s an interactive platform where users can search for items and materials they want to dispose of and easily retrieve information on the appropriate waste bin, recycling yard, or donation point — with the location nearest to the user marked on a map. The RePsyched prototype was implemented by a team of eight techies, leveraging our newly gained skills in UX Design, Data Science and Web Development as part of the TechLabs Berlin Digital Shaper Program. After an ideation session with the team and our TechLabs mentor to align on the goal of the project and to define its scope, we dived into building our MVP.

## UX Design

The three UX team members started with mapping out the user flow within the platform. This was then fine-tuned to include four web pages according to feedback from our potential users — in the first instance our team. We later expanded our research to include a larger pool of participants. We sent out an online survey of 10 questions to help us understand our potential users better. After gathering data on people’s current recycling habits, what frustrates them about separating trash, and what they would expect from our platform, we created personas, user stories and storyboards.

Based on user stories we designed the basic wireframe of each page in Figma. Ease of usability was a main focus of our website, therefore we focused on designing a simple interface with intuitive navigation in mind. We created three variations of the wireframe, with the intention to give options to the rest of the team, although there were no big differences. One of the wireframes was taken as the foundation to build a higher fidelity one, integrating colors, iconography, typography and logo. We created three prototype designs and after some discussion, we agreed to combine these into a final prototype to hand off to the web developers.

![Image of final prototype](https://raw.githubusercontent.com/louisa0206/RePsyched/main/Blog%20image%2001.png) The Figma prototype

## Data Science

The first challenge for the Data Science team was evaluating what data would be important for our product. After consultation, within the Data Science team and the other RePsyched members, we came to the conclusion that the location of recycling centers, glass containers and information about the different categories of waste disposal are most relevant for the RePsyched website. 

As a next step we divided up the chosen categories among the three of us and started searching and evaluating websites that contain the information we were looking for. 
Evaluating criteria were not only the completeness and correctness of information but also the way it was presented on the website and the ability to run a web scraper on it.

Web scraping basically means extracting data from human-readable output. For building the web scraper we used the Beautifulsoup and scrapy. We then discussed with the Web Developers in what format we store our information we scraped from the websites. We agreed on CSV files. The next step for us was cleaning and processing the data. As a last step we handed the data over to the WebDev team.

![Image of the pipeline that processes the scraped data](https://raw.githubusercontent.com/louisa0206/RePsyched/main/Blog%20image%2002.png) The pipeline that processes the scraped data

![Image of the result of the data scrape](https://raw.githubusercontent.com/louisa0206/RePsyched/main/Blog%20image%2003.png) The result


## Web Development

For us, the WebDev team, RePsyched was a great first hands-on experience, as we had no prior web development knowledge. Through the online course we already had a good fundamental understanding of HTML, CSS, JavaScript and React, but now it was time to put the recently gained theoretical skills into practice. 

We started with a very simple structure consisting of two HTML and CSS files to test the feasibility of our code.  Once the final prototype variant was selected, we divided the pages and modified our existing code by adding images, navigation bars, information paragraphs, etc. to match the template.
 
At this point, our website was visually realized but not yet functional. Therefore, we chose to build our website using React. Although we had already started the React project, we decided to add functionality through simple JavaScript, due to some technical difficulties in installing the necessary dependencies and inconsistencies of versions. Once we received the data from the Data Science team, we added the functional map and the search bar with autocompletion and made the entire website more user-friendly.

During the project phase, we were constantly in contact with the whole team and our mentor, to evaluate our progress and to ask for their suggestions for changes and improvements.

![Image of the green bins on the map](https://raw.githubusercontent.com/louisa0206/RePsyched/main/Blog%20image%2004.png) Green bins marked on the map

## Project Results

Under the time constraints of the program, we implemented a preliminary website that loads in recycling information for parts of Berlin. In the future, this could be expanded to cover the entire city. Features we brainstormed at the start of the project could be implemented as well, including a mobile version of the site and photo recognition capabilities so users can take a photo of an item they want to recycle and receive relevant recycling information.

**GitHub:**
https://github.com/louisa0206/RePsyched

**The Team:**
Agnes Emri — UX
Anna von Blohn — DS
Fariz Hakim — UX
Gwendolyn Grüntuch — WD
Irena Yeung — UX
Louisa Henschke — DS
Muhammad Ahsan Qayyum — WD
Zafar Iqbal — DS

**Mentor:**
Nils Strassenburg


