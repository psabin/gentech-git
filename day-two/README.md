# Day 2 - 98% usecase of Git

We will be doing git exercises today. There are multiple exercises listed for each section. 

Recommended approach to do the exercise is reading man page for each git command. Google for answer as last resort.

## Cloning (`git-clone`)

Download a copy of remote repository in a new directory.

<details>
<summary>1) Clone a repo</summary>
<code>git clone &lt;repository&gt;</code>
</details>

<details>
<summary>2) Clone repo with "gentech" directory</summary>
<code>git clone &lt;repository&gt; gentech </code>
</details>

<details>
<summary>3) Clone only 1 branch</summary>
<code>git clone &lt;repository&gt; --single-branch &lt;branch&gt; </code>
</details>

<details>
<summary>4) Shallow clone last commit</summary>
<code>git clone &lt;repository&gt; --depth 1 </code>
</details>

## Branching (`git-branch`)

Create a separate working tree for set of changes

<details>
<summary>1) Create a branch</summary>
<code>git branch &lt;branch&gt; </code>
</details>

<details>
<summary>2) List local branches</summary>
<code>git branch </code>
</details>

<details>
<summary>3) List remote branches</summary>
<code>git branch --remotes </code>
</details>

<details>
<summary>4) Delete local branch</summary>
<code>git branch --delete test </code>
</details>

<details>
<summary>5) Rename branch</summary>
<code>git branch -m &lt;old branch&gt; &lt;new branch&gt; </code>
</details>

Related: do look into `git-checkout` and `git-switch` too.

## Staging (`git-add`)

Take changes from working tree to Staging area

<details>
<summary>1) Stage all changes</summary>
<code>git add . </code>
</details>

<details>
<summary>2) Stage only 1 file</summary>
<code>git add path/to/file </code>
</details>

<details>
<summary>3) Interactive stage 1 file</summary>
<code>git add --interactive </code>
</details>

Related: how to unstage staged files? see `git-restore`

## Reverting (`git-revert`)

Reverse the commit

<details>
<summary>1) Revert last commit</summary>
<code>git revert HEAD </code>
</details>

<details>
<summary>2) Revert 4th commit</summary>
<code>git revert &lt;4th commit hash&gt; </code>
</details>

## Commiting (`git-commit`)

Record changes 

<details>
<summary>1) Add a commit</summary>
<code>git commit -m 'commit message here' </code>
</details>

<details>
<summary>2) Change that commit message</summary>
<code>git commit --amend </code>
</details>

<details>
<summary>3) Add new changes to last commit</summary>
<code>git commit --amend --no-edit </code>
</details>

<details>
<summary>3) Auto stage changes and commit</summary>
<code>git commit -am 'commit message here' </code>
</details>

## Undoing (`git-reset`)


<details>
<summary>1) Remove last commit</summary>
<code>git reset HEAD~ --hard</code>
</details>

<details>
<summary>2) Remove last commit along with the changes</summary>
<code>git reset HEAD~ --soft</code>
</details>

## Checking Status (`git-status`)

Status of working tree 

1) Check how many files are staged or unstaged
## Pushing (`git-push`)

Distribute the changes without everyone

<details>
<summary>1) Push a change into a branch</summary>
<code>git push</code>
</details>

<details>
<summary>2) Push changes in freshly created branch</summary>
<code>git push -u origin &lt;branch&gt;  </code>
</details>

<details>
<summary>3) Push tags</summary>
<code>git push origin --tags </code>
</details>

<details>
<summary>4) Delete remote branch that is longer in local</summary>
<code>git push --prune </code>
</details>

<details>
<summary>5) Delete a branch in remote</summary>
<code>git push origin :&lt;branch&gt; </code>
</details>

## Viewing History (`git-log`)

View history of all the commits

<details>
<summary>1) View number of commits by author</summary>
<code>git shortlog -s</code>
</details>

<details>
<summary>2) View commit log in oneline </summary>
<code>git log --oneline  </code>
</details>

<details>
<summary>3) View commit log between ranges</summary>
<code>git log &lt;newer commit hash&gt;...&lt;older commit hash&gt; </code>
</details>

<details>
<summary>4) View commit log with only 1 commit per branch</summary>
<code>git log --first-parent  </code>
</details>

Related: Do check `git-reflog` too

## Merging
## Rebasing
## Conflict Handling
## Tagging