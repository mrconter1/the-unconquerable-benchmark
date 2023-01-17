# the-unconquerable-benchmark

As many people are aware the machine learning discipline is continuing to make great strides in terms of what it can do. Especially the transformers architecture together with scale seem to be able to process almost any kind of data including images, text, audio, and even robot movement. This naturally begs the question if there are any types of mappings it can not do. I choose to tackle this question in a very specific way by creating a benchmark that is so difficult that

I see it as a win-win situation. If no transformer (or potentially newer) architecture ever manage to solve it I can point towards this benchmark and go "Haha I managed to find an benchmark that only humans can do and we will at least always be better than machines in that aspect". If we ever get a model that can solve (i.e get 100% on the benchmark) it the consequences would be mindboggling.

The idea for this benchmark is very simple and is made up out of the following:

### Input
`A ordinary screenshot of an operating system` **+** `An instruction`

### Output
`X, Y coordinates` (The most reasonable *next* clicking location in order to move towards solving the instruction)

## Benchmark example

The following example contains transparent rectangles over each area corresponding to an instruction. In this example there are several different instruction to one image.

### Input screenshot
<img src="https://i.imgur.com/V6t9Ql9.png" alt="drawing" width="200"/>

### Instruction(s) (color of rectangle in correct area)
* Close window (red)
* Check what kind of http security that is used on this site (green)
* Ok (blue)
* Change color to red without closing the window (pink)
* Check version of the browser (yellow)
