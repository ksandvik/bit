workflow 

git co -b new-branch

- use UI for diffs
- git add .
- git commit -m "asdf"

- git add .
- git commit -m "asdf"

- git add .
- git commit -m "asdf"


- git push


- git rebase -i AFDFLSDKJFSFDLKJ


- fill out form to squash everything 


- git rebase --continue


- git push -f 


- git pull -r origin master


- git push -f 


- git co master 


- git merge new-branch



- bit version new-branch (click y)
- bit save "asdf"  // git commit -am "asdf"
- bit save         // git commit -a --amend (needs to check if ahead of master somehow?)
- bit save
- bit sync (if ahead it will push; if behind it will rebase) (git pull -r; git push)
- bit sync origin master (git pull -r origin master)
- bit version master 
- bit merge new-branch
- bit push


- bit undo ???????
- bit sync origin master
- bit prepare-for master
- either bit switch or bit version


https://blog.carbonfive.com/always-squash-and-rebase-your-git-commits/

gitless 
branches are parallel universes. Staged changes should never be shared between them
commit/save tracked files by default 

https://spderosso.github.io/oopsla16.pdf

https://opensource.com/article/20/4/git-extras
https://devhints.io/git-extras


git-info, git-summary, git-effort

git-feature

git-release


--force-with-lease


git for-each-ref --sort=-committerdate refs/heads/ refs/remotes --format='%(authordate:short) %(authorname) %(color:red)%(objectname:short) %(color:yellow)%(refname:short)%(color:reset) (%(color:green)%(committerdate:relative)%(color:reset))'
--> use git merge-base to see if merged already

git difftool --tool=vimdiff --no-prompt

https://wiki.diasporafoundation.org/Git_workflow

tests
command completion
bash history
git-effort failing 
bit release bump
man page parsing + flag suggestions for all commands 


git log --pretty=format:"* [%s](https://github.com/chriswalz/bit/commit/%H)" 09facd30..HEAD

deleting tags from local and origin is painful

COMP_POINT=25 COMP_LINE="bit status" bitcomplete

apt-get install language-pack-es
locale -e
LC_ALL=es_MX.utf8 git status


https://github.com/chriswalz/bit/releases/download/v0.6.5/bit_0.6.5_Darwin_x86_64.tar.gz

https://github.com/chriswalz/bit/releases/v0.6.5/bit_0.6.5_Darwin_x86_64.tar.gz

bit release should have prepush and post push scripts

git-extras sync?

bit fix undo-commit
bit fix untrack-file
bit fix rename-commit
bit fix catch-up-to-branch

delete tag local and on origin

bit save -e 

combine bit & bitcomplete into one binary?

basic usage tracking

add bit --version suggestion (add global flag suggestions)
bit update not behaving with homebrew 

brew Symlink
already exists 
usr/local/bin/bit
symlink
realpath /usr/local/Cellar/bit-git/0.9.2


show recently edited files when checking out a branch
git log --name-status -10 path/to/dir

Getting tab completions from zsh
git st$'\t\t' | zsh -i

https://brbsix.github.io/2015/11/29/accessing-tab-completion-programmatically-in-bash/

use macrorecorder?


-[X] display descriptions for all available suggestions 
-[X] show common commands first 
-[X] when "-" display single dash flags 
-[X] flag filtering not working (e.g. bit push --all doesn't show "--all" suggestion)
-[X] "bit checkout -2 " doesn't display branches
-[X] bit co should suggest "commit" (currently displays nothing)
-[X] bit commit should suggest "commit" (currently displays nothing)
-[X] bit commit should suggest "commit" (currently displays nothing)
-[X] branches need to remain ordered
-[X] bit version && --version are missing
-[X] branches need to have descriptions again
-[X] reenable bit pr & have correct descriptions
-[] maps need to be ordered?
-[] "co" suggestion from generation tree needs to be disabled manually
-[] some descriptions are getting cut off // FIXME

-[X] "bit checkout -2 " is showing double dashes for branches
-[X] verify tab completions work
-[] use schlex 
