---
title: 'How I went from a Composer to a Data Engineer'
date: '2024-12-10'
tags: ['Career Change', 'Python', 'Data Engineering', 'Side Projects']
description: "How doing some side gigs at my girlfriend's school shot me into job stability"
---
<!--


I never planned to become a data engineer, or work with computers, at all.

The year was good ol' 2021, I was 20 years old studying Music Composition, writing music for student films and piss-poor videogame developers, living under my mom's roof and earning about 15 bucks a month. My girlfriend was struggling with Stata for her econometrics class and ranted all day about how her stupid computer would correct her but not auto-fix her errors, which pushed me to reach in and help her out: "I've always had my way with computers" I thought, so I started learning on a pirated copy of Stata MP on how to help her.

I reached out to my best friend, who was also in her class, and asked if he wanted to do this together. He agreed, and we started working on that semester's econometrics project together.

I started by throwing together some Do-files and moving data, following the TA's instructions. We got the hang of it quickly, and before we knew it, we were doing more and more.

```stata

* DONT REMOVE THIS OR IT BREAKS
clear all
set more off

* load the csv (CHANGE THE FOLDER TO YOURS)
import delimited "[...]", clear

```
> All my scripts had this at the beggining, so my best friend wouldn't remove it when working his part.

---
I started to realize that the whole data-cleaning process required a lot of patience and attention to detail, which is something I had always been good at. And the repetition involved pushed me into loops and functions, which I've never had to do before.

This whole data-cleaning experience, which was around 80% of the grunt-work of the project, was a great learning experience for me. My best friend and I had fun doing it, and _we_ (my girlfriend and my best friend) got some pretty good grades out of it.

That settled it, I would do the Stata projects for my girlfriend that semester and in the future, and that's what I did.

