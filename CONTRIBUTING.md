## Contribution Guidelines

### Pull requests are always welcome

We are always thrilled to receive pull requests, and do our best to
process them as fast as possible. Not sure if that typo is worth a pull
request? Do it! We will appreciate it.

If your pull request is not accepted on the first try, don't be
discouraged! If there's a problem with the implementation, hopefully you
received feedback on what to improve.

We're trying very hard to keep the project lean and focused. We don't want it
to do everything for everybody. This means that we might decide against
incorporating a new feature.


### Clear Communications

To ensure that communications happen smoothly, openly and free from suspicion
of malice, particular behaviors of involvement can be distracting.

Taking from the [section on interference with organizations](https://www.cia.gov/news-information/featured-story-archive/2012-featured-story-archive/CleanedUOSSSimpleSabotage_sm.pdf),
the following points are *NOT* beneficial to making progress.

> 1. Insist on doing everything through "channels."
>    Never permit short-cuts to be taken in order to expedite decision.
> 2. Make "speeches."
>    Talk as frequently as possible and at great length.
>    Illustrate you "points" by long anecdotes and accounts of personal experiences.
>    Never hestitate to make a few appropriate "patriotic" comments.
> 3. When possible, refer all matters to committees, for "furth study and consideration."
>    Attempt to make the committees as large as possible -- never less than five.
> 4. Bring up irrelevant issues as frequently as possible.
> 5. Haggle over precise wordings of communications, minutes and resolutions.
> 6. Refer back to matters decided upon at the last meeting and attempt to re-open the question of the advisability of that decision.
> 7. Advocate "caution."
>    Be "reasonable" and urge your fellow-conferees to be "reasonable" and avoid haste which might result in embarrassments or difficulties later on.
> 8. Be worried about the propriety of any decision -- raise the question of whether such action as is contemplated lies within the jurisdiction of the group or whether it might conflict with the policy of some higher echelon.

While these items are vague, the direct counter to such interference is largely to keep communications on topic, clear, and objective.

### Conventions

Fork the repo and make changes on your fork in a feature branch:

- If it's a bugfix branch, name it XXX-something where XXX is the number of the
  issue
- If it's a feature branch, create an enhancement issue to announce your
  intentions, and name it XXX-something where XXX is the number of the issue.

Small changes or changes that have been discussed on the project mailing list
may be submitted without a leader issue, in which case you are free to name
your branch however you like.

If the project has a test suite, submit unit tests for your changes. Take a
look at existing tests for inspiration. Run the full test suite on your branch
before submitting a pull request.

Update the documentation when creating or modifying features. Test
your documentation changes for clarity, concision, and correctness, as
well as a clean documentation build. See ``docs/README.md`` for more
information on building the docs and how docs get released.

Write clean code. Universally formatted code promotes ease of writing, reading,
and maintenance. Always run `gofmt -s -w file.go` on each changed file before
committing your changes. Most editors have plugins that do this automatically.

Pull requests descriptions should be as clear as possible and include a
reference to all the issues that they address.

Commit messages must start with a capitalized and short summary
written in the imperative, followed by an optional, more detailed
explanatory text which is separated from the summary by an empty line.

Code review comments may be added to your pull request. Discuss, then make the
suggested modifications and push additional commits to your feature branch. Be
sure to post a comment after pushing. The new commits will show up in the pull
request automatically, but the reviewers will not be notified unless you
comment.

Before the pull request is merged, make sure that you squash your commits into
logical units of work using `git rebase -i` and `git push -f`. After every
commit the test suite (if any) should be passing. Include documentation changes
in the same commit so that a revert would remove all traces of the feature or
fix.

Commits that fix or close an issue should include a reference like `Closes #XXX`
or `Fixes #XXX`, which will automatically close the issue when merged.

### Sign your work

The sign-off is a simple line at the end of the explanation for the
patch, which certifies that you wrote it or otherwise have the right to
pass it on as an open-source patch.  The rules are pretty simple: if you
can certify the below (from
[developercertificate.org](http://developercertificate.org/)):

```
Developer Certificate of Origin
Version 1.1

Copyright (C) 2004, 2006 The Linux Foundation and its contributors.
660 York Street, Suite 102,
San Francisco, CA 94110 USA

Everyone is permitted to copy and distribute verbatim copies of this
license document, but changing it is not allowed.


Developer's Certificate of Origin 1.1

By making a contribution to this project, I certify that:

(a) The contribution was created in whole or in part by me and I
    have the right to submit it under the open source license
    indicated in the file; or

(b) The contribution is based upon previous work that, to the best
    of my knowledge, is covered under an appropriate open source
    license and I have the right under that license to submit that
    work with modifications, whether created in whole or in part
    by me, under the same open source license (unless I am
    permitted to submit under a different license), as indicated
    in the file; or

(c) The contribution was provided directly to me by some other
    person who certified (a), (b) or (c) and I have not modified
    it.

(d) I understand and agree that this project and the contribution
    are public and that a record of the contribution (including all
    personal information I submit with it, including my sign-off) is
    maintained indefinitely and may be redistributed consistent with
    this project or the open source license(s) involved.
```

then you just add a line to every git commit message:

    Signed-off-by: Joe Smith <joe@gmail.com>

using your real name (sorry, no pseudonyms or anonymous contributions.)

You can add the sign off when creating the git commit via `git commit -s`.
