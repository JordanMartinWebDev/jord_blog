---
thumbnail: 'src/lib/assets/Full Logo.svg'
title: Hard Lessons For An Early Dev
description: A practical guide to learning development without tutorials to slow you down. Why it's important to just get started.
date: '4/11/2024'
categories:
- "programming"
- "practical advise"
---

# Hard Lessons For An Early Dev
## **You're Going To Suck** (at first)

If you've been around the software engineering community for a while, you've likely heard to "just start coding." But if you're anything like me, this is easier said than done. What should I build? What technologies should I use? Has this been done before? Is this good enough for my resume?

Paralysis by analysis. Deer in headlights. **BOOM!** You're done for.

The truth is, it doesn't matter, you're going to suck.

Take any other skill. Piano, basketball, skiing. Everyone starts off being terrible. But for some reason, as a software engineer, we think we should come out of the gate like Linus Torvalds. The truth is, we are all going to be really bad when we first start out. The key is practice. That's how you get good at anything.

## **Practice**

So in a normal article, this would be where I give "10 projects to practice your coding skills NOW." But if you're anything like me, this isn't helpful. Showing me all the things I don't know how to do, then offering me a tutorial to follow step-by-step, isn't just un-helpful, it's counter-intuitive. Let me explain.

You don't get good at piano by watching your piano teacher play and following right along with them every step. You get good by going home and practicing what you know. The same can be said for most skills. We learn by doing, not by following.

Tutorials are a double-edged sword. While they can be useful in the right circumstances, as a beginner you're too new to determine those circumstances for yourself. You end up watching tutorial after tutorial and can't build a thing on your own. And forget documentation, you'll just find a YouTube tutorial instead. We call this "**Tutorial Hell**".

But where others tell you, "Don't get into Tutorial Hell", then try to sell you their $99 full stack in 30 days course...I'm not going to do that. I'm going to give you practical tips that I learned the hard way.

## **1) You're Going To Suck**

I think we've already covered this point a bit, but I want to reiterate it again. All of your projects don't have to be masterpieces. You don't have to create Facebook everytime you touch the keyboard. In fact, you SHOULDN'T try to make Facebook. As a beginner, you don't have a single clue what you're doing yet.

You're just simply not going to go from 'Hello World' to databases, docker, AWS, etc. So instead...let's start with **something you know**.

#### NOTE: The next section assumes you know at least 1 programming language. If not, I recommend Python for beginners and you should take a Python Fundamentals course to get you off the ground with basic control flow, loops, etc. DO NOT TAKE TUTORIALS TO BUILD THINGS! Only learn the fundamentals.

## **2) What Do You Know**

If you're fresh out of a fundamentals course, you should already have some powerful tools under your belt. You should know the basics of loops, control flow (if/then & logical operators), functions, println, basic data structures (arrays/lists), and Objects/Classes (if you picked an Object Oriented language). Believe it or not, you already have a HUGE toolbelt. So let's start building some projects.

First pick a project. Here are the rules. 
- You can't pick something that is completely out of your realm. No social media sites, asset management sites, etc. You don't know any of that, so **stop it**.
- Your idea doesn't need to be unique. You're far making a start-up right now, so we aren't going for unique. We are trying to learn.
- You can only use JSON or Text files for storage. No databases, browser cache, etc.
- Don't worry about "clean code", error handling, & whatever other niceties you can come up with. You want to get something that works (even if it is only the "happy path")
- Always commit to Git. I don't care if you think your code is bad. Make a private repo if you want, but have the practice of working with Git.

Here are some project ideas:
- Password Generator (Easy)
- Todo List (Easy)
- Calculator (Easy)
- Number Guessing Game (Easy)
- Money Convertion/Measurement Converstion Tool (Easy)
- Interest Calculator (Easy)
- Project Manager (Medium)
- Password Manager (Medium)
- Maze Solver (Hard) (GUI library allowed)
- Static Site Generator (Hard) (Markdown allowed)

Notice, **none of these are unique**. That's because we are not looking to make a masterpiece, we are looking to build reps. If you can come up with a simple project that's personal to you, that's great. Don't let uniqueness stop you though. If you don't have an idea, get started on one of these.

But where do you start? First I recommend breaking out a whiteboard (or excalidraw) and thinking about the features and components you'll need. Let's use the Password Manager project as an example.

What features does a password manager need to have? The ability to generate passwords, store passwords, retrieve passwords, and delete passwords.

Now, break this down even further. "Ability to generate passwords" sounds like you're constructing an object. In this case, the object being a 'Password.' What would that object have on it? A name for what site it's for? The password string? How are you going to generate the password string to fill this object (probably a function)? Draw a diagram of this.

Now you have a password object. How are you going to store them? Well, lucky for you I already decided that for you. You're going to use a JSON file to output your data to. You may not know how to do this.

**WAIT!** Don't reach for a password manager tutorial. Reach for **exactly** what you need. Google "how to output python object to JSON file."

Take note of this. As an engineer you'll be solving unique problems. Problems there aren't a tutorial for on YouTube. We need to know how to reach for the content we need. We do this by breaking down and understanding our problems "in the details."

You'd continue this idea through the rest of making a password manager. The good part of this project is it's expandable. Let's say you have the basic CRUD (Create, Read, Update, Delete) operations in place...you should never store a password in plaintext. How do you hash the password? How do you encrypt the JSON file? How do you protect from errors? How do you protect from bad user input? You can take this project further.

## **3) ALL HAIL THE TUI!!!**
You don't NEED a GUI. Repeat after me. **YOU DON'T NEED A GUI**. A Terminal User Interface (TUI) is perfectly fine while you're learning. Heck, even professionally there are some amazing applications that use TUIs. Think about how you run your programs, install packages, etc. None of these great pieces of software have a GUI. So if it's good enough for professional production code, it's good enough for you.

Learning the fundamentals of programming isn't flashy. I see so many programmers (including myself) spending large amounts of time designing, planning, and building a glorious frontend...for your mom and one friend to visit the site one time. **Stop it**. Use a TUI. Focus on the construction and achitecture of what you're building. Worry with fancy UIs later.

*"But you don't understand my app is special and complicated!"*

First off...no. You don't know enough for your project to be too special or too complicated right now. But let's say you're stubborn...how about a better TUI?

Check out some of these libraries to elevate your TUI:
- Charm (Go)
- Rich (Python)
- Prompts (NodeJS)
- Inquirer (NodeJS)
- Chalk (NodeJS)

## **4) What Next?**
You've made a simple project with a TUI. Congradulations!!! Now do it again. Pick a new project and go.

You thought you were done with the basics after 1 project? Think again.

New project means new challenges to overcome. Pick something else and get started with it. **NO TUTORIALS!** Search only for what you need when you're completely stuck. This is how you learn, this is how you grow.

## **5) What's After?**
After you've made several projects utilizing a TUI and your foundational knowledge, I want you to spread your wings. But not too far.

Try adding 1 more piece of tech to your next project. This could be calling an API and manipulating the data, making a GUI for a new application, etc. But only add 1 technology! Not 2 or 3, that's too much to digest all at once. Now make 2-3 projects with these techs.

What's after that? Add another tech.

**Build stuff**.

After that? Add another tech.

**Build stuff**.

## **Conclusion**
This is what I've found to be the best way to learn. Am I an expert in everything I touch? No.

But through this method of starting with what I know and learning to learn on my own, I'm growing faster than I ever have before.

This is engineering. Figuring things out and making them work. No tutorials.
