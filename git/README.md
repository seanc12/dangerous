https://www.learnenough.com/git-tutorial
Learn Enough GIT

wget https://softcover.s3.amazonaws.com/636/ruby_on_rails_tutorial_4th_edition/images/figures/tech_support_cheat_sheet.png

which git

git config --global user.name "seanc12"
git config --global user.email sean.cox.or@gmail.com

mkdir -p repos/website

git add .

wget https://softcover.s3.amazonaws.com/636/learn_enough_git/images/figures/git_status_sequence.png

cd repos/website
touch index.html

git add .
git commit -m "initial commit"
git log

echo "hello, world" > index.html
git diff

git add .
git commit -m "add content to repos/website/index.html"

index.html
<h1>hello, world</h1>