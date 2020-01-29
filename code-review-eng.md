## A few steps, for improving a code review process

### What is a code review?
**Before getting started, I want to give my definition of a code review::**
- Code review is a discussion about the new code. It's necessary to involve the team in assessing the importance of this change.
- Code review is sharing knowledge about a project because it can reduce a bus factor. In cases, when developers don't know how works some modules, code review can fix this omission.
- Code review is a refactoring, improving code quality.
- Code review is finding logical mistakes because autotests can miss those errors.
- Code review is a way to integrate a culture of mentoring and mutual assistance in a team.

**And...**
- Code review is not checking a code style - it can be automated with linters.
- Code review is not checking a auto-tests is passing - it can be automated and should be automated.

### Primary steps before making Pull Request (PR):
1. Before making PR, it would be nice to look at the code as if the code was written by your colleague, not you. This will allow you to clarify points that are obvious to you, but not clear to the reviewer.
2. When it's possible, give a brief for PR: what has been changed, pay attention to what(?). This will provide a context for the reviewer, which the author possesses: the author investigated the problem, and knows the reasons for the changes.

### Improving a code review process: 
- Your PR delivers only one feature at a time. 
- Choose a better time for a code review. In a morning time reviewers less overloaded and not in a hurry to go home as soon as possible.
- Create basic checklist for checking a PR, e.g:
  - Autotests were written logically, there may be tests that pass in 100% of cases.
  - No code reuse: as the project grows, the likelihood of violating the DRY principle increases.
  - Documentation updated, if necessary.
  - Performance test: some language constructs may work more slowly, and can be rewritten in advance for a faster option.

### Emotional aspects of feedback:
- Avoid imperative forms in words; ask leading questions, for example, ask “why did you decide to write like that?” and suggest solutions, preferably with code examples.
- comment a code, not an author: “there is not enough test” instead of “you forgot to write a test”
