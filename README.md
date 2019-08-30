# Learning Tapestry Server-side Developer Test

This is a test project to assess a software developer's skills. This test is a form of [Kobayashi Maru scenario](https://en.wikipedia.org/wiki/Kobayashi_Maru). (Yes, some of us are dorks).

## Tips for passing this test

- Read this README carefully and come up with a plan to finish it as best as you can.
- Use simple frameworks instead of complicated ones.
- Ask us if you're unsure about something.
- Don't submit your project without tests. You won't have time to test everything, so choose what to test.
- It's better to accomplish only part of the project well, than to get partway done with everything.

## References

Refer to:
- [Credential Registry](http://www.credreg.net). Don't spend too much time understanding CR. It's a big OSS project.
  - Some quick start docs: [Basic walkthrough of using CR APIs](https://github.com/CredentialEngine/CredentialRegistry/blob/master/docs/02_ce-registry_walkthrough.md)

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

- [ ] 1) Pull the data from the [Staging CR API](https://staging.credentialengineregistry.org/envelopes).

    - The code that does this is a part of your app as well and written in the same language. It should be configurable and repeatable, and it's a good idea to write tests for it.

- [ ] 2) Normalize the data as best you can into a relational structure and store the data into a PostgreSQL database.

    - You should decode and normalize (as much as you have time for) the `resource` field, which contains base64 strings, encoded using [JWT](https://jwt.io/), that have JSON data inside. (Note you may find a shortcut to decoding the resource field, which is fine to use.)
    - Bonus: Validate that the JWT `resource` field was encoded by the public key provided in the envelope.

- [ ] 3) Expose the data via an API.

    - The API should have two methods:
        - `/resources`: Resource browser with pagination
        - `/resources_by_field`: groups resources by field names. Allows an `?[field_name]=` parameters that filter out records by the values of certain field names contained within the resource field (which you decoded and normalized in the step above). If the parameter is not present, aggregated values must be displayed anyway (e.g. use a default aggregation). We encourage you to use SQL as far as possible for this method.

          Example output:
          ```
          [{ "ceterms:agentType": "Business", "results": [ { /*... resource JSON ...*/ }, ...] }, ...]
          ```

- [ ] 4) Write a piece of code - an API client - that consumes your API and displays the returned data.

- [ ] 5) Write tests.

- [ ] 6) Provide some basic documentation on how to use your project.

- [ ] 7) Limit your effort to no more than 8 hours total.

- [ ] 8) Create a final report of what you were unable to accomplish, and how long you think it will take to complete.

- [ ] 9) Send us your repo in a [git bundle](https://git-scm.com/blog/2010/03/10/bundles.html).

### Ruby specific notes

- You can use a Rake task to invoke 5).

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

### Ruby specific notes

- We suggest following [bbatsov's style guide](https://github.com/bbatsov/ruby-style-guide)
