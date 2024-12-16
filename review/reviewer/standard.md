# The Standard of Code Review

## The Standard

The primary purpose of code review is to make sure that the overall code quality of Grata's code base is improving over time. The senior principle among all of the code review guidelines is:

Reviewers should approve a PR once it:

* Definitely improves overall code quality, even if the PR isn't perfect.

* Is free from major defects that could cause outages or bugs.

There are limitations to this principle, of course. For example, if a PR adds a feature that the reviewer doesn't want in their system, then the reviewer can certainly deny approval even if the code is well-designed. Nothing in this document justifies checking in PRs that definitely worsen the overall code quality of the system. The only time you would do that would be in an emergency.

A key point here is that there is no such thing as "perfect" code—there is only better code. Reviewers should not require the author to polish every tiny piece of a PR before granting approval. Rather, the reviewer should balance out the need to make forward progress compared to the importance of the changes they are suggesting. Instead of seeking perfection, what a reviewer should seek is continuous improvement. A PR that, as a whole, improves the maintainability, readability, and understandability of the system shouldn't be delayed for days or weeks because it isn't "perfect."

In defining this principle, we’re balancing two concerns:

Developers must be able to make progress on their tasks. If you’re never able to contribute, the codebase never improves. If a reviewer makes it very difficult for any change to be made, developers will be unlikely to make improvements in the future.

On the other hand, it is the duty of the reviewer to make sure that each PR maintains or increases the overall code quality of the codebase. This can be tricky! Codebases often degrade through small decreases in code quality over time, especially when a team is under significant time constraints and they feel that they have to take shortcuts in order to accomplish their goals.

Also, a reviewer has ownership and responsibility over the code they are reviewing. They want to ensure that the codebase stays consistent, maintainable, etc.

## Principles

    Both the author and the reviewer share responsibility for the code that is merged.

    Assume best intent, and rest assured that the other party will as well. Do not be afraid to leave a lot of comments or to raise serious concerns.

    If no other rule applies, then the reviewer may ask the author to be consistent with what is in the current codebase, as long as that doesn't worsen the overall code quality of the system.

## Nitpicks

Always feel free to mention when you think something could be better. If you have a comment that is purely educational, or otherwise not a big deal, preface it with “Nitpick: “ or “Nit: “. These comments can be safely ignored.

## Resolving Conflicts

In any conflict on a code review, the first step should always be for the developer and reviewer to try to come to consensus.

When coming to consensus becomes especially difficult, it can help to have a face-to-face meeting or a video conference between the reviewer and the author, instead of just trying to resolve the conflict through code review comments. (If you do this, though, make sure to record the results of the discussion as a comment on the PL, for future readers.)

If that doesn't resolve the situation, the most common way to resolve it would be to escalate. Often the escalation path is to a broader team discussion, having a Technical Lead weigh in, asking for a decision from a maintainer of the code, or asking an Eng Manager to help out. Don't let a PR sit around because the author and the reviewer can't come to an agreement.
