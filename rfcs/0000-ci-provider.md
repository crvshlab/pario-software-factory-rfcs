- Name of suggestion: ci_provider
- Start Date: 2020-03-23(fill me in with today's date, YYYY-MM-DD)
- RFC PR: 
- PSF Issue: 

# Summary
[summary]: #summary

Github actions as the pipeline to use for continuous integration.

# Motivation
[example]: #motiviation

We need to setup a continuous integration pipeline for us to be in a position to
confidently develop and deploy our services for the backoffice portal.

The expected outcome is to have a continuous integration pipeline that can build, test and integrate any code changes. This is to ensure that the code can be updated confidently multiple times a day and tested for regressions frequently.

The solution should be as simple to maintain as possible and have the ability to run custom scripts to allow various testing and deployment strategies to meet any changing needs we cross during development.

The outcome of these changes should be a setup Github actions pipeline that is ready for 
building, testing and deploying code with new changes.

# Detailed explanation
[explanation]: #explanation

I propose that we use Github actions as the chosen pipeline stack for our CI.

We want to be able to run custom scripts, in this sense both Github actions and Gitlab pipelines allow this. 


The reasons for this choice: 
- It is close to the source and documentation.
- It reduces the number of different licenses we work with.
- It has all the modern features that we require.(including )
- It has a strong backing of a company with a proven track record.

# Drawbacks
[drawbacks]: #drawbacks

- We don't get to leverage the knowledge of Vodafone staff that are more experienced in Gitlab pipelines.
- We are buying into Githubs still unproven CI offering.
- New CI pipeline will require training for use.

# Alternatives
[alternatives]: #alternatives

Gitlab pipelines and Github Actions are almost identical. We need to decided between the new offering or the currently in use offering.

Alternatives:
- Gitlab pipelines
- CircleCI

# Adoption strategy
[adoption]: #adoption


The adoption of Github actions would have no impact on existing work efforts in the Pario team, namely documentation.

The documentation linked in the next section includes a wealth of knowledge about using Github actions and should be sufficiently detailed to adopt it as our CI tool of choice.

None of the existing Vodafone teams should need to adopt it. It can be used in isolation by the Pario team, at least for the immediate future.

# How we teach this
[adoption]: #adoption
We could just use official documentation and existing online resources.

https://github.com/features/actions

# Unresolved questions
[unresolved-questions]: #unresolved-questions

- What security concerns are there in using a new CI tool rather than the pre-existing Gitlab tools?

- Does Vodafone apply business restrictions to what tools we can use and that have access to any resources within Vodafone that we might need?

# Future possibilities
[future-possibilities]: #future-possibilities

It is important to understand that many CI tools today are very similar in their feature sets and that making a decision in this regard should not take long.
The simplest Build, Test, Deploy ability should be sufficient for our needs and both tools provide this.

The question is more:
Do we want to use a tool with closer ties to our code? or do we want to have people with more experience there to provide support?
