# .github

Used for certain git default files for any repository that do not have a copy of those files. (Note: this repository has to be kept public)


> GitHub will use and display default files for any repository owned by the account that does not have its own file of that type in any of the following places:
> 
> * the root of the repository
> * the .github folder
> * the docs folder

For more details, [See the github documentation](https://docs.github.com/en/communities/setting-up-your-project-for-healthy-contributions/creating-a-default-community-health-file).


## .github/delete-merged-branch-config.yml
We are using it for the default configuration of [delete-merge-branch app](https://github.com/apps/delete-merged-branch/), used to auto-delete our branch after merge. Use it to add any branch that should never be deleted.

Here is an example usage:

```
exclude:
    - master
    - staging
    - production
    - release*
delete_closed_pr: false
```
