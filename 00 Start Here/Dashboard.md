
> [!note] Daily Flow:
1. Visit `Dashboard.md` (this page)
2. Read your goals & sabotages
3. Create or update your daily log

Consistency > Perfection.
Let’s go.

*Read [[README|this]] first then you can delete this 👇🏼 line and everything above it for a clean dashboard.*

___
### 🧭 Your Daily Dashboard

> [!success]+ 🏆 **Win Moment?**
> Click the 📅 **Daily Notes** button in the sidebar to jump to today’s log — scroll to **"Any Wins Today?"** and lock it in so you don't forget! — [🍽️ Log Today's Meals](https://www.myfitnesspal.com/food/diary)

___
```dataviewjs
const quotes = [
  `"Discipline isn’t something you do. It’s someone you become." — Unknown`,
  `"We are what we repeatedly do. Excellence, then, is not an act, but a habit." — Will Durant`,
  `"The chains of habit are too light to be felt until they are too heavy to be broken." — Samuel Johnson`,
  `"You must expect great things of yourself before you can do them." — Michael Jordan`,
  `"The man who loves walking will walk further than the man who loves the destination." — Unknown`,
  `"He who has a why to live can bear almost any how." — Friedrich Nietzsche`,
  `"Suffer the pain of discipline or suffer the pain of regret." — Jim Rohn`,
  `"Success is nothing more than a few simple disciplines, practiced every day." — Jim Rohn`,
  `"The first principle is that you must not fool yourself — and you are the easiest person to fool." — Richard Feynman`,
  `"It’s supposed to be hard. If it were easy, everyone would do it. The hard is what makes it great." — Jimmy Dugan`
];

const randomQuote = quotes[Math.floor(Math.random() * quotes.length)];
dv.paragraph("> 💬 *" + randomQuote + "*");

```

___

![[My Plan#🎯 What do you want to achieve?]]

___

![[My Plan#🚧 Who or what will try to stop you?]]

___

## 🏆 Recent Wins — Last 3

```dataviewjs
const pages = dv.pages('"02 Journal Entries"')
  .where(p => p.wins && p.wins.length > 1) // only entries with non-empty wins
  .sort(p => p.file.name, 'desc')          // sort newest to oldest
  .slice(0, 3);                             // take the top 3

if (pages.length) {
  const rows = pages.map(p => [p.file.link, p.wins]);
  dv.table(["Date", "Win"], rows);
} else {
  dv.paragraph("No wins found yet. Log one today!");
}


```

___
### 📖 Resources

> [!tip] #### 🛠️ Tools & Ideas  
> Helpful tools for tracking, discipline, and staying sharp on your journey:
> 
> - [[Helpful Apps & Tools]] ← Tools to stay sharp
>     
> - [The Vertical Diet](https://amzn.to/3SK48F3) ← This book explains how all the other diets work and much more
> - [Links Page](https://davidsbrainapk.com/mp/links) ← Links to products and things I use in my human terrarium 
>     

> [!tip] #### 🧠 Awareness  
> Mindset shifts and mental models to help you stay grounded and flexible:
> 
> - [[The Map Isn’t the Territory]] ← Plans are useful, but the real world will demand flexibility
>     
> - [[Brick Mentality — Stack Days, Not Streaks]] ← You're stacking bricks, not "starting over"
>     
> - [[The Inner Voice — Your Greatest Ally or Enemy]] ← How to speak to yourself when motivation dips
>     

> [!tip] #### 🍗 Food  
> Staying nourished and flexible — the strategies, not just the meals:
> 
> - [[Food Cheat Sheet]] ← Examples of different macros
>     
> - [[Easy Options]] ← Staples for when time is tight
>     
> - [[Fasting Tips & Tricks]] ← A strategy to eliminate temptations and distractions
>     
> - [[Crisis Craving Options]] ← If you're gonna cave, cave smarter
>     
> - [[Processed Foods]] ← Foods built for addiction

> [!tip] #### 🧪 Hacks and Tips  
> Fitness tricks, recovery ideas, and body-priming techniques for faster progress:
> 
> - [[Leverage Glycogen — Ultimate Gohan Mode]] ← Good news... bagels will make you jacked
>     
> - [[Moments of Weakness]] ← Feeling weak? Read this...
>     
> - [[Sleep Hygiene]] ← Bad sleep is making you an NPC
>     
> - [[Stay Hydrated — or Stay Flat]] ← SpongeBob, you are dried out. You need some water
>     
> - [[Stay Moving, Stay Sane]] ← Move it, Spidey... movement is life
>     
> - [[The Scale vs. The Jeans — Who You Gonna Trust]] ← Ignore the scale, trust the process
>     

> [!tip] #### 🔍 Things You Should Know  
> Hard truths and helpful reframes to prepare for the road ahead:
> 
> - [[Burning Fat]] ← _The first two weeks feel like withdrawals_
>     
> - [[Reset Rituals]] ← Sometimes you need a reset...
>     
> - [[What Is & Isn’t Possible for You]] ← Don’t train like someone else’s body is yours
>     
> - [Real Life Examples or Inspiration](https://davidsbrainapk.com) ← My Publish site with real methods, meals, and results
>