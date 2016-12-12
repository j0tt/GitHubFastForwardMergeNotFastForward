# GitHubFastForwardMergeNotFastForward
An example of how GitHub PR rebase and merge is not fast forward.


This repository has _never been_ force pushed.

The branch feature1 was created off of master, 3 commits were made: https://github.com/j0tt/GitHubFastForwardMergeNotFastForward/commits/feature1

A pull request to bring feature1 to master was created: https://github.com/j0tt/GitHubFastForwardMergeNotFastForward/pull/1

The pull request was accepted and merged to master via "Rebase and Merge" option. According to the github documentation, this should do a fast forward merge.

Notice the commit SHA's on feature1 and master are _different_. This should not be the case, if the merge was truely fast-forward, the rebase on master should have been an noop since the remote had not changed, and the merge should have been fast forward, _retaining_ the commit SHAs.