# Pario RFCs

Many changes, including bug fixes and documentation improvements can be
implemented and reviewed via the normal GitHub pull request workflow.

Some changes though are "substantial", and we ask that these be put
through a bit of a design process and produce a consensus among the Crvsh 
team.

The "RFC" (request for comments) process is intended to provide a
consistent and controlled path for new features to enter the project.

[Active RFC List](https://github.com/crvshlab/pario-software-factory-rfcs/pulls)

Pario is still **actively developing** this process, and it will still change as
more features are implemented.

## When to follow this process

You should consider using this process if you intend to make "substantial"
changes to the Pario way of working or its 'documentation'. Some examples that would benefit
from an RFC are:

   - A new feature that creates new API surface area, and would
     require a feature flag if introduced.
   - The removal of features that already shipped as part of the release
     channel.
   - The introduction of new idiomatic usage or conventions, even if they
     do not include code changes.

The RFC process is a great opportunity to get more eyeballs on your proposal
before it becomes a part of a released version of Pario. Quite often, even
proposals that seem "obvious" can be significantly improved once a wider
group of interested people have a chance to weigh in.

The RFC process can also be helpful to encourage discussions about a proposed
feature as it is being designed, and incorporate important constraints into
the design while it's easier to change, before the design has been fully
implemented.

Some changes do not require an RFC:

  - Rephrasing, reorganizing or refactoring
  - Addition or removal of warnings
  - Additions that strictly improve objective, numerical quality criteria (e.g. speedup)
  - Additions only likely to be _noticed by_ other implementors, invisible to users.
