ruby -v
ruby 2.4.0p0 (2016-12-24 revision 57164) [x86_64-linux]

rvm -v
rvm 1.29.2 (latest) by Michal Papis, Piotr Kuczynski, Wayne E. Seguin [https://rvm.io/]

gem install rails -v 5.1.4

rails -v
Rails 5.1.4

Update Gemfile

cd hello_app/
bundle install
bundle update

rails server
*c9 only*
rails s -b $IP -p $PORT
