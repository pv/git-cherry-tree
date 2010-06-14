git-cherry-tree
===============

Find commits not merged in the current branch.

Same as ``git-cherry``, but (optionally) consider only patches touching given
subdirs, and try hard to check if the patch was actually applied.  Has also
extra features for interactive picking of a patch sequence.

Examples::

  Which patches are in master branch, but not in the current one
  $ git cherry-tree master

  Which patches are in master branch, in directory `spam`, but not in current
  $ git cherry-tree master -- spam

  Interactively cherry-pick missing patches in `spam` directory
  $ git cherry-tree -pix master -- spam

