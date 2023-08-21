# Liberty Mutual Capstones

Welcome to capstones! You'll spend 10 days working in groups on your own app, concluding with a project presentation for your colleagues at Liberty.

## Project Requirements

Your app must have:

* A broad thematic purpose with multiple features
* A styled front-end written in React (styling can be accomplished however you want)
* An API written in Express
* Models written in Mongoose
* A Mongo database
* A working deployment
* A least one create, read, update, delete, and list operation

Beyond that, you have a lot of flexibility in how you approach this. Not every app or feature needs to lean on each layer to the same degree and you may use additional libraries, 3rd-party APIs, and technologies as you see fit.  Don't overthink it, just make an app!

## Presentation Requirements

Your group must present your project live. Requirements:

* Limit your presentations to 5 minutes. I promise no one in the audience has ever wanted a student web app presentation to be longer.
* Everyone in your group should participate in the presentation
* Your app should have an accompanying slide deck with the following information in roughly this order:
	* An opening slide with your app name and group members
	* What problem your app addresses
	* How your app makes this problem better
	* What was interesting and/or challenging about working on this project
	* What technologies you used to build it
	* A closing slide with the app name and group members
* Your presentation should include a live demonstration of the app

Since the presentation will be the only thing most of the audience sees, we'll use it as our primary measurement of progress. We'll have **multiple times** over the 10 days where we dry-run project presentations together, including in the first few days of the project! It's intended to be an incremental thing where you're getting feedback on your week and incorporating it as you go. This has an added benefit of helping focus your project on presentable features.

## How You'll Work

### Feature-based Development

Work in **features**, not **layers**. A feature has:

* A real-world benefit to the people who use your application
* A web interface they interact with to get this benefit
* An API server to provide data and other services to the web interface (as-needed)
* A way to persist data needed for the feature (as-needed)

For example, an application that saves your favorite restaurants might have "list local restaurants" as a feature. Creating this feature would involve (in this order!):

* Figuring out why someone would find this feature valuable, such making it easier to decide on a restaurant
* Designing and implementing a layout for the providing this benefit with React and CSS/Bootstrap
* Creating a list route in an API with Express
* Creating a schema for restaurant data with Mongoose
* Storing the restaurant data in a Mongo database

This isn't waterfall development, so if you discover a problem with your user interface while designing the data schema, you should go back and make everything agree. The point of working front-to-back isn't to get everything right the first time; it's to make sure that everything you're doing is focused on providing some direct user benefit.



Some smells that you're doing this wrong:

* You're designing and/or building your entire database schema or API before building the user interface
* You're adding data fields or API endpoints that aren't being used yet, or links to pages that don't exist yet
* The benefit of the feature can only be described using technical language such as "API", "database", etc.
* You're starting to work on another feature before finishing the last
* You have multiple parts of features started but not finished
* Your features aren't styled

If you do this correctly, your project should be "done" multiple times through the duration of capstones, because at the end of each feature you shouldn't have any loose ends. This also means that you're working on exactly one feature at a time. **All of this dramatically reduces the stress of development**. Instead of trying to guess how much you can get done in 2 weeks up front and crunching & cutting corners in the last 3 days to cram it all in, each finished feature leaves the project in a potential "done" state. This means that when you run out of time, you can present the 3 features you have have instead of trying to cobble something together out 10 half-finished things that didn't quite get done. It's counter-intuitive, but it's [mathematically impossible](https://en.wikipedia.org/wiki/Little%27s_law) to increase how much you're getting done by starting more things at once. As agile folk say, "starting things feels fast; finishing things is fast."

### Ensemble Development

You'll work in groups _the entire time_. This means you shouldn't:

* Split up the project so that everyone is working on different features
* Split up the project so that one person does all the styling, another does all the database work, etc.
* Work solo for a period of time and then try to integrate the individual work into the group project ("Scatter/Gather" development)
* Work on the project at night or on the weekend without your group

