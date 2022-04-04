# TimelineJS Workshop Plan
## Learning Outcomes
* Introduce timelines as a way to visualize data in a linear, sequential fashion 
* Identify TimelineJS components and prepare a sample timeline 
* Define best practices for timeline creation and maintenance 

## Part 1: What is a timeline?
> “I am a Tralfamadorian, seeing all time as you might see a stretch of the Rocky Mountains. All time is all time. It does not change. It does not lend itself to warnings or explanations. It simply is. Take it moment by moment, and you will find that we are all, as I’ve said before, bugs in amber.” – Kurt Vonnegut, Slaughterhouse-Five

**Question: Who has made a timeline, either analog or digital?**

Timeline definition: Timelines, both analog and visual, are a form of data visualization using data that have a temporal component. We are taking pieces of data (dates, times, images, text) and presenting them in an interesting way to tell a story or make an argument. Digital timelines have the advantage of being interactive, so you can embed interactive media, link to other materials, and edit them to add new events, or correct errors.

*Review [Examples of analog timelines](http://archive.nytimes.com/www.nytimes.com/slideshow/2010/04/15/books/20100415-timelines-ss_index.html) from Cartographies of Time:  A History of the Timeline by Anthony Grafton and Daniel Rosenberg*

**Question: Why use a timeline?**
* Visualize data that are linear, progressive, and sequential 
* Provide historical context to events (in other words, place them in their point in history) 
* The main goal of a timeline is to help people understand temporal relationships quickly

**Question: When should you not use a timeline?**
* The events in time you are trying to visualize are non-linear in nature 
* Your focus is on a very specific point in time (so not much movement) 
* There’s no need to contextualize an event in the greater spacetime-continuum

**Question: How does a timeline reflect dominant views of how we experience time?**

Time is the “fourth dimension” but it is an element of our experience that we cannot change our place in. We can easily move in space (the other 3 dimensions) with enough will and force. However, we cannot move through time, other than the inevitable march forward. However, how we perceive time is very much on the personal experience of each person. There are additional challenges with how we move through time, especially as we approach the speed of light, but we will assume that we aren't doing that at the moment.

Our brain encodes new experiences, but not familiar ones, into memory, and our retrospective judgment of time is based on how many new memories we create over a certain period. In other words, the more new memories we build on a weekend getaway, the longer that trip will seem in hindsight. [Why does time seem to speed up with age?](https://www.scientificamerican.com/article/why-does-time-seem-to-speed-up-with-age/)

Most digital timelines and other similar tools use ISO standard date/time formats, which is based on a predominantly white, Euro-American conception of time. This doesn't mean standards are bad! But the idea that time is a left-to-right, top-to-bottom, linear progression reflects how we read, as well as how we perceive time. Think of the debate around Daylight Savings Time each year, and how we are willing to change how we perceive time because of how it conveniences/inconveniences us.  Time zones, meant to standardize time across countries based on longitudinal distance from Greenwich, England (another arbritrary choice) don't line up either (see [Asia Time Zones](https://www.timetemperature.com/asia/asia_time_zones.shtml)).

### Timeline Examples and Review
Divide the workshop into X groups of X participants each. Each group reviews a timeline and briefly reports out after 5 minutes of analysis.
* Group 1: [The Untold Story](https://cdn.knightlab.com/libs/timeline3/latest/embed/index.html?source=1tC5YnvokPvGWkwkxcyGeA9igftNws1Q0NkN47-VcGxQ&font=Default&lang=en&initial_zoom=2&height=700)
* Group 2: [A Brief Introduction to Animal Liberation and Veganism](https://cdn.knightlab.com/libs/timeline3/latest/embed/index.html?source=1qLFux0t3qLaXk4H5K9cdSy-ZGdsxaOpqFnv4het3RXM&font=Default&lang=en&initial_zoom=2&height=650)
* Group 3: [Lilith Through the Ages](https://cdn.knightlab.com/libs/timeline3/latest/embed/index.html?source=15FgHpGsOUn46JbZFgi5VpElTpzKWwcHxyr1-sPGCGho&font=Default&lang=en&initial_zoom=2&height=650)
* Group 4: [Children in Pittsburgh](https://cdn.knightlab.com/libs/timeline3/latest/embed/index.html?source=1kXV3p1ARuZLpoq5LUj_Gsro78gCVAKYNGdX9cIlgsN4&font=Default&lang=en&initial_zoom=2&height=650)

*Review the responses with the workshop participants, and allow them to navigate through the timeline themselves if technology/time allows)

#### Questions to Answer
* What is the goal/theme of the timeline? 
* What kinds of data/events are portrayed? 
* Is this an effective use of a timeline? Do you understand the progression of events, see how each event fits into the larger narrative, does the timeline tell a story? 

## Part 2: Elements of a TimelineJS Timeline
[TimelineJS](http://timeline.knightlab.com/) was created by the [Knight Lab](https://knightlab.northwestern.edu/), part of Northwestern University, as a way to provide journalists a quick and easy way to build an interactive timeline that could be included with online news stories. It requires no programming or coding knowledge, although if you know HTML and CSS you can use those languages to add additional features to your timeline, such as links and different styles. 

TimelineJS uses Google Sheets to create timelines. One way to do this is to copy the [TimelineJS Google Sheet template](https://docs.google.com/spreadsheets/d/1pHBvXN7nmGkiG8uQSUB82eNlnL8xHu6kydzH_-eguHQ/copy) from the TimelineJS website, fill it out, publish it to the web, and then copy and paste the link to the Sheet into their timeline creation tool. 

[Example Google Sheet](https://docs.google.com/spreadsheets/d/e/2PACX-1vTqQ6jAd56IZcis1yZ2tFC0QZxL851FUsmO6D2sAeQK9LqDhhAOJKamKC_S9ip3jWm7_vfyGBdD7rFW/pubhtml)

From the example, each ROW on the timeline is an event. Each COLUMN corresponds to a different element that is part of the event. 

While most users just directly input their data into the Sheet, you can also use a Google Form to populate a Google Sheet, which is what we are doing today to introduce you to the process. To start, we will go to our Google Form and you will create an event using the fields in the form. Then we will later look at it in the Google Sheet directly. This should give you a better understanding of how the different columns in the timeline are displaying their data.

### TimelineJS Display Elements
A TimelineJS timeline can roughly be broken into two parts, the **events**, and the **timeline**.
#### Events
Every TimelineJS timeline is made up of events, which have two parts: the media on the left, and the event text on the right. Either are optional - you can have only media, or only text. Events can use HTML and CSS to style text, create links, and do advanced things like create blockquotes, embed iFrames, etc.  
##### Title Slide
The title slide is the first "event" you see, if you create one. It shows up before any of the events, and acts as an introduction to the timeline. It's optional.
##### Event Text
Event text is broken up into three elements - the Display Date, the Headline, and the Text. 
###### Display Date
The Display Date, by default is the date (or range of dates) for the event. You can override this to display custom text (such as circa) in order to show some "fuzziness" to the date.
###### Headline
The Headline should briefly introduce the topic/information on the event.
###### Text
The text should give additional information about the event itself. There's not a lot of real estate to work with here - think about 50-75 words. However, if your event needs more content, you can always use HTML to create a link to another webpage.
##### Media
Generally, you use links to media that already exist on the Internet as media on an event. TimelineJS allows for a wide variety of media to be used. In addition to images and videos, you can also embed Tweets, Google Maps, Soundcloud and Spotify audio, Wikipedia articles, another TimelineJS timeline ... really just about anything that is already on the Internet. Since you are linking to media that is already on the Internet, and not necessarily downloading it and uploading it to the timeline, there is a bit less to think about when it comes to copyright issues. However, if you are going to download images from the Internet and then store them elsewhere, such as on your own website, or on Google Drive, etc., it is usually best to look for [media files that are in the public domain, or have a license applied to them that allows them to be used freely](https://dh.sites.gettysburg.edu/toolkit/media/finding-images/).

One thing to note is that links to images should generally end with an image file format (such as .jpg, .png, .gif) - although images on Flickr don't require this.
###### Caption
Below the media, there is a space for a caption to give your media some additional context as to what it is, and why it is there. There isn't a lot of space here, so you need to be to the point. 
###### Credit
There is also a space to add a credit for the media. A best practice for media credits is to use the [TASL (Title, Author, Source, License) method of attribution](https://dh.sites.gettysburg.edu/toolkit/media/attribution/). Some media formats will automatically create citations, such as YouTube or Flickr. 
##### Background
By default, the background of an event is white. However, you can use the background color element of the event to turn the background a different color using [hex codes](https://www.w3schools.com/colors/colors_picker.asp). Hex codes are alphanumeric codes that start with a hash sign and have 6 numbers and/or letters. This can become an accessiblily issue, however, if you use a color without enough contrast for the text. Another option is to use a link to an image to create a background image for the event. Background colors can be a good way to "categorize" different slides - such as all events of one type with a white background, events of another type with a blue background, etc. 
#### Timeline
At the bottom, all of your events are part of the overall timeline, which you can zoom in and out on.
##### Groups
You can create groups of events, by giving them the same group name in the Google Sheet. This creates a "sandwich" effect in the timeline, where each event is on the layer that corresponds with its group. Generally 3-4 groups is the most you should consider having.
##### Eras
Eras create blocks of color that can differentiate different eras of time. These are created by having an event that has a start and and end date, and the event type is defined as an era. 
### Other Options
When you create your TimelineJS timeline, there are additional options you can set, such as the fonts for the text, if you want the timeline on the top or bottom, if you want to start from the end of the timeline, etc. 

## Best Practices, and Common Issues
### Common Issues
* Broken image: this may mean the link isn't a link to an image (Wikimedia Commons photos are a big offender), the link has been taken down, or the link is configured in such a way that it doesn't allow it to be hotlinked to display on another website
* Error fetching sheets data: the Google Sheet isn't published
* Weird stuff started showing up: the Google Sheet may be set to be allowed to be edited by anyone, which isn't a good idea. If you are using it to create a collaborative timeline, then either invite users to edit it with a Google login, or change the access to view only when collaborative editing isn't needed anymore. 
* Scroll bars appear with text: it's probably too much text, revise and resubmit.
* Timeline doesn't update after making a change to Google Sheets: sometimes this takes a few minutes, be patient!
* Other weirdness: sometimes a blank row will cause problems, or more than one title slide, or an era event without both start and end dates
### Best Practices
Based off of what you have seen so far, both in the examples, and also what you have worked with today, let’s think of some best practices we can agree on. 

*Whiteboard best practices – break up into different categories at first* 

* Presentation/Aesthetics 
* Narrative/Story 
* Usability 

**Additional best practices**
* Have an argument! The timeline should have a theme and an argument it is trying to make.
* Events should reinforce each other. You are telling a story with the timeline, so it should be clear why each event is on the timeline. Each event should be a part of the larger narrative. Large gaps in time on your timeline may cause your users to question what happened in the interim. 
* Be clear and concise! Link out to other webpages instead of trying to put too much information on a single event. Your vent headline should reinforce the content and draw in users to read more. 
* Keep data in multiple places – in case the Google Sheet has a glitch, or if something gets accidentally erased, you want to make sure your data isn’t only living in one place. 
* Pick media that reinforce the event and your text. Always include a caption that provides some additional context for your image, and a credit to the original. Never assume that your users will see your picture and know what it is. Giving credit back to the original creator is the ethical thing to do. 
* Crediting media 
  * At the very least, you should include: 
    * The title of the media 
    * The creator of the media (author) 
    * A link back to where it was found originally 
  * Don’t worry about things like trying to do indents or italics, this isn’t citation, it is attribution.

## Final Questions to Ponder
* How do you think you might use TimelineJS for a classroom activity, assignment/project, and/or your own research?
* What do you feel comfortable doing on your own, or what things would you need additional support for (either synchronously, such as a training session, or asynchronously, such as video tutorials)?
* How would you grade/assess a timeline that you might use as part of an assignment? What rubrics/specifications would you give students to consider as they build their own timelines?
