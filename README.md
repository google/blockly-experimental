# Blockly Experiments

Google's Blockly is a web-based, visual programming editor.  Users can drag
blocks together to build programs.  All code is free and open source.

This repository holds experimental code: projects that didn't work out, but
might still be interesting references.

**The Blockly library is at
[github.com/google/blockly](github.com/google/blockly)**

## Accessibility Demo
The code in this directory renders a version of the Blockly toolbox and
workspace that is fully keyboard-navigable, and compatible with most screen
readers. It is optimized for NVDA on Firefox.

### Motivation
We built this demo in 2016/2017 and tested it with students at a nearby school
for the blind. The goal was to build workflows that combined the best parts of
block-based programming (such as high-level abstractions about available
functions and a lack of syntax errors) with keyboard-only navigation.

### Lessons Learned
We learned that:
- Students are not necessarily comfortable with a screenreader
- Completely removing the visualization makes it difficult for a sighted and
  blind user to work together

### Using the demo
Open the [demo
page](https://github.com/google/blockly-experimental/blob/master/demos/accessible/index.html).
This demo uses the compressed version of the code.

### Building
To build the demo you will need the rest of Blockly.  The `accessible` folder
must be at the same level as Blockly's `core` folder.  Run `build.py
-accessible` to generate the compressed and uncompressed files.
