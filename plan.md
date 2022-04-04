# TimelineJS Lesson Plan
## Learning Outcomes
* Introduce timelines as a way to visualize data in a linear, sequential fashion 
* Identify TimelineJS components and prepare a sample timeline 
* Define best practices for timeline creation and maintenance 

## Part 1: What is a timeline?
> “I am a Tralfamadorian, seeing all time as you might see a stretch of the Rocky Mountains. All time is all time. It does not change. It does not lend itself to warnings or explanations. It simply is. Take it moment by moment, and you will find that we are all, as I’ve said before, bugs in amber.” – Kurt Vonnegut, Slaughterhouse-Five

**Question: Who has made a timeline, either analog or digital?**

Timeline definition: Timelines, both analog and visual, are a form of data visualization using data that have a temporal component. We are taking pieces of data (dates, times, images, text) and presenting them in an interesting way to tell a story or make an argument. Digital timelines have the advantage of being interactive, so you can embed interactive media, link to other materials, and edit them to add new events, or correct errors.

[Examples of analog timelines](http://archive.nytimes.com/www.nytimes.com/slideshow/2010/04/15/books/20100415-timelines-ss_index.html) from *Cartographies of Time:  A History of the Timeline* by Anthony Grafton and Daniel Rosenberg

**Question: Why use a timeline?**
* Visualize data that are linear, progressive, and sequential 
* Provide historical context to events (in other words, place them in their point in history) 
* The main goal of a timeline is to help people understand temporal relationships quickly

**Question: When should you not use a timeline?**
* The events in time you are trying to visualize are non-linear in nature 
* Your focus is on a very specific point in time (so not much movement) 
* There’s no need to contextualize an event in the greater spacetime-continuum

**Question: How does a timeline reflect dominant views of how we experience time?**

Time is the “fourth dimension” but it is an element of our experience that we cannot change our place in. We can easily move in space (the other 3 dimensions) with enough will and force. However, we cannot move through time, other than the inevitable march forward. However, how we perceive time is very much on the personal experience of each person.

Our brain encodes new experiences, but not familiar ones, into memory, and our retrospective judgment of time is based on how many new memories we create over a certain period. In other words, the more new memories we build on a weekend getaway, the longer that trip will seem in hindsight. [Why does time seem to speed up with age?](https://www.scientificamerican.com/article/why-does-time-seem-to-speed-up-with-age/)

Most timelines and other similar tools use ISO standard date/time formats, which is based on a predominantly white, Euro-American conception of time. This doesn't mean standards are bad! But the idea that time is a left-to-right, top-to-bottom, linear progression reflects how we read, as well as how we perceive time. Think of the debate around Daylight Savings Time each year, and how we are willing to change how we perceive time because of how it conveniences/inconveniences us.  Time zones, meant to standardize time across countries based on longitudinal distance from Greenwich, England (another arbritrary choice) don't line up either (see [Asia Time Zones](https://www.timetemperature.com/asia/asia_time_zones.shtml)).

### Timeline Examples and Review
Divide the workshop into X groups of X participants each. Each group reviews a timeline and briefly reports out after 5 minutes of analysis.
* Group 1: [The Untold Story](https://cdn.knightlab.com/libs/timeline3/latest/embed/index.html?source=1tC5YnvokPvGWkwkxcyGeA9igftNws1Q0NkN47-VcGxQ&font=Default&lang=en&initial_zoom=2&height=700)
* Group 2: [A Brief Introduction to Animal Liberation and Veganism](https://cdn.knightlab.com/libs/timeline3/latest/embed/index.html?source=1qLFux0t3qLaXk4H5K9cdSy-ZGdsxaOpqFnv4het3RXM&font=Default&lang=en&initial_zoom=2&height=650)
* Group 3: [Lilith Through the Ages](https://cdn.knightlab.com/libs/timeline3/latest/embed/index.html?source=15FgHpGsOUn46JbZFgi5VpElTpzKWwcHxyr1-sPGCGho&font=Default&lang=en&initial_zoom=2&height=650)
* Group 4: [Children in Pittsburgh](https://cdn.knightlab.com/libs/timeline3/latest/embed/index.html?source=1kXV3p1ARuZLpoq5LUj_Gsro78gCVAKYNGdX9cIlgsN4&font=Default&lang=en&initial_zoom=2&height=650)

#### Questions to Answer
* What is the goal/theme of the timeline? 
* What kinds of data/events are portrayed? 
* Is this an effective use of a timeline? Do you understand the progression of events, see how each event fits into the larger narrative, does the timeline tell a story? 

## Part 2: Building a TimelineJS Timeline
TimelineJS was created by the Knight Lab, part of Northwestern University, as a way to provide journalists a quick and easy way to build an interactive timeline that could be included with online news stories. It requires no programming or coding knowledge, although if you know HTML and CSS you can use those languages to add additional features to your timeline, such as links and different styles. 

TimelineJS uses Google Sheets to create timelines. One way to do this is to copy the TimelineJS Google Sheet template from the TimelineJS website, fill it out, and then copy and paste the link to the Sheet into their timeline creation tool. 

[Example Google Sheet](https://docs.google.com/spreadsheets/d/e/2PACX-1vTqQ6jAd56IZcis1yZ2tFC0QZxL851FUsmO6D2sAeQK9LqDhhAOJKamKC_S9ip3jWm7_vfyGBdD7rFW/pubhtml)

Each ROW on the timeline is an event. Each COLUMN corresponds to a different element that is part of the event. 

While many users just directly input their data into the Sheet, you can also use a Google Form to populate a Google Sheet, which is what we are doing today to introduce you to the process. 

To start, we will go to our Google Form and you will create an event using the fields in the form. Then we will later look at it in the Google Sheet directly. This should give you a better understanding of how the different columns in the timeline are displaying their data. 

We have a sandbox form that we will use for this class session. After this class session, you can continue to use this sandbox form and Google Sheet to play around and try things. When it’s time to create your specific portion of the timeline for your assignment, you will have a separate form for each group. After you’ve done your events, then we will stitch all the spreadsheets together to make the final larger timeline. 

### Finding Media 

TimelineJS allows for a wide variety of media to be used. In addition to images and videos, you can also embed Tweets, maps, Soundcloud and Spotify audio, Wikipedia articles … really just about anything. Since you are linking to media, and not necessarily downloading it and uploading it to the timeline, there is a bit less to think about when it comes to copyright issues. However, it is usually best to look for media files that are in the public domain, or have a license applied to them that allows them to be used freely.
