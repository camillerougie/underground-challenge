## The PLURAL AI Underground Challenge
---

We're delighted you're interviewing with Plural, and can't wait to meet you! Just to recap, our technical interview process consists of the following stages:

1. An initial phone call, congratulations, you aced that
2. This - a short take home project (you have a week to complete it from our initial email, but it shouldn't take more than one or two evenings)
3. An on-site interview (about half a day), which consists in a pairing exercise (which usually extends the project), and a final interview going deeper into your background and past projects. We then wrap up with a social with the team so you can get to know us on a personal level.

The goal of this project is to see how you tackle a novel challenge, how you design and implement a solution. There's no right answers, we're interested in how you think, how you work pragmatically and prioritise when there's lots to do. You may also have to pick up some new skills. It will also give us a starting point for the pair programming exercise we'll do when we invite you to our office.

We'll add you to our Slack workspace for the duration of the project and we encourage you to ask questions if you need clarification or advice. We're here to help, not just to judge. This project is also an opportunity for you to get a sense of what working with us is like. So don't be afraid to reach out.

The problem described below might seem like a toy problem, but it's actually a microcosm of the kind of challenges we tackle at a massively larger scale: ingesting data, structuring it, and then using the model to answer complex questions. We hope you find it intellectually challenging, and satisfying to solve.

---

## Problem Statement

*Using Wikipedia as your datasource, build a representation of the London Underground. Deploy your model in the cloud, then build a web API that will allow it to be queried.*

Attempt the following goals in order, see how far you can get in the time you have available.

*Step 1* - Fetch the list of stations from:
https://en.wikipedia.org/wiki/List_of_London_Underground_stations

*Step 2* - Build a representation of the stations and the connections between them.

*Step 3* - Now, add a new source, and update your model with DLR stations from:
https://en.wikipedia.org/wiki/List_of_Docklands_Light_Railway_stations

*Step 4* - Can you use your model to answer some simple questions? Which station has the most interchanges? Which line is the longest?

*Step 5* - Can you use your model for route-planning? For instance, can it tell you the best route from Farringdon to Canary Wharf?

*Step 6* - If you haven't already, create a server in the cloud, and deploy what you've written to it.

*Step 7* - Now expose your model through a REST API, so a caller can make the following queries:

    GET /station/{station-name}
    GET /station/{station-name}/interchanges
    GET /line/{line-name}/list-stations
    GET /route/{start-station-name}/{destination-station-name}

*Stretch Goal 1* - Create a simple natural language user interface which uses the API, and presents the results nicely on screen. This can be as simple as a Google-style text field, bonus points for usability.

*Stretch Goal 2* - Add a new feature to your application using your own initiative, with the potential to surprise and delight.

---

#### Requirements

* Please implement the server-side part of your solution in Python 3.x, you may use any language or framework for the user interface.

* Feel free to use 3rd party libraries or frameworks in your implementation. There’s no need to reimplement the wheel. Just create a virtual environment (venv), install any libraries you use with pip, then use pip freeze to write the requirements.txt

* You can deploy your code to any publicly accessible server, on any cloud platform of your choice.


#### Hints and Tips

* Prioritise clean, understandable code over hacky optimisations. Algorithms should be efficient, but also maintainable and easy to understand by your colleagues.

* You should be able to talk through what you’ve created, and the design tradeoffs you've made.

* The best technologies are the ones you know how to use, effectively and appropriately.

* Comments are our friends.

* Unit tests, yes.

* When you're ready to submit your work, just let us know on Slack, and we'll send instructions.

--- 

Enjoy the challenge, we look forward to seeing what you build!
