# How to create a simple Processor

If there's no Demo processor it can be added this way:

By importing the processor `JupyterDemoProcessor.eops`
or
By creating a new processor, you can follow the screenshot present here and add the following `Dockerfile` and `workflow.sh` in the sources tab. Also input and output must correspond to the ones in the screenshot or can be changed by modifying the `workflow.sh` script.

This is possibly one of the simplest processor that can be run, it is simply concatenating two input strings and produces an output text file.