You can take time to think, research individually, or experiment as needed, but all production code should be written as a group. It's up to your group to figure out navigator/driver rotation, breaks, and priorities.

## Getting Started

1. The first thing your group needs is an app idea. You should discuss multiple ideas. Prioritize stuff that sounds fun to use and work on and can be incrementally developed.
2. Next, brainstorm some features for this app. They should be **small**. "Users can delete a dog from the available list" is a good feature; "Users can manage dogs in the app" is way too big. Prioritize these numerically. If you only got 2 features done the whole 10 days, would the first two be ones you'd pick? What about 3? What about 6?
3. The **next** thing your group needs is a slide deck for your presentation (seriously). Start with the end in mind; what would a successful project presentation look like? When come up with your live "demo" for this presentation you won't actually have an app, but act as if the project were done. What would ideally you say and do to show the app working? You'll come back to this throughout the project to help focus your work and refine your presentation.
3. Next, create a Git repository on GitHub and make sure everyone has access. You are free to create your own, use separate repos for frontend and backend or one for the entire project, use Eric's starter code repos, or reference them or any other projects in your own hybrid approach. I think creating your own from scratch will ultimately be easier for your, but I'll leave the decision to your group.
4. Take a moment at this point to discuss how you're going to work together. This might include talking about days you can't come to class, how long you think rotation times should be, any strengths you can bring to the group and growth areas you're looking to expand on during the week.
5. The last thing you need to get started is an initial feature or two that cut across your whole stack. The goal is make sure your entire deployment pipeline works up front. The feature should be ~trivial technically so you can focus on getting all of the plumbing working. This is **not** where you design a full layout for the site, build a nav bar with links to all of the stuff you'll eventually have, or build a full database schema. It should still be styled and useful. A good first target is something that helps a user identify what your app is called and what it does.

All of this might take a day or two, and that's OK. After this, you're off to the races! Work through your feature priority list. It's not a contract and you can and should change it as you move along, but your priority list should help keep you focused and all on the same page about what your next goal is.

## General Capstone Tips

* Capstone ideas don't need to be ambitious, viable as a business, or original. A to-do list that you can hit a home run with will end up being a better project than an AI laundry service that you can't really pull off.
* Your capstone idea should be personal rather than generic. Instead of a generic to-do list, make one focused on steps in a recipe, or a camping checklist, or a list of wine varietals to try. It should be something that your group finds interesting enough that you won't mind spending 2 potentially frustrating weeks working on it!
* Clean up as you go. After every feature, you should be proud of the state of the codebase. That means good variable names, no commented out code, no sloppy designs. If you try to put all of that off until day 9, there's a 100% chance you'll break your app in the process.
* Keep your commits small! If you need to cancel a feature or if you break something, you'll want those save points to go back to. In general, your commits should reflect how much time you're OK with losing; burning 5 minutes isn't a big deal, but losing an hour of work hurts.
* **Relax**. This isn't the most important project of your entire life, and in 2 weeks you can either keep working on it on your own, start a different project, try to do this one over again, or even never write a line of code again. You'll do a better job and have a more pleasant 2 weeks if you don't pressure yourself and just have some fun and stay open to learning new things.
* If you get stuck, rely on each other first. If you've been stuck for a significant amount of time (say ~20 minutes) reach out for help so we can get you unblocked and back on track.
* For most resources, the following sequence of actions is often the most useful:
	1. **List**: Worst case scenario, you manually enter everything into the database but lots of people can see it
	2. **Create**: Once you've deleted everything you can't delete any more, but there's no limit to how much you can add. This usually makes adding records the next most useful action.
	3. **Delete**: Update can be simulated with deleting and re-creating it with the updated data, making this usually more important than editing.
	4. **Get**: Accessing a single item from a list makes it possible to share that specific item with other people
	5. **Update**: Generally a more efficient and reasonable operation than deleting and re-creating something.
* Get fast at wiping out your database and having a fresh starting point. You may even want a script to make this easier!
