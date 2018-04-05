# Atlas: A voyage of discovery on the high seas of scripting

Slides for my talk at Scalar 2018 about building scripting languages in Scala.

Licensed [CC-BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/).

## Abstract

In this talk Dave will describe the design, motivation,
and implementation of [Atlas](https://github.com/cartographerio/atlas),
a scripting language written in Scala.
He'll discuss the use of functional techniques
to implement some interesting details
including parsing, sandboxing, monitoring,
and interaction with the host environment.
It'll be a chance to look at Scala
for an interesting and slightly
out-of-the-ordinary application.

What enterprise software is complete without scripting support?
When checkboxes and sliders aren't flexible enough,
simply embed [Python](http://www.jython.org/)
or [JavaScript](http://openjdk.java.net/projects/nashorn/)
to give your users all the power in the world!

All that power will go to their heads, though.
The code will need to be sandboxed and monitored
so scripts can't consume too many resources.
And it'll need to talk to the database
so it'll have to be asynchronous and non-blocking.
We can't expose any of that complexity to the user,
though, so we'll need to take care of unwanted effects in the interpreter.
And don't even get me started on endorsing
an imperative scripting language
in our beautiful Scala codebase.

No. JavaScript and Python won't do.
What we need is a *new* scripting language.
Something shiny. Something invented here.
How could this possibly be a bad idea?

## Further Reading

Here are some useful resources for those looking
to follow up on any of the material in this talk:

- Here's [the actual source code for Atlas](https://github.com/cartographerio/atlas)
- I highly recommend the free online ebook [Programming Languages: Application and Interpretation](http://cs.brown.edu/~sk/Publications/Books/ProgLangs/) by Shriram Krishnamurthi
- The talk [A Type Inferencer for ML in 200 Lines of Scala](https://www.youtube.com/watch?v=H7x4THVU4BQ) by Ionuț Stan taught me everything I know about ML style type inference
- The [FastParse](https://github.com/lihaoyi/fastparse) library by Li Haoyi is super great and well documented
- Haoyi's talk [Li Haoyi, FastParse: Fast, Programmable, Modern Parser-Combinators in Scala](https://www.youtube.com/watch?v=mARO-qchsKM) from Scala By The Bay 2015
