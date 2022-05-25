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
<summary>3) Auto stage changes to the commit</summary>
<code>git commit -am 'commit message here' </code>
</details>

## Undoing

1) Remove last commit
2) Remove last commit along with the changes

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


## Merging
## Reverting
## Rebasing
## Conflict Handling
## Tagging
## Viewing History