# Managing risk

Everything you need to know about successfully executing a data journalism project can be found in [this video about bathroom renovations](https://www.youtube.com/watch?v=e_qc0IE3cTw).

## The goal

In my opinion, **an unfinished project is worse than no project at all.**

Yes, working through a project always teaches you skills. I have approximately one million unfinished, unpublished projects sitting on my computer that will never see the light of day. I'm sure I learned a lot with all of them, and I'm better off for having started them. *But every one of them is a terrible weight on my mind.*

One of the biggest problems with unfinished projects is they aren't *emotionally fulfilling*. Even if you learned a lot, these projects can feel like lost time, weighing you down with an odd form of productivity guilt. Did you *really* accomplish something during all those days/hours/weeks you spent on it? Whatever you can do to get it across the finish line – even if you don't like the final product – is going to feel better in the long run.

In a more practical sense, it's also easier to talk to someone about your skillsset when you can point to projects that used those skills. Even if you give sixteen qualifiers about how dissatisfied you are with a particular project, it's better than "I have a project where I worked on something like that, I just never published it..."

!!! example

    At the end of last semester I published the [pandas question factory](https://jsoma.github.io/pandas-question-factory/), a little tool that provides practice questions when doing data analysis with pandas. Even though I feel it has potential, *I hate it.*
    
    It has about ten thousand improvements that I think are mandatory before it ascends from being Complete Garbage, but I pushed it out anyway. I have no idea if I'll ever make those improvements, and it's at least functional!

### How to make things work

It's one thing when you're knee-deep in a project that isn't going well. Depending on your timeframe, you have a few options:

* Pivot, pivot, pivot, pivot, until you find a thread that's worth pursuing.
* Simplify, simplify, simplify until you have nine words and a bar chart.
* Quit. But let's take that off the table for now!

Everything else on this page is aimed at preventing you from ending up in one of those bad situations.

!!! tip "But what if in the end my project is garbage?"

    If it's a personal project, who honestly cares? Just publish the garbage. Something is better than nothing.
    
    Slap it on a web page, publish your github repo – [hot tips on that here](https://jonathansoma.com/fancy-github/) – and never think about it again. Don't highlight its existence, but *put it out there*.

### Risk, value, and reward

During the planning stages of your project, you have to ask yourself two questions:

* Do I have the time to get the job done?
* Do I have the ability to get the job done? 

The more complicated a project is, the longer it will take. The lower your skill level, the longer a project will take. If you pick a complicated project where you'll need to learn a lot along the way, **you need to budget a long, long time.**

On the other hand, sometimes a giant project is absolutely worth it. You'll learn skills that you can't pick up in a short period of time, or you'll win all of those journalism awards you've always had your eye on.

It's perfectly fine to head down that long road, *as long as you've made a plan and are aware of what's in store.* You don't want to charge head-first into a beautiful, rewarding project and realize you only have a fraction of the time you'll need to complete it.

## Planning ahead

There are a handful of things you can do to improve your chances of completing a quality project by the deadline and reducing stress along the way. Let's take a look at a few ideas that involve a tiny, tiny bit of planning ahead.

### Minimum viable story

At the start of a project it's useful to define a **minimum viable story** - the smallest, tiniest story that our work could produce. Yes, we'd love to make every project a shining, gorgeous, completely perfect piece of art. In reality, though, we have limited skills and limited time.

Our minimum viable story is without a doubt far more boring than we'd like it to be, with fewer interviews, less depth, and uninteresting graphics. But it helps keep us grounded, and if we hit a wall we can be comforted that there's still *something* we can produce, even if it isn't our best work.

To our editors it's a guarantee we'll have something to turn it at the deadline, and to us it's emotional insurance that unexpected issues aren't the end of the world.

### Risk analysis

At the start of a project, we can break it down into several stages and assign a risk level to each. Our scoring might look something like this:

|step|tools|new topics|risk|
|---|---|---|---|
|**Data collection**|Selenium, pandas|multi-page scraping|medium risk|
|**Analysis**|pandas|none|low risk|
|**Visualization**|DataWrapper|stacked charts, annotations|low risk|

After breaking it down, we can see that overall there isn't too much risk involved: it seems like a doable project. Even if our data collection takes longer than predicted, the rest of the project doesn't have many moving parts and will most likely go smoothly.

If we change our analysis stage to include text mining and our visualization to be based on D3, we might end up with two "high risk" rows! If our deadline is in two weeks, that's a signal to reevaluate our plan. If we have a couple months, though, we can use the extra time to cover for our still-growing skillset.

### Acknowledge your weaknesses

When you write a pitch, it's easy to ignore all of the gotchas and potential problems you might encounter down the line. Chances are you'll focus on what you're good at!

While focusing on your strengths is certainly *important* – especially for getting a pitch accepted – it isn't necessarily *helpful* when those problems rear their head. Instead, treat a pitch like a planning document: acknowledge that you might hit a stumbling block with a section of the project and show you plan for coping with them ahead of time.

For example, if I'm doing a piece about gerrymandering and I know I'm not great at mapping with GIS software, my pitch might have a lot of space dedicated to how great my interviews are going to me. It might distract the editor, but that's just ignoring the problem.

Instead, I can mention that if a "real" map doesn't work out I can use Illustrator to trace the images released by the political boundaries task force.

!!! tip

    Okay, so maybe cold-pitching someone you've never worked with before and explaining how awful you are at one thing or another isn't a great idea! But for internal pitches, class pitches, etc etc, this shows that you've really thought things through, and gives you a roadmap for when issues come up.

## Reducing risk

### Blockers and points of failure

When you're working on a project, things will always end up going wrong! The ones to watch out for are **blockers** or **single points of failure**. These are situations that you get into where you can't move forward until the problem is resolved. Depending on what your project is, some examples might be:

* Scraper gets blocked or isn't possible
* FOIA request isn't fulfilled
* Can't figure out how to make X chart
* Your one dataset isn't interesting

The more potential for blockers, the more risk, the more of a chance your story won't get done. It's important to structure your story in a way that if one or two parts fall apart, the rest of the story doesn't go with it.

The easiest way to protect yourself is by having complementary approaches and resources at hand. Multiple datasets, multiple sources, multiple visuals. It might be a little more effort to plan up front, but it's a lot more comfortable than staring at your screen for sixteen hours because a Python script won't do what you're asking it to!

### Risk in data sources

All data sources have the potential to increase risk! But custom-made datasets are some of the more difficult ones.

1. **FOI requests** might take months to obtain or never be granted at all
2. **Large text datasets** can be difficult to parse and process
3. **Scrapers** have a tendency to get blocked, break, or miss edge cases
4. **Hand-entered records** typically require a lot of cleaning

To reduce risk with your big fancy data source, **always have alternative, simpler datasets within arm's reach**. It's good to have some spreadsheets or CSVs that you can rely on if the other parts don't work out.

!!! info "What if the dataset *is* my story?"

    You should almost never rely on a single dataset as the sole reason your story exists. With rare exceptions stories exist because of *ideas*, not because of data. There's always some way to push your story in another direction, expand it a little, cover something slightly tangential – anything to make you less dependent on that one source.
    
    And if your original data source works out? Congratulations, you can use the secondary one(s) to make your story deeper and more interesting!

### Risk in analysis

The biggest risk in your data analysis is spending a lot of time *looking* at it but not asking it any *questions*. 

Let's be honest: I hate exploratory data analysis. To me, EDA is the idea that if you just poke around at a dataset long enough you'll find a story inside of it. I don't find that to be true! Instead you burn a lot of time looking at histograms and averages without aksing yourself *why* they might be interesting.

To reduce risk when heading into the analyis step, be sure you have a **clear goal going into your analysis.**

Personally, I like to write headline templates about what I'm looking for. For example:

* Rent dropped ____% during first wave of pandemic
* Trash collection complaints spiked to _____ during sanitation workers' protest regarding vaccine mandate
* As workers return to the office, animals are being returned to shelters at ____ times the normal rate 

Now all you need to do is fill in the blanks! And note that it doesn't matter if the data doesn't support the fill-in-the-blanks headline: it's just an exercise to direct our analysis.

As another similar option, I've heard of other people brainstorming based on the tweet that their story would get.

!!! tip "Make sure it's measureable"

    I was recently talking to a student who wanted to compare right-wing politicians' content on Twitter compared to Parler. While getting the data might provide its own stumbling block, what do we *mean* by comparison?

    You might want to compare how provocative they are, or how angry, or how much spin they put on events. *But how do you measure any of those?* Calculating the time of day they tweet or counting how many posts mention the word "taxes" are all simple and easy to measure. You can't measure provocativeness in the same way, though, as it's not something specific and countable.

    Yes, [sentiment analysis exists](https://investigate.ai/investigating-sentiment-analysis/comparing-sentiment-analysis-tools/) and there are [more nuanced approaches](https://www.nytimes.com/interactive/2017/02/28/upshot/trump-sounds-different-tone-in-first-address-to-congress.html), but make sure you know exactly what you're measuring and how you're doing it before you end up going down a rabbit hole.

### Risk in visualization

To reduce risk with your data visualization, **get into the practice of iterating.**

Instead of attempting to build the fancy, magic, perfect visualization all at once, start with something simpler and build it up piece by piece. That way if you hit a wall (or a deadline!) you still have something you can use.

A simple way to do this is start with a basic bar chart or scatterplot. No highlights, no annotations, no nothing. Use whatever you're most comfortable with: Datawrapper, pandas, ggplot, anything is fine.