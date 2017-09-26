# Learning Registry Developer Test

This is a test project to assess a software developer's skills. This test is a form of [Kobayashi Maru scenario](https://en.wikipedia.org/wiki/Kobayashi_Maru).

## Tips for passing this test

- Read this README carefully and come up with a plan to finish it as best as you can. 
- Use simple frameworks instead of complicated ones.
- Ask us if you're unsure about something.

## References

Refer to:
- [Learning Registry](http://www.learningregistry.org). Don't spend too much time understanding LR. It's a big OSS project.
- [LR extractor](https://github.com/learningtapestry/learning-registry-ruby-tools/tree/master/extractor). This is an example on how to extract data out of the LR. Don't copy code code from this code base.

## Requirements

- You must use a minimal framework for the web aspect of the project.
- You must write tests.
- You must follow the instructions closely.
- You must version your code with git.

### Ruby specific notes

- Do not use Rails. Any other libraries are allowed.
- Write tests with minitest or RSpec.

## Instructions

- [ ] 1) Pull the data from the [LR API](http://node01.public.learningregistry.net/) (3000 records are enough). Please include the code for that in your project, as well as instructions for operating that part of your solution. This part of the app should be written in the same language as the rest of the app.

    - The code that does this should be configurable and repeatable.

- [ ] 2) Normalize the data as best you can into a relational structure.

    - We would like you to deserialize the `resource_data` field, which contains UTF-8 strings that have XML or JSON data. You can skip some records that are poorly formed, but try to process as high a percentage of `resource_data` as you can.

    - The XML and JSON data will have a variety of schema, which may also prove challenging. Perfection in this task is not expected, but a good effort is. By "good effort" we mean that you might find some similar fields that you can process from many records, and you might drop some data that doesn't seem important or common from many of the records.

- [ ] 3) Store the data into a structured PostgreSQL database.

- [ ] 4) Expose the data via an API.

    - The API should have two methods:
        - /resources: Resource browser with pagination
        - /resources_by_identity: Aggregates resources by identity. Allows an `?identity=` parameter that filters out identities. If the parameter is not present, aggregated values must be displayed anyway. We encourage you to do the aggregation in SQL.

- [ ] 5) Write a piece of code that queries your API and displays the returned data.

- [ ] 6) Write tests.

- [ ] 7) Provide some basic documentation on how to use your project.

- [ ] 8) Limit your effort to no more than 8 hours total.

- [ ] 9) Create a final report of what you were unable to accomplish, and how long you think it will take to complete.

- [ ] 10) Send us your repo in a [git bundle](https://git-scm.com/blog/2010/03/10/bundles.html).

### Ruby specific notes

- You can use a Rake task to invoke 5).

## Notes

- We believe it is impossible to finish this job completely in 8 hours. Try to get a basic end-to-end prototype solution working. Do the best you can - your effort and approach are being tested.
- The Learning Registry API is pretty bad in quality of service: you will experience unreliability errors most likely from the API. That's a known problem. We have intentionally included LR in this project for that reason.
- If you run into trouble, ask us questions.

## Evaluation Criteria (in order of importance)

1. Is there an end-to-end architecture in place that clearly describes a solution that works?
2. Does the code have tests?
3. Is the code cleanly implemented and using adequate software patterns? Is the overall project well-organized and orderly?
4. Is the code efficient? Does it make inappropriate use of system resources, like consuming far too much ram?
5. We assume the project will not be completed entirely. Does the final report give a good summary as to what work is remaining, how to solve it, and how much time it will take?
6. Does the project code follow a consistent style? 
7. Are the git commits small and with good comments?
8. Is the code easy to install?

### Ruby specific notes

- We suggest following [bbatsov's style guide](https://github.com/bbatsov/ruby-style-guide)
