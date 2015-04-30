---
layout: post
title: "Bus Factor Valuation"
date: 2015-04-29 20:15:00 -05:00
comments: false
---

Probably most IT folks are familiar with the "[bus factor](http://en.wikipedia.org/wiki/Bus_factor)"
or "the lottery factor" if you prefer to think of good things happening to your
coworkers. It's the number of people who can get hit by a bus (or retire to a 
Carribean Island) before a project is doomed because no one knows how anything
works.

The question is, what is a good bus factor? For really small projects it's 
simply going to be 1 and that is just the way it is. Hiring two people who both
have complete knowlege of one job is just too expensive and the project simply
won't happen. For a larger project, how do you know whether 3 or 5 or 10 is 
appropriate?

Enter the **Bus Factor Valuation Formula**:

[![actual value = desired value * (1 - 1/bus factor)](/images/bus_factor_valuation_eq.png)](http://arachnoid.com/latex/?equ=%5Ctext%7Bactual%20value%7D%20%3D%20%5Ctext%7Bdesired%20value%7D%5Ctimes(1%20-%20%5Cfrac%7B1%7D%7Bbus%20factor%7D)%0A)

From a graph of that last term you can see that this is a pretty harsh 
function for small teams:

[![Bus Factor Valuation graph](/images/bus_factor_valuation_graph.png)]
(https://www.desmos.com/calculator)

If only one person knows how everything works, your project is worth nothing.
Even with 2 people knowing how your project works, your project is really
only worth half of what you want it to be. Past 4 or 5 people the value 
flattens out fast. If you want to get more than 80% of what you think your
project is worth, you need to start thinking about redundant teams, not
redundant people.

I won't make any statements about the fact that this equation imples every
project is [worth less than anyone thinks it is](http://finance.yahoo.com/echarts?s=^NDX+Interactive#{"range"%3A"max"%2C"scale"%3A"linear"}).

Here is my coworkers' take on this idea:

![Bus Factor Whiteboard](/images/bus_factor_whiteboard.jpg)

