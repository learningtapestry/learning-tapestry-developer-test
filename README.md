# Learning Tapestry Front-end Developer Test

This is a test project to assess a software developer's skills. This test is a form of [Kobayashi Maru scenario](https://en.wikipedia.org/wiki/Kobayashi_Maru). (Yes, some of us are dorks).

## Tips for passing this test

- Read this README carefully and come up with a plan to finish it as best as you can.
- Use simple frameworks instead of complicated ones.
- Ask us if you're unsure about something.
- Don't submit your project without tests. You won't have time to test everything, so choose what to test.
- It's better to accomplish only part of the project well, than to get partway done with everything.

## References

Refer to: [Wikipedia API](https://www.mediawiki.org/wiki/API:Main_page)

## Requirements

- You must use the framework agreed upon between you and the hiring manager, for the web aspect of the project. You can add additional libraries and tools where needed, but it would be unreasonable (for example) to add Angular to a React framework project.
- You must write meaningful tests.
- You must follow the instructions on this page closely.
- You must version your code with git.
- All of your interfaces should use CSS for layout and style. You can use any CSS compiler, unless you are asked to use a specific one. You can use any CSS page layout framework (you should use one), unless you asked to use a specific one.    
- Your pages should be stand-alone HTML, meaning they can just be loaded into a browser locally and they will work. It's fine to use a compiler but your final work product should be stand-alone.
- Your user interface can be simple, but it should be functional and nice to look at. You aren't being tested on your graphic art skills or your UX design skills, but you are being tested on your ability to make simple, nice looking interfaces based on api data.
- Provide some basic documentation on how to use your project.
- Limit your effort to no more than 8 hours total.
- Create a final report of what you were unable to accomplish, and how long you think it will take to complete.
- Send us your repo in a [git bundle](https://git-scm.com/blog/2010/03/10/bundles.html).

## Instructions

- [ ] 1) Pull the data from the [Wikipedia Recent Changes API](https://en.wikipedia.org/w/api.php?action=query&list=recentchanges&format=json&rcstart=2019-08-29T10:59:20Z&rcnamespace=0&rcshow=!minor%7C!bot%7C!anon%7C!redirect&rclimit=500&rcdir=newer).

    - Bonus: Use rcstart to fix the results so that reloading the page will only update to show results by hour. So if the browser time is 10:59:59, the system will only show data for 10:00 and earlier, and at 11:00:00, it will show data for 11:00:00 and earlier.

- [ ] 2) Build a user-interface to present this data. Paginate the data to 20 rows. 
    - Bonus: pagination size is user configurable. 
    - Bonus: Data sort or filtering options are provided in the interface.
    - Bonus: User interface element allows user to load all recent changes (ignoring rcstart limit above)

- [ ] 3) (Only if you have time but do this before the bonus tasks above) Build a second user-interface (could be part of above screen as a single page application) that allows the user to click on each article and display the more detailed Wikipedia article page. This page should be built using the Wikipedia API+json and not just (for example) an i-frame to the Wikipedia article page. 

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
