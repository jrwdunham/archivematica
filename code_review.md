Code review
===========

Every new feature and bugfix to a project is expected to go through code review before inclusion.
This applies both to developers at Artefactual and to outside contributors.

The contribution process in general is outlined in the [contributing document](CONTRIBUTING.md).
This provides a checklist and set of guidelines for what to do when doing code review.
It also helps set expectations for contributors about what to expect.

Checklist
---------

### Meta
- [ ] Have they submitted a signed contributor's agreement?
- [ ] Does this meet the requirements? Does it fix the bug?
- [ ] Is this feature useful to multiple users or potential users?
- [ ] Is there documentation?  This includes docstrings, comments & potentially user-facing documentation.
- [ ] Is the commit history clean?

### Architecture
- [ ] Does this duplicate functionality found elsewhere?
- [ ] Does it make more sense for this to be implemented elsewhere? E.g. Should this happen in the storage service vs a client script, or should a helper function live in archivematicaCommon?
- [ ] Does this add or reduce technical debt?
- [ ] Does this conflict with or benefit from work being done in parallel?
- [ ] Does this have security implications? Does it add or close a security vulnerability?
- [ ] Is there a more efficient way to do this? Is it significantly less readable?

### Style
- [ ] Does it follow [PEP8](https://www.python.org/dev/peps/pep-0008/) (code style)?
- [ ] Does it follow [PEP257](https://www.python.org/dev/peps/pep-0257/) (docstrings)?
- [ ] Do docstrings list the parameters and behaviour?
- [ ] Are the names accurate and sensible?
- [ ] Are there massive functions, classes or files? Can they be split?
- [ ] Are errors handled?  Is this consistent with similar code?

### Syntax:
- [ ] Is it Python 2.7 & Python 3 compatible?
- [ ] Are all user-facing strings marked for translation?

### Tests
- [ ] Are there tests?
- [ ] Do the tests cover all the new functionality or fixes?
- [ ] Do the tests handle error cases?
- [ ] Is unit testing or integration testing more appropriate?

### Doing
- [ ] Do I understand what this is supposed to solve?
- [ ] Have I checked out and run this code to verify it does what it says?
- [ ] Is someone else an expert in this area? Should I ask them to also review this?

More advice and suggestions can be found at https://www.kevinlondon.com/2015/05/05/code-review-best-practices.html
