| [home page](https://zoya2130.github.io/dataviz-portfolio/) | [data viz examples](dataviz-examples) | [critique by design](critique-by-design) | [final project I](final-project-part-one) | [final project II](final-project-part-two) | [final project III](final-project-part-three) |

# Final Project, Part 2: Wireframes, Storyboards, and User Research

Zoe Wang | 94-870 Telling Stories with Data | Carnegie Mellon University

**On this page:** [1. Wireframes and storyboards](#1-wireframes-and-storyboards) | [2. User research](#2-user-research) | [References](#references) | [AI acknowledgements](#ai-acknowledgements)

---

## 1. Wireframes and storyboards

My draft story is built in Shorthand. It is called **Who Pays for the Show?** You can read it here:

**[Who Pays for the Show? (draft Shorthand story)](https://carnegiemellon.shorthandstories.com/who-pays-for-the-show/index.html)**

I used the outline and sketches from [Part 1](final-project-part-one) as my guide. The draft Shorthand story works as my storyboard. Each screen has the text for that part of the story. The charts are made in Tableau and embedded in the story.

### Storyboard

| Screen | Section in the story | What the reader sees | Chart | Main message |
|--------|----------------------|----------------------|-------|--------------|
| 1 | Opening | Title, photo, and a short question: who pays for live performance in Pittsburgh? | None | This story follows the income of seven leading arts groups, from 2019 to today. |
| 2 | March 2020 | Short text with national and local numbers about the shutdown and relief money | None | The shows stopped. Who paid the bills? |
| 3 | Who are the seven? | Short profile of the seven groups, then the first chart | Stacked bar chart of income structure in 2019 for each group. Other income is grey. | Before the pandemic, the groups did not look the same. Donations paid for 42% to 70% of revenue. |
| 4 | Donors carried the load (2020 to 2021) | One chart and a short note about relief funds | Line chart of donations as a share of revenue. The years 2019 to 2021 are blue. Other years are grey. | In 2021, donations paid for 69% to 97% of revenue. |
| 5 | 2022: Three groups had their biggest year | One chart and two examples | Small charts of total revenue for each group, FY2017 to FY2025 | Opera, Ballet, and Quantum Theatre had their highest revenue in 2022. |
| 6 | Now: No single recovery story | Text with the numbers for each group, then the charts for the latest year | Charts of income structure in the latest year, and donation share in 2019 compared with the latest year | Two groups rely more on donations, three rely less, and two are about the same. |
| 7 | What this means | Three short messages: for donors, for board members, and for audience members | None | A mix of income that depends on one source is a risk in a crisis. |
| 8 | Data and method | Data source, method, sources, and credits | None | Readers can check where the numbers came from. |

### Design choices in the charts

- I show each income source as a share of total revenue. This lets a small group and a large group sit side by side.
- Grey is used for "Other" income, so the three main sources stand out.
- On the donation chart, 2019 to 2021 is blue and the other years are grey. This points the reader to the pandemic years.
- Each chart has a short heading and a caption. The data source and method are explained in the Data and method section of the story.

---

## 2. User research

### Research goal and questions

**Goal of the research.** I want to learn whether readers understand my story, whether the charts are easy to read, and whether the screen order makes sense.

**Research questions**

1. Can readers understand the main message?
2. Which charts are easy to read, and which charts are confusing?
3. Is the story order clear?

### a. Target audience

My main audience is people who enjoy live performances and may support local arts groups. They love the arts, but they usually don't read financial reports. My second audience is people who work or study in the arts. They want to understand how arts groups depend on different income sources.

### b. How I chose people to interview

I will interview three people I know personally. I chose them to be different from each other:

1. One person who often goes to live performances.
2. One person who studies in arts management.
3. One person who has design experience.

### c. Interview script

Each interview takes about 10 minutes.

**Warm up**

- How comfortable are you with charts and numbers, from 1 to 5?

**Reading the story**

- Please read the story from the top. I will not explain anything while you read.

**After reading**

- In your own words, what is this story about?
- Which chart was easiest to understand? Which was hardest?
- If you could change only one thing, what would it be?

### d. Interview findings

I removed all names and personal details. The interviewees are described in general terms only. The interviews were in Chinese. I translated the quotes into English.

| Interviewee | Who they are | In your own words, what is this story about? | Which chart was easiest? Which was hardest? | If you could change only one thing, what would it be? |
|-------------|--------------|-----------------------------------------------|---------------------------------------------|--------------------------------------------------------|
| Friend A | Often goes to live performances | Understood the story. Said the design is "like data news." | Did not pick one easiest chart. Hardest: the 2022 revenue chart. It has "too many grey blocks" and feels crowded. This distracts from the message. The chart of 2019 compared with the latest year has a new form, but it "looks more like a comparison across groups than a change over time." Also, some charts did not open in one browser. | Change the white chart background. It "looks sudden" on the page. Also show only 2019 to 2022 in the revenue chart, and try a line chart for the 2019 and latest year comparison. |
| Friend B | Has design experience | Summarized it well: the story follows the tax filings of seven Pittsburgh performing arts groups from 2017 to 2025. It shows how their income was structured before the pandemic, during the shutdown, and today. When the shows stopped, donations kept the groups going. Since then their paths have been different, so there is "no single answer." | Easiest: the income structure chart. It is "very direct and effective." Hardest: the 2020 to 2021 line chart. "I did not understand it." | Make the chart background the same color as the web page. |
| Friend C | Studies arts management | Seven Pittsburgh arts groups, and how their income sources changed before and after the pandemic. Ticket income fell sharply and donations paid for most costs. After the pandemic, ticket income did not return to the old level. The story reminds arts groups not to depend on one source of income. | Easiest: the comparison of donation share before and after the pandemic. Hardest: the revenue chart that puts all groups and many years together. "Too much information is mixed together. I had to look for a long time." | Split the mixed revenue chart so each group is shown on its own. "Then it is clearer to read." |

**Where the interviewees agreed**

- All three understood the main message. Donations carried the groups when shows stopped, and each group recovered in a different way. Friend B said there is "no single answer." Friend C took away that groups should not depend on one source of income.
- Two interviewees (A and C) said the revenue chart for all groups across many years is too crowded.
- Two interviewees (A and B) said the white chart background looks out of place on the page.
- The income structure chart and the donation comparison before and after the pandemic were named as easy to read (B and C).

**Where the interviewees had different views**

- The chart of donation share in 2019 compared with the latest year. Friend C found it the easiest chart. Friend A liked the new form, but said it looks like a comparison across groups, not a change over time.
- Line charts. Friend A suggested a line chart for the 2019 and latest year comparison. Friend B found the 2020 to 2021 line chart the hardest. So a line chart is not always the clearer choice.
- How to fix the crowded revenue chart. Friend A wants fewer years (2019 to 2022). Friend C wants each group shown separately.
- Only Friend A said that some charts did not open. I had the same problem and needed to change browsers.

### e. Changes I plan to make in Part 3

| What I learned | Who said it | Change I plan to make |
|----------------|-------------|------------------------|
| The white chart background looks out of place | A, B | Change the background of all Tableau charts to match the Shorthand page color. |
| Some charts did not open in one browser | A (I saw it too) | Test the charts in Chrome, Safari, and Firefox. Add a link under each chart: "Open this chart in Tableau Public." |
| The 2022 revenue chart is crowded | A, C | Show only 2019 to 2022. Make each group chart larger. Color the three groups with record revenue in 2022, and make the other groups light grey. |
| The 2020 to 2021 line chart is hard to understand | B | Put each group name at the end of its line. Mark the 2021 values. Add one short sentence on how to read it: each line is one group, and a higher line means more reliance on donations. |
| The 2019 and latest year chart looks like a comparison across groups | A (C found it easiest) | Keep this chart type, because C understood it fast. Label both ends "2019" and "Latest year." Use color to show if a group went up or down. Test it again before I decide to use a line chart. |
| The main message was clear to all three readers | A, B, C | Keep the story order and the main text. Make only small edits. |

---

## References

- Story: [Who Pays for the Show?](https://carnegiemellon.shorthandstories.com/who-pays-for-the-show/index.html) (Shorthand)
- Data: IRS Form 990 filings of seven Pittsburgh arts groups, fiscal years 2017 to 2025, from [ProPublica Nonprofit Explorer](https://projects.propublica.org/nonprofits/). See [Part 1](final-project-part-one) for the full data description and the list of national and Pittsburgh sources.
- Charts: made in Tableau and embedded in Shorthand.

## AI acknowledgements

- **Microsoft Copilot:** I used it to collect the Form 990 data. I checked the numbers.
