# Learning Registry Developer Test
* A test project to assess a software developer's skills
* This test is a form of https://en.wikipedia.org/wiki/Kobayashi_Maru scenario

## References
* Refer to: 
  * https://github.com/learningtapestry/learning-registry-ruby-tools/tree/master/extractor
    * Example of how to extract data from LR
    * (Don't copy code code from this code base)
  * http://www.learningregistry.org (don't spend too much time understanding LR - it's a big, open source project)

## Instructions
* Generate agreement with us about what languages, databases and frameworks you will use for this project.
* Create an appropriate project with a private git repo (feel free to use Bitbucket or any free git provider)
* Use any libraries, frameworks or gems that you want
* Pull the data from LR api on server (approx 1000 records): http://node01.public.learningregistry.net/
* Normalize it as best you can into a relational structure
* Put it into a structured postgres database (not json fields)
* Expose the data via an api or html user interface
* Include a test harness and some tests
* Provide some basic documentation on how to use your project
* Limit your effort to no more than 8 hours total
* Create a final report of what you were unable to accomplish, and how long you think it will take to complete.
* Send us your repo via private access online, [git bundle](https://git-scm.com/blog/2010/03/10/bundles.html), or tar/gz file (we prefer a method that lets us see commit history).

## Notes
* We believe it is impossible to finish this job completely in 8 hours. Try to get a basic end-to-end prototype solution working. Do the best you can - your effort and approach are being tested.
* The Learning Registry API is pretty bad in quality of service: you will experience unreliability errors most likely from the API. That's a known problem. We have intentionally included LR in this project for that reason.
* If you run into trouble, ask us questions.

## Evaluation Criteria (in order of importance)
1. Is there an end-to-end architecture in place that clearly describes a solution that could work?
1. Does the implemented code work? (It only needs to work on a developer's workstation)
1. Does the code have tests?
1. Is the code cleanly implemented? Is the overall project well-organized and orderly?
1. We assume the project will not be completed entirely: Does the final report give a good summary as to what work is remaining, how to solve it, and how much time it will take?
1. Is the code easy to install?
1. Is the code efficient? (Does it make inappropriate use of system resources, like consuming far too much ram?)
1. Does the project code follow a consistent style? (If in Ruby, it should look mostly like https://github.com/bbatsov/ruby-style-guide, but perfection is not expected. Other languages should follow similar standard convention standards.)
1. Are the git commits small and with good comments?
