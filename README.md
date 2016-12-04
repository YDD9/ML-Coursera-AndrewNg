machine-learning-coursera
=========================

This repo is specially created for all the work done my me as a part of Coursera's Machine Learning Course.


:boom: **git hub initialization commands**
[http://dont-be-afraid-to-commit.readthedocs.io/en/latest/git/commandlinegit.html](git commit link)
echo "# ML-Coursera-AndrewNg" >> README.md
```
git init
git add README.md
git commit -m "first commit"
git remote add origin https://github.com/YDD9/ML-Coursera-AndrewNg.git
git push -u origin master
```


:boom: **Installing octave via MAC software management tool homebrew**
[http://jatinganhotra.com/blog/2014/01/21/installing-octave-on-os-x-10-dot-9-mavericks/]
brew installation path:
/usr/local/Cellar/octave
symlink path:
/urs/local/bin


:boom: **octave startup config file path:**
/usr/local/Cellar/octave/4.2.0/share/octave/site/m/startup
accept all octave command
[https://www.gnu.org/software/octave/doc/v4.0.0/Startup-Files.html]


:boom: **Issues of plot frozen and wrong terminal error, add following into the config**
```
graphics_toolkit('gnuplot');
setenv('GNUTERM','qt');
```
[http://stackoverflow.com/questions/32086405/warning-plotting-with-an-unknown-terminal-no-output-will-be-generated-pleas]
or `setenv('GNUTERM','X11');` depending on your gnuplot list

if can be verified inside octave-cli with command:
```
available_graphics_toolkits;
loaded_graphics_toolkits;
```
