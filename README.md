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

## Evaluating the Benchmark

The screenshots for the benchmark can be found in the `images` folder. The corresponding metadata, including the coordinates of the hitboxes, are stored in the `data.csv` file in the following format:

> name_of_screenshot.png,0.5,0.5,0.52,0.52

The four numbers represent the normalized start/stop X and Y coordinates of the hitboxes.

## TODO

- Upload screenshots and metadata to this repository 
- Create a website to demonstrate proficiency in the task for human users 
- Develop a tool to facilitate the creation of additional tests 
- Create an additional benchmark that allows for more complex user interactions, such as long presses and scrolling.
