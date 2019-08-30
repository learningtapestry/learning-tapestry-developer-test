# Learning Tapestry Front-end Developer Test

This is a test project to assess a software developer's skills. This test is a form of [Kobayashi Maru scenario](https://en.wikipedia.org/wiki/Kobayashi_Maru). (Yes, some of us are dorks).

## Tips for passing this test
Refer to [this list](https://github.com/learningtapestry/learning-tapestry-developer-test/blob/front-end/detailed-requirements.md#tips-for-passing-this-test) for advice on doing well on this test.

## References

Refer to: [Wikipedia API](https://www.mediawiki.org/wiki/API:Main_page)

## Requirements

- Read and follow all the [detailed requirements for this project(https://github.com/learningtapestry/learning-tapestry-developer-test/blob/front-end/detailed-requirements.md#detailed-requirements)

## Instructions

- [ ] 1) Pull the data from the [Wikipedia Recent Changes API](https://en.wikipedia.org/w/api.php?action=query&list=recentchanges&format=json&rcstart=2019-08-29T10:59:20Z&rcnamespace=0&rcshow=!minor%7C!bot%7C!anon%7C!redirect&rclimit=500&rcdir=newer).

    - Bonus: Use rcstart to fix the results so that reloading the page will only update to show results by hour. So if the browser time is 10:59:59, the system will only show data for 10:00 and earlier, and at 11:00:00, it will show data for 11:00:00 and earlier.

- [ ] 2) Build a user-interface to present this data. Paginate the data to 20 rows. 
    - Bonus: pagination size is user configurable. 
    - Bonus: Data sort or filtering options are provided in the interface.
    - Bonus: User interface element allows user to load all recent changes (ignoring rcstart limit above)

- [ ] 3) Build a second user-interface that allows the user to click on each article and display the more detailed Wikipedia article page. This page should be built using the Wikipedia API+json and not just (for example) an i-frame to the Wikipedia article page. 
    - Only do this item if you have time. But do this item before the bonus tasks above.
    - This interface page could be part of above screen in #2 as part of a single page application approach. 

- [ ] 4) Write tests for as many aspects of the functionality as you have time for, and are needed. Prioritize integration tests that show the system is working correctly overall (but functional and unit level tests are welcome).

## Notes

- We believe it is impossible to finish this job completely in 8 hours. Try to get a basic end-to-end prototype solution working. Do the best you can - your effort and approach are being tested. We are also trying to understand how you wrap up a project temporarily before it is fully complete.
- If you run into trouble, ask us questions by emailing your point of contact for the test. We can provide feedback on what is important to focus on, or whether a particular framework or library is allowed under the test, but we can't provide feedback or direction on work in process.

## Evaluation Criteria (in order of importance)

0. Do the final results show that the instructions and guidelines above were followed?
1. Is there an end-to-end architecture in place that clearly describes a solution that works?
2. Does the code have tests? Do the tests cover the most critical functionality of the project?
3. Is the code cleanly implemented and using adequate software patterns? Is the overall project well-organized and orderly?
4. Is the code efficient? Does it make inappropriate use of system resources, like consuming far too much ram?
5. We assume the project will not be completed entirely. Does the final report give a good summary as to what work is remaining, how to solve it, and how much time it will take?
6. Does the project code follow a consistent style?
7. Are the git commits small and with good comments?
8. Is the code easy to install?
