# How to solve: vs code interactive windows slow too slow  

Essentially put this in your python.dataScience.runStartupCommands in setting.json

%config IPCompleter.use_jedi = False

ref: https://github.com/microsoft/vscode-python/issues/8171


# Setup Environment variables on windows 10 before install R and R studio  
U_USER C:\Lib  
R_USER_USER C:\Lib\R  

# Editing dcast multipe value.var column  

> require(reshape2); require(data.table)    
> names(airquality) <- tolower(names(airquality))    
> aqm <- melt(airquality, id=c("month", "day"), na.rm=TRUE)    
> dcast(as.data.table(aqm), month + day ~ variable, value.var = c('value', 'value2'))    
