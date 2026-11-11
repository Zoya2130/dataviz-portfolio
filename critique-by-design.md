| [home page](https://zoya2130.github.io/dataviz-portfolio/) | [data viz examples](dataviz-examples) | [critique by design](critique-by-design) | [final project I](final-project-part-one) | [final project II](final-project-part-two) | [final project III](final-project-part-three) |

# PISA 2025: Critique and Redesign (MakeoverMonday)

*Course: 94-870 Data Stories. Assignment: Critique and redesign (MakeoverMonday).*

## Step one: the visualization

**Original link:** [MakeoverMonday, PISA 2025](https://makeovermonday.vercel.app/dataset/pisa-2025)

**Source:** OECD, *Student performance in PISA 2025* (PISA 2025 Results, Volume I).

![The original chart](original%20question.webp)

*Original chart by the OECD. Shown here for critique and redesign.*

**Why I chose it.** I chose this chart because it comes from the OECD, a public source, and MakeoverMonday gives a data file for it. I also saw clear design problems that I could name and try to fix.

## Step two: the critique

I used Stephen Few's Data Visualization Effectiveness Profile. These are the main points from my form.

**What I noticed first.** Japan is at the top. Japan has the largest share of students at Level 3 and above. The countries are ordered from the highest result to the lowest. The OECD average is highlighted. The country names are easy to find on the left.

**What worked well**

- The countries are sorted, so the reader can find the highest and the lowest.
- The OECD average is highlighted.
- The country names are written next to the bars.
- A dropdown lets the reader switch between OECD countries and other groups.

**What did not work well**

- The chart shows the share of students at each level for every country. This is a lot of information, and the shades of blue are hard to tell apart.
- I was confused about what each level means. I also did not understand why 0% is in the middle of the axis. The chart does not explain this. The reason is in the text on the side. Level 3 is the point where students start to show solid skills and can make fast progress. It starts at 468 score points.
- There are no value labels.
- Only the segments next to the center line start from the same baseline. It is hard to compare the other segments between countries.
- The chart does not say how the countries are sorted.

**The audience.** The main readers are policymakers, school leaders, and people who work in education. The chart works for readers who already know PISA. It is less effective for a general reader like me. The chart shows many levels, and I cannot understand the idea right away. I need to read the text next to the chart to learn what the levels mean.

**The method.** Few's profile gave me seven clear questions, so I could name specific problems, such as the similar blue shades and the unexplained center line. But it judges a finished chart, and the scores are partly personal. The Good Charts method starts with the purpose of the chart, and then asks you to talk to people, sketch, and test. The tests showed problems that the profile did not show, such as readers not knowing what PISA and the OECD are. I think the two methods work well together.

## Step three: Sketch a solution

### The problem with the data

My redesign plan had three parts:

1. Write a new headline that states the main conclusion, and explain why Level 3 matters.
2. Show one number for each country: the share of students at Level 3 and above.
3. Highlight a few countries and the OECD average.

The MakeoverMonday data does not have the share of students at each level. It only has the mean score for each country. So I could not do the second part. I had to think about a new story. I decided to show which countries score above the OECD average. I added a note to explain Level 3. The note also says what the OECD reports: about two thirds of students in OECD countries reach Level 3 or above.

### What I tried in Tableau

I tried several chart types before I chose the final design.

- **A dot plot by region.** The orange dots for countries outside the OECD took too much attention. The vertical position only showed the region.
- **A dot plot with one row for each country.** The dots made a diagonal line. A reader could think it is a trend for one country.
- **A single row of dots.** The dots were crowded and hard to read.
- **A scatter plot of top performers and low performers.** It was interesting, but it measures a different thing from the original chart. It uses three subjects, not computational problem solving.
- **A map only.** A map is good for finding a country. But the highest scoring places, like Singapore, Macao, and Hong Kong, are very small and hard to see. Color alone cannot show how many points a country is above the average.
- **A bar chart only.** It shows the ranking clearly, but it has no sense of place.

So I combined a map and a bar chart. The map shows where. The bar chart shows how much.

### My first sketch

After these tries, I chose a map with a bar chart. This is my first sketch. I made it directly in Tableau as a digital draft, and I did not draw it on paper. The map has green circles that show the points above the average. I showed it in class.

<div class='tableauPlaceholder' id='viz1794372744425' style='position: relative'><noscript><a href='#'><img alt='Dashboard 1 ' src='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;PI&#47;PISA2025Zoedraft&#47;Dashboard1&#47;1_rss.png' style='border: none' /></a></noscript><object class='tableauViz'  style='display:none;'><param name='host_url' value='https%3A%2F%2Fpublic.tableau.com%2F' /> <param name='embed_code_version' value='3' /> <param name='site_root' value='' /><param name='name' value='PISA2025Zoedraft&#47;Dashboard1' /><param name='tabs' value='no' /><param name='toolbar' value='yes' /><param name='static_image' value='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;PI&#47;PISA2025Zoedraft&#47;Dashboard1&#47;1.png' /> <param name='animate_transition' value='yes' /><param name='display_static_image' value='yes' /><param name='display_spinner' value='yes' /><param name='display_overlay' value='yes' /><param name='display_count' value='yes' /><param name='language' value='en-US' /><param name='filter' value='publish=yes' /></object></div>

<script type='text/javascript'>                    var divElement = document.getElementById('viz1794372744425');                    var vizElement = divElement.getElementsByTagName('object')[0];                    if ( divElement.offsetWidth > 800 ) { vizElement.style.width='100%';vizElement.style.height=(divElement.offsetWidth*0.75)+'px';} else if ( divElement.offsetWidth > 500 ) { vizElement.style.width='100%';vizElement.style.height=(divElement.offsetWidth*0.75)+'px';} else { vizElement.style.width='100%';vizElement.style.height='727px';}                     var scriptElement = document.createElement('script');                    scriptElement.src = 'https://public.tableau.com/javascripts/api/viz_v1.js';                    vizElement.parentNode.insertBefore(scriptElement, vizElement);                </script>

## Step four: Test the solution

I talked to three classmates from my group.

- Person A: student, about 24 years old
- Person B: student, about 24 years old
- Person C: student, about 24 years old

**Feedback from class**

| What I heard | What I changed |
|---|---|
| The legend said "Above 500" and "At or below 500". People did not know what 500 means. A note does not fix this. | I changed the legend to "Above the OECD average" and "At or below the OECD average". |
| The circles on the map and the bar chart showed the same information. | I removed the circles. The bar chart now uses a blue gradient, from the most points above the average to the fewest. |
| People did not know what the test is or what the OECD is. This showed me that the title is hard for a general reader. | I wrote a new title and added a short note under it. The note explains PISA and the OECD. |
| Some people suggested a color gradient on the map, or zoomed maps for small places. | I did not make this change. See the next paragraph. |

**What I did not do, and why.** I agree with the idea. The highest scoring places are small, so a gradient on the map would not help the reader see them. A zoomed view of small places would help. With other tools, I could draw each place larger, like learning the shape of each state in a geography class. I could not do this in Tableau. It was too hard for me technically, and it would make the page too busy. So I chose a middle path. I kept two colors on the map and used the bar chart to show the amount.

**Patterns in the feedback.** People could read the colors quickly. They needed more context to understand the numbers and the names. I also saw this myself. The first thing I noticed on my map was the blue and yellow colors, not the three highest places. So the title now describes what the map shows first.

## Step five: build the solution

<div class='tableauPlaceholder' id='viz1794372875429' style='position: relative'><noscript><a href='#'><img alt='Dashboard 1 ' src='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;PI&#47;PISA2025Zoefinal&#47;Dashboard1&#47;1_rss.png' style='border: none' /></a></noscript><object class='tableauViz'  style='display:none;'><param name='host_url' value='https%3A%2F%2Fpublic.tableau.com%2F' /> <param name='embed_code_version' value='3' /> <param name='site_root' value='' /><param name='name' value='PISA2025Zoefinal&#47;Dashboard1' /><param name='tabs' value='no' /><param name='toolbar' value='yes' /><param name='static_image' value='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;PI&#47;PISA2025Zoefinal&#47;Dashboard1&#47;1.png' /> <param name='animate_transition' value='yes' /><param name='display_static_image' value='yes' /><param name='display_spinner' value='yes' /><param name='display_overlay' value='yes' /><param name='display_count' value='yes' /><param name='language' value='en-GB' /><param name='filter' value='publish=yes' /></object></div>

<script type='text/javascript'>                    var divElement = document.getElementById('viz1794372875429');                    var vizElement = divElement.getElementsByTagName('object')[0];                    if ( divElement.offsetWidth > 800 ) { vizElement.style.width='100%';vizElement.style.height=(divElement.offsetWidth*0.75)+'px';} else if ( divElement.offsetWidth > 500 ) { vizElement.style.width='100%';vizElement.style.height=(divElement.offsetWidth*0.75)+'px';} else { vizElement.style.width='100%';vizElement.style.height='727px';}                     var scriptElement = document.createElement('script');                    scriptElement.src = 'https://public.tableau.com/javascripts/api/viz_v1.js';                    vizElement.parentNode.insertBefore(scriptElement, vizElement);                </script>

### The story in this chart

About one third of the countries and regions in this data score above the OECD average. The OECD average is 500 points. In the data, 27 of 85 countries and regions are above it.

The six highest places are all in East and Southeast Asia. They are Macao (China), Singapore, B-S-J-Z (China), Japan, Chinese Taipei, and Hong Kong (China). Macao is the highest, with 572 points. Most of the other places above the average are in Europe. Australia, New Zealand, Canada, and the United States are also above it. In this data, every place in Latin America and in the Middle East and North Africa is below the average.

The OECD also reports that about two thirds of students in OECD countries reach Level 3 or above. My chart cannot show this, because my data only has average scores. I put it in the note instead.

### Limits of my version

The data only has mean scores, so it does not show the share of students at each level. Six countries and regions have no computational problem solving score. B-S-J-Z (China) means four Chinese provinces and cities, which are Beijing, Shanghai, Jiangsu, and Zhejiang, but on the map it is shown on all of China. Singapore, Hong Kong, and Macao are very small on a world map, so the bar chart lists them. The bar chart shows only the 27 countries and regions above the average.

## References

- **Data:** PISA2025.xlsx from MakeoverMonday (Week 44, 2026). It has mean scores for 85 countries and regions. The original source is the OECD.
- **OECD:** *PISA 2025 Results (Volume I)*, Student performance in PISA 2025.
- **MakeoverMonday:** https://makeovermonday.vercel.app/dataset/pisa-2025
- **Tools:** Tableau Desktop and Tableau Public. The map background is from Mapbox and OpenStreetMap.
- Stephen Few, "Data Visualization Effectiveness Profile," Perceptual Edge, 2017.
- Scott Berinato, *Good Charts*, Chapters 3 and 4.
- Fernanda Martin, "Design and Redesign in Data Visualization" (Medium).
- Evan Peck, "Data is Personal. What We Learned from 42 Interviews in Rural America" (Medium).