```stata
foreach var of varlist q87-01 q88 q90-07 {
    replace `var' = 0 if `var' == .
}
```
> This took me about 2 hours to get working. I'd never used backticks in my life, so I was writing 'var' instead of \`var', thanks StackOverflow!

---

After doing 2 or 3 of these, I got really tired of the cleanup using Stata, so I started to search for youtube videos doing it on python. It was pretty fun and easy to understand, and I really felt like a hacker whenever I ran the script and it worked.

Honestly, the best part about this was getting the code pre-made by the community in StackOverflow, it's a lot easier to find weird edge cases for python than for Stata there.

Finally I accepted my destiny and started to do the homework for other students in the class for a fee, which was both a lot of fun and a lot of money. And of course dug directly into my performance in university, which was not good at all.

Word got around. Suddenly I was tutoring half the class. Students paid me to clean up the data in R instead of Stata and how to make sick graphs with ggplot2. This was 2022 already and it felt like free money compared to music gigs.

---

## The Development

I started a loop, falling deeper and deeper into what I could do automatically with python, some homework in my own classes, the first miserable attempts at a website (Had no clue what Javascript was, so it was python + html).

With it, I also started programming music, using PureData, Max/MSP and its connection with Ableton Live. So I also had a comeback on music again, making friends with the electroacoustic nerds in my class.

This was also the release of the infamous ChatGPT, which was a game changer for me. I was able to get answers to my questions in a matter of seconds, and I was able to learn a lot from it. This is where I started to follow actual programmers on social media, and getting ideas of becoming a videogame dev.

Of course those ideas were pretty short-lived when I installed Unity and looked at a single line of C#, I got scared, and promptly fucked right off videogame development. I was also starting to see how difficult it was to make a living as a musician, and how much easier it was to make a living as a programmer, but didn't have too much faith on how much anyone would pay for the simple and easy-to-learn python.

---

## The Pivot

I graduated from university on December 2023, finally freeing myself from the shackles of singing atonal music every week and practicing piano 2hrs a day. I started looking for jobs in the area, videogame programming, something remote in the US or Europe to take advantage of how high the pay is in comparison to my home country.

Even though the economy was booming in 2023, it was still pretty tough to find a job in my field. My girlfriend and mom encouraged me to broaden my search, stay in my home country, and look into data analytics or other IT jobs, the kind you don’t really understand until you’re actually doing them.

I found a certain opening on Datawalt, a company which I've never ever heard of before, but I applied anyway, with my resume being pretty much only Music stuff, and being very transparent on my non-existent experience in the field.

The interview was really funny, they asked me questions about my music background, what videogames I played, a lot of questions about my hobbies and my life. I was really surprised, but I was able to answer all of them, pretty successfully, but the skill test was a bit more difficult.

I got 2/10 questions right, and took it as homework, to send them back in a few days. Which I did only 3 hours later, with a bit of help from ChatGPT.

To my surprise, they hired me as an Intern BI Developer. Within a year, I was leading their first Data Engineering team, and designing the company's main data platform for all our clients.

-->

I never planned to work with computers, much less become a Data Engineer. I was a <span style="color:#ef4444; font-weight:bold;">musician</span>. A <span style="color:#ef4444; font-style:italic;">struggling</span> one. The year was 2021, I was 20, and I was studying Music Composition, writing scores for student films and piss-poor videogame developers while earning a magnificent average of **15 bucks a month**.

My journey began not with a career plan, but with a girlfriend who was losing her mind over her Econometrics class. Her biggest enemy? **StataCorp** and their fuck-ass software called Stata. She ranted endlessly about how the stupid computer would *correct* her but never *auto-fix* her errors.

_"I've always had my way with computers,"_ I thought. So, I grabbed a <span style="color:#8b5cf6; font-weight:bold;">pirated copy</span> of Stata MP and started <span style="color:#10b981; font-weight:bold;">digging in</span>.

## The Overture: From MIDI to Munging

I roped my best friend (who was also in the class) into the chaos, and we started tackling the semester’s econometrics project. I began by throwing together some Do-files, following the TA's instructions, and moving data around.

My scripts were notoriously cautious:
```stata
* DONT REMOVE THIS OR IT BREAKS
clear all
set more off
* load the csv (CHANGE THE FOLDER TO YOURS)
import delimited "[...]", clear
```
The early grunt work was data cleaning, which was about **80% of the project**. I quickly realized that the process required intense patience and attention to detail—something I was surprisingly good at. The repetition pushed me into learning my first loops and functions.

The learning curve was steep but <span style="color:#f59e0b; font-weight:bold;">hilarious</span>. I spent two hours fighting the simplest concept: the backtick.

> This took me about 2 hours to get working. I'd never used backticks in my life, so I was writing 'var' instead of \`var', thanks **StackOverflow!**
> ```stata
> foreach var of varlist q87-01 q88 q90-07 {
>     replace `var' = 0 if `var' == .
> }
> ```

My best friend and my girlfriend got great grades, and I found a <span style="color:#8b5cf6; font-style:italic;">bizarre</span> new hobby. That settled it: I was the designated <span style="font-family:monospace; background-color:#1a1a1a; color:#e4e4e7; padding:2px 4px; border-radius:3px;">programming</span> guy.

## The Crescendo: Free Money & Python

After a couple more semesters of <span style="color:#ef4444; font-weight:bold;">painful</span> Stata clean-up, I was exhausted. I searched YouTube and discovered how easy and fun the process was in **Python**. It felt like <span style="color:#10b981; font-weight:bold;">pure magic</span>. I'd run a script, and the job was done. I genuinely felt like a <span style="color:#8b5cf6; font-weight:bold;">hacker</span>.

The best part? The Python community on **StackOverflow** was a <span style="color:#f59e0b; font-weight:bold;">goldmine</span> for pre-made code, making it infinitely easier to handle weird edge cases than it was with Stata.

I finally accepted my destiny and started doing homework for other students (for a fee). It was fun, easy, and made me **a ton of money** compared to music gigs. I was suddenly tutoring half the class, teaching them how to clean data in **R** and make <span style="font-family:Impact,Arial,sans-serif; color:#ff6600; font-weight: bold; text-shadow: 1px 1px 0 #000, 1px 1px 4px #f90;">🔥SICK GRAPHS🔥</span> with **ggplot2**. My university performance, naturally, tanked.

## The Cadenza: ChatGPT and The Detours

I fell deeper into the <span style="color:#8b5cf6; font-weight:bold;">tech spiral</span>. Python became my go-to for everything: automating homework, <span style="color:#ef4444; font-style:italic;">miserable</span> early attempts at websites (pure Python + HTML, because I refused to even understand whatever the fuck was going on in the web world), and even programming music using **PureData** and **Max/MSP**.

Then came the <span style="color:#10b981; font-weight:bold;">legendary</span> (and infamous) <span style="background: linear-gradient(45deg, #8b5cf6, #06b6d4); color: white; font-weight: bold; text-shadow: 1px 1px 0 #000, 1px 1px 4px #f90; padding: 2px 6px; border-radius: 4px;">**ChatGPT**</span>. It was insane! I could get answers in seconds, boosting my self-education immensely. I even briefly toyed with becoming a videogame developer.

That dream lasted exactly as long as it took me to install Unity and look at a single line of **C#**, got <span style="color:#ef4444; font-weight:bold;">spooked</span>, and promptly fucked right off that whole scene. I was starting to see how <span style="color:#ef4444; font-weight:bold;">tough</span> it was to be a full-time musician, and how much <span style="color:#10b981; font-weight:bold;">easier</span> programming was, even if I doubted anyone would pay big bucks for "simple" Python skills.

## The Symphony: The Unlikely Pivot

I graduated in December 2023, finally freeing myself from the <span style="color:#ef4444; font-weight:bold;">shackles</span> of singing atonal music and practicing piano 2 hours a day.

The job hunt was <span style="color:#ef4444; font-weight:bold;">brutal</span>. My resume was mostly music and arts stuff. My girlfriend and mom encouraged me to broaden the search into **Data Analytics** or **IT**—the kind of jobs you don't understand until you're already doing them.

I found an opening at a company called **Datawalt**, a company I’d never heard of, and applied with almost non-existent experience. I was transparent: my coding background came from helping students cheat on econometrics homework, and had zero formal education in the field.

The interview was <span style="color:#10b981; font-weight:bold;">hilarious</span>. They asked about my music, my hobbies, and the video games I played. The skill test, however, was a <span style="color:#ef4444; font-weight:bold;">disaster</span>: **I got 2/10 questions right.** I took it home, hammered it out with a little help from my new best friend, ChatGPT, and sent it back *three hours later*.

To my <span style="color:#ef4444; font-weight:bold;">absolute shock</span>, that was enough proof, they hired the music composer as an **Intern BI Developer**.

Within a year, that music composer was **leading their first Data Engineering team** and designing the company's main data platform.

---

## What Actually Mattered (For a young startup)

- <b style="color:#7fd1b9;">Interview:</b>
    - Make <span style="color:#ffb347;">them laugh</span>, show you fit in, and that you fit the role. <br>
        &emsp;Make them see that you're a good fit for the company and the role.
    - Let them see you’re ready to learn. <span style="color:#b2bec3;">Graduates don't know shit out of University. </span><br>
        &emsp;Show them you’re <b>eager</b> to learn what they need you to do.
- <b style="color:#a29bfe;">Skill Test:</b>
    - Don’t stress about perfection <br>
        &emsp;Just do your best, and show how you handle errors and gaps in your knowledge.
    - Treat it as a taste of the real job, not a final exam. <br>
        &emsp;If you fail, you know what to expect now.
- <b style="color:#fab1a0;">On the Job:</b>
    - Be <span style="color:#ffeaa7;">honest</span> about your experience and skills.
    - <span style="color:#b2bec3; font-weight:bold;">Communication > technical skills. </span> <br>
        &emsp;Explaining what you build and why it matters makes people like you—and gets you promoted.
    - <span style="color:#ff7675;">Crunching</span> can get you noticed, but don’t make it a habit. Or you'll end up working late nights and weekends forever.<br>
        &emsp;Use it like a <span style="font-weight:bold; color:#ffb347;">turbo button</span>—only when you really need it.



## Now

I lead a team that processes <span style="color:#10b981; font-weight:bold;">millions of records daily</span>, for dozens of clients all over the world. I handle some <span style="color:#ef4444; font-weight:bold;">massive > hundred million records</span> historic loads weekly. And I still do some BI development for some clients, it's hard to drop that which gave you the job in the first place.

## TL;DR

Started learning to program to help my girlfriend with homework. Ended up not using my degree and <span style="color:#10b981; font-weight:bold;">leading a data engineering team</span>.