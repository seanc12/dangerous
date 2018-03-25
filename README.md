
     ,-----.,--.                  ,--. ,---.   ,--.,------.  ,------.
    '  .--./|  | ,---. ,--.,--. ,-|  || o   \  |  ||  .-.  \ |  .---'
    |  |    |  || .-. ||  ||  |' .-. |`..'  |  |  ||  |  \  :|  `--, 
    '  '--'\|  |' '-' ''  ''  '\ `-' | .'  /   |  ||  '--'  /|  `---.
     `-----'`--' `---'  `----'  `---'  `--'    `--'`-------' `------'
    ----------------------------------------------------------------- 


Hi there! Welcome to Cloud9 IDE!

To get you started, create some files, play with the terminal,
or visit http://docs.c9.io for our documentation.
If you want, you can also go watch some training videos at
http://www.youtube.com/user/c9ide.

Happy coding!
The Cloud9 IDE team

c9 Blank Ubuntu

http://conqueringthecommandline.com/book/basics
Learn enough Command Line


pwd
pwd -P
ls
ls /usr/local/
ls -a
ls -l
ls -lh
ls -lhS
ls -lt
ls -lr

create a.txt "Hello World"
ln a.txt b.txt
rm a.txt
ls -l
ln a.txt b.txt
ln -f a.txt b.txt
ln -s a.txt b.txt

mkdir foo
cd foo
mkdir -p a/b/c
ls -la a/b/c
mkdir -v a
cp a.txt b.txt
cp a.txt b.txt foo
cp *.txt foo
a.txt -> b.txt
cp foo bar
cp -Rv foo bar

cp a.txt b.txt
cp -i a.txt b.txt

rm -v a.txt

***   Local Computer Only (does not work w/c9 virtual box)

ALWAYS USE VPN

https://www.digitalocean.com/community/tutorials/how-to-install-and-use-ack-a-grep-replacement-for-developers-on-ubuntu-14-04

sudo apt-get update
sudo apt-get install ack-grep
sudo apt install silversearcher-ag

ack /path/to/python
ag /path/to/python
ag DHH
ag DHH guides/
ag readme$
ag .rb railties/CHANGELOG.md
ag -Q .rb railties/CHANGELOG.md
ag readme -l -i -G ec
ag readme -l -i -G ec$

apt-get update

***   Back to C9 seanc12:~/workspace
ag DHH -l
ag readme -l
ag readme -l -i

***   Fun Stuff

sudo apt-get install curl
curl quiet-waters-1228.herokuapp.com/hello
curl -i quiet-waters-1228.herokuapp.com/hello

curl -o my_image.jpg http://quiet-waters-1228.herokuapp.com/assets/image.jpg
curl -X POST quiet-waters-1228.herokuapp.com/echo
curl -X PUT quiet-waters-1228.herokuapp.com/echo
curl -X POST -d "fname=Mark&lname=Bates" quiet-waters-1228.herokuapp.com/echo
curl -X POST -d @form_data.json quiet-waters-1228.herokuapp.com/echo

curl -X POST -F user[fname]=Mark -F user[lname]=Bates -F foo=bar \
  quiet-waters-1228.herokuapp.com/echo -H "Accept: application/json"
  
curl -X POST -d @form_data.json quiet-waters-1228.herokuapp.com/echo \
  -H "Accept: application/json"

curl -X POST -d @form_data.json quiet-waters-1228.herokuapp.com/echo \
  -H "Accept: application/json" -H "X-Auth: 1234567890"
  
curl -i -X POST quiet-waters-1228.herokuapp.com/login
curl -X POST -u "user1:password1" quiet-waters-1228.herokuapp.com/login
curl -i quiet-waters-1228.herokuapp.com/whoami
curl -i -u "user1:password1" quiet-waters-1228.herokuapp.com/whoami

curl -X POST -D headers -u "user1:password1" \
  quiet-waters-1228.herokuapp.com/login
  
curl -X POST --dump-header headers -u "user1:password1" \
  quiet-waters-1228.herokuapp.com/login
  
curl -b headers quiet-waters-1228.herokuapp.com/whoami

curl -X POST -c cookies.txt -u "user1:password1" \
  quiet-waters-1228.herokuapp.com/login

curl -b cookies.txt quiet-waters-1228.herokuapp.com/whoami






https://www.learnenough.com/git-tutorial
Learn Enough GIT

wget https://softcover.s3.amazonaws.com/636/ruby_on_rails_tutorial_4th_edition/images/figures/tech_support_cheat_sheet.png

which git

git config --global user.name "seanc12"
git config --global user.email sean.cox.or@gmail.com

mkdir -p repos/website

git add -A (or) 

wget https://softcover.s3.amazonaws.com/636/learn_enough_git/images/figures/git_status_sequence.png

cd repos/website
touch index.html

git add .
git commit -m "initial commit"
git log

echo "hello, world" > index.html
git diff




