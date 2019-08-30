# Learning Tapestry Front-end Developer Test

This is a test project to assess a software developer's skills. This test is a form of [Kobayashi Maru scenario](https://en.wikipedia.org/wiki/Kobayashi_Maru). (Yes, some of us are dorks).

## Tips for passing this test
Refer to [this list](https://github.com/learningtapestry/learning-tapestry-developer-test/blob/front-end/detailed-requirements.md#tips-for-passing-this-test) for advice on doing well on this test.

## References

Refer to: [Wikipedia API](https://www.mediawiki.org/wiki/API:Main_page)

## Requirements

Read and follow all the [detailed requirements for this project](https://github.com/learningtapestry/learning-tapestry-developer-test/blob/front-end/detailed-requirements.md#detailed-requirements)

## Notes

Additional [notes and information here](https://github.com/learningtapestry/learning-tapestry-developer-test/blob/front-end/detailed-requirements.md#notes).

## Instructions

- Create a React app with 2 pages:
  - An index page that pulls data from the [Wikipedia Recent Changes API](https://en.wikipedia.org/w/api.php?action=query&list=recentchanges&format=json&rcstart=2019-08-29T10:59:20Z&rcnamespace=0&rcshow=!minor%7C!bot%7C!anon%7C!redirect&rclimit=500&rcdir=newer)
      - The index page should paginate data 
  - A detail page that displays a specific article
     - The detail page should use API data and not just show an iframe to Wikipedia
     - Bonus: pagination parameters are user configurable
     - Bonus: Data sort or filtering options are provided in the interface.
     - Bonus: User interface element allows user to load all recent changes (ignoring rcstart limit above)
- Use whichever state-handling techniques you prefer
- The user should be able to navigate to the index or specific pages via distinct URLs (could be parameters or anchors)
- Write tests for as many aspects of the functionality as you have time for, and are needed. Prioritize integration tests that show the system is working correctly overall (but functional and unit level tests are welcome).


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
