# Learning Tapestry Four Hour Developer Test

This is a test project to assess a software developer's range of skills. All the tasks in this test may take more than the available time to complete - this is intentional: This test is a form of [Kobayashi Maru scenario](https://en.wikipedia.org/wiki/Kobayashi_Maru). (Yes, some of us are dorks).

## Tips for passing this test

- Read this README carefully and come up with a plan to finish it as best as you can.
- Use simple frameworks instead of complicated ones.
- Ask us if you're unsure about something.
- Don't submit your project without tests. You won't have time to test everything, so choose what to test.
- It's better to accomplish only part of the project well, than to get partway done with everything.
- Use all the time available to you - if you can implement more and specify/estimate less of the project, that will improve your score. But wrapping up your work on the project clearly/cleanly is paramount.

## References

Refer to:
- https://homework.adhoc.team/fetch/ (or here if page is down: https://web.archive.org/web20190211200527/http://homework.adhoc.team/fetch/)

## Requirements

- You must use a minimal framework for the web aspect of the project. In other words, no kitcken-sink frameworks like Django or Rails, though individual components of those frameworks are OK.
- You must write meaningful tests.
- You must follow the instructions on this page closely.
- You must version your code with git.

### Ruby specific notes

- Do not use Rails. Any other libraries are allowed (ORMs are okay).
  - Note: The reason we ask you not to use Rails is because we want to see how you write software in this test. We use Rails regularly in our professional work, and expect you will use it here if you're a Ruby engineer. But in terms of seeing what kind of programmer you are, Rails tends to obscure certain skills that we would like to see you apply.
- Write tests with minitest or RSpec.

## Instructions

- [ ] 1) Follow the instructions for the FETCH project, however you should build the solution in the programming language you mutually agreed to, with the hiring manager here. The FETCH project refers to this project as a front-end app: for this test, consider this a backend API task.

  - Note that FETCH also refers to Javascript specifically, which you should ignore (though not the JSON!). In the "Additional Requirements" section, you can ignore all the library requirements and restrictions. 
  - Note also that the download file for this project is not working - so you have to stub out all the APIs and resources for this project in some way on your own.

- [ ] 2) Store the data as best you can into Postgres - it's fine to use json/b format where appropriate, but normalized data structures are generally preferred.

- [ ] 3) Write tests for all implemented components. Specify and estimate the amount of time required to complete test coverage .

- [ ] 4) Provide some basic documentation on how to use your project, including but not limited to installing the project and running the tests.

- [ ] 5) Limit your effort to no more than 4 hours total.

- [ ] 6) Create a final report of what you were unable to accomplish, and how long you think it will take to complete the remainder in total. Provide any feedback on the project itself: what went well, what was difficult, in what ways this test itself could be improved (you can also send PRs to this repo with suggestions - totally optional).

- [ ] 7) Send us your repo in a [git bundle](https://git-scm.com/blog/2010/03/10/bundles.html).

### Ruby specific notes

- You can use a Rake task to invoke 3).

## Notes

- We believe it isn't possible to thoroughly finish this job completely in the time alloted. Try to get something basic operational. Do the best you can - your effort and approach are being tested. We are also trying to understand how you specify and estimate future work, as well as how you wrap up a project temporarily before it is fully complete.
- If you run into trouble, ask us questions by emailing your point of contact for the test. We can provide feedback on what is important to focus on, or whether a particular framework or library is allowed under the test, but we can't provide feedback or direction on work in process.

## Evaluation Criteria (in order of importance)

0. Does the final result show that the instructions and guidelines above were followed?
1. Is there an end-to-end architecture in place that clearly describes a solution that will work? (Noting it won't be fully implemented)
2. Are the specifications and time estimates clearly written and reasonably accurate?
3. Does the code have tests? Do the tests cover the most critical functionality of the project?
4. Is the code cleanly implemented and using adequate software patterns? Is the overall project well-organized and orderly?
5. Is the code efficient? Does it make inappropriate use of system resources, like consuming far too much ram?
6. We assume the project will not be completed entirely. Does the final report give a good summary as to what work is remaining, how to solve it, and how much time it will take?
7. Does the project code follow a consistent style?
8. Are the git commits small and with good comments?
9. Is the code easy to install?

### Ruby specific notes

- We suggest following [bbatsov's style guide](https://github.com/bbatsov/ruby-style-guide)
