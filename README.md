machine-learning-coursera
=========================

This repo is specially created for all the work done my me as a part of Coursera's Machine Learning Course.


:boom: **git hub initialization commands**
[git commands for beginners](http://dont-be-afraid-to-commit.readthedocs.io/en/latest/git/commandlinegit.html)
```
git init
git add README.md
git commit -m "first commit"
git remote add origin https://github.com/YDD9/ML-Coursera-AndrewNg.git
git push -u origin master
```


:boom: **Installing octave via MAC software management tool homebrew**
[how to intall octave with homebrew ](http://jatinganhotra.com/blog/2014/01/21/installing-octave-on-os-x-10-dot-9-mavericks/)
brew installation path:
/usr/local/Cellar/octave
symlink path:
/urs/local/bin


:boom: **octave startup config file: octaverc**
/usr/local/Cellar/octave/4.2.0/share/octave/site/m/startup/octaverc
the config file accepts all octave command
[Details of the config file](https://www.gnu.org/software/octave/doc/v4.0.0/Startup-Files.html)


:boom: **Issues of plot frozen and wrong terminal error, add following into the config**
```
graphics_toolkit('gnuplot');
setenv('GNUTERM','qt');
```
[Issue description and solution](http://stackoverflow.com/questions/32086405/warning-plotting-with-an-unknown-terminal-no-output-will-be-generated-pleas)
depending on your env list, you may need to use `setenv('GNUTERM','X11');` instead of 'qt'

Above setting can be verified:
first open terminal and enter `octave-cli` to activate octave interface then
```
available_graphics_toolkits;
loaded_graphics_toolkits;
```
