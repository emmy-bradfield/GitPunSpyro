# GitPun Challenge: Team Spyro
New repo made to fix the old one

Code (as sent in chat) is also below for getting back up-to-date

1. Visit https://github.com/emmy-bradfield/GitPunSpyro
2. Press the 'fork' button to fork to your repos
3. Open your bash terminal/VSC/etc
4. use cd <path> to get to the file you wish to clone the repo into
5. Enter the following commands:

#

git clone git@github.com:<your-username>/GitPunSpyro.git

#

or just click "code" > "SSH" > "copy to clipboard" on your forked repo and paste the url

#

cd GitPunSpyro


git init

#

this step can be skipped, I personally always do it because it confirms the directory has been
initialised for git and that I am in fact in a git repo - I tend to goof and end up in the wrong place a lot
but if you don't do this then don't worry xD

#

git branch

#

confirm the branches there are - there may be a dev one already forked from my repo
if there is a dev branch, skip this step and jump to after the next "# comment"

#

git checkout -b dev


git push --set-upstream origin dev

#

if there is a dev branch, go from here. if there wasn't, there now is, so carry on as usual
for the below, [x] just represents your initial

#

git checkout -b feature-[x]1


echo "[your pun]" > [file-name].txt


git add .


git commit -m "added [file-name].txt"


echo "pointless file" > pointless-file.txt


git add .


git commit -m "added pointless-file.txt"


git log --oneline

#

this is just to confirm both the commits have happened, on the right branch, and all is okay

#

git revert HEAD

#

for Shahmeen -> an online guide suggests that pressing <esc> twice then 'O' will save the name, and
then <esc> twice and 'X' (or just <F12>) should save the name and close it on Mac. Apologies,
a guide was hard to find, but seeing as you figured it out lasting time I'm hoping you remember? Sorry!

#

git push --set-upstream origin feature-[x]1


git checkout dev


git checkout -b feature-[x]2


touch [file-name].txt


git add .


git commit -m "added [file-name].txt"


echo "[second pun]" > [file-name].txt


git add .


git commit -m "updated [file-name].txt"


git push --set-upstream origin feature-[x]2


git checkout dev

#

from here, you can step away from the bash terminal and open your GitHub account. We will go
through it all together as it's easier. Honestly, it's stupidly easy to mess up the next bit, the only reason
I even caught it so easily is because I'm the PO so it shows up on mine what's happened. However,
all the files should be added, the branches pushed, and we're now ready to go through the pull
requests together. This is probably good to do together as it means we can make sure everyone
is happy with it, and also I know it's a bit iffy because:
1) GitHub defaults are set up to skip a few steps that we have to do. Normally, you wouldn't need
to do these extra steps but we do for the challenge
2) My default name for the primary branch is "master" because I changed it on GitHub - by default
it is "main" and I imagine you guys' branches are called "main" so I wanna make sure it doesn't
end up causing an issue. If it is a problem, I'll need to go temporarily change mine so if we go through
it together I can check if I'll need to and do that, rather than waiting and seeing it's all a bit goofed
