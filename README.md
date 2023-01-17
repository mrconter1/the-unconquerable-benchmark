# The Unconquerable Benchmark

The Machine Learning (ML) discipline has grown rapidly and has enabled machines to perform a variety of tasks, including image, text, audio and robot movement processing. This naturally raises the question of whether there exist any mappings that are still fundamentally beyond the reach of today's ML models. To address this, we have created a benchmark that is so difficult that no transformer or newer architecture currently is able to solve it. 

This benchmark consists of two inputs: an ordinary screenshot of an operating system and an instruction. The output should be the reasonable X and Y coordinates for the next clicking location in order to move towards solving the instruction.

## Benchmark Example

The following example contains transparent rectangles over each area corresponding to an instruction. In this example, there are several different instructions for one image.

### Input Screenshot
<img src="https://i.imgur.com/l5sQcJF.png" alt="drawing" width="250"/>

### Instructions (Rectangle Color in Respective Area)
* Close Window (Red)
* Check What Type of HTTP Security is used on the Site (Green)
* Ok (Blue)
* Change Color to Red Without Closing the Window (Pink)
* Check Browser Version (Yellow)

We believe this benchmark is a win-win situation; if no model can solve it, we can point to it as an example of a task that only humans can do. On the other hand, if a model can solve it, the results would be truly revolutionary.
