ruby-101
========
##Installing Ruby

###RVM or RBENV
```
curl -sSL https://get.rvm.io | bash -s stable
```
This gets the latest version of ruby  
To verify that it is installed check what version you are using by running 
```
ruby -v
```

###IRB

To open a Ruby console just type ```irb``` and thats it.

###.rvmrc files
Making a gemset for a project/directory is easy. Just 'cd' to the directory and make the .rvmrc file.
```
touch .rvmrc
```
Then edit that file 
```
nano .rvmrc
```
And fill in with something like this

```
rvm use 2.0.0@something --create
```
Chnge something to the project name to something else and optinally change the ruby version. Save and exit and then reload change back out and then into the directory again and you will be asked if you would like the create the gemset.

##Making a new Rails Application
To start with run 
```
gem install rails --no-ri --no-rdoc
```

This will download and install rails. 

To make a new application do

```
rails new something
```

Once again substitue something for your application name. Change into your new application folder and make a .rvrmc file like above


