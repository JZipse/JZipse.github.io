---
layout: project
type: project
image: 
title: Baseball sim
permalink: projects/baseball sim
# All dates must be YYYY-MM-DD format!
date: 2019-02-19
labels:
  - Java
summary: I built a simple baseball game using baseball averages along with a random number generator and took a lineup using a queue
---



For one of my assignments in my data structures class, we were tasked with taking a baseball lineup consisting of 9 players and their 9 averages
and making a simple game that keep running through different innings until the winning score is met. Every inning had to end in either 3 outs or 
when the winning score was achieved. We also had to make sure we kept the batting order in tact so that every person was batting so after the first 
3 batters got out, when the next inning started, the 4th batter was up. This was achieved through the use of a queue that stored a batter object which
stored the first and last name as well as their batting average. To determine if the batter got a hit, a random number generator was used. If the number 
came out to be less than the average, it was a hit, and 4 hits would equate to 1 run. If the number was greater, the batter was out and once 3 outs were 
achieved, the inning ended.

I really enjoyed working on this problem as it really helped me get a handle on how the queue data structure works and I am also a big fan of baseball.
In the future I would like to adjust the game to add some more real life baseball elements like home runs and maybe even a balls and strike counter.

Here is some code that illustrates how I decided if the hitter achieved a hit:

```js
byte ADCRead(byte ch)
{
    word value;
    ADC1SC1 = ch;
    while (ADC1SC1_COCO != 1)
    {   // wait until ADC conversion is completed   
    }
    return ADC1RL;  // lower 8-bit value out of 10-bit data from the ADC
}
```




