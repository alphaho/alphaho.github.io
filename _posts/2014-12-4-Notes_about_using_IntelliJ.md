---
layout: post
title: Notes about using IntelliJ
---
Here's some notes about using intellij:

### 1. Get error "Package name does not correspond to the path"
May have opened the project at the wrong directory level. Try to open it at the subdirectory(the project/modules root).


### 2. Get error "Can't resolve symbol"
This is the most common error I have run into.  
I usually fix it by:  

* Set the jdk settings for the module   
  Project Structure -> Project Settings -> Modules -> select the modules one by one -> Dependencies Tab -> Module SDK set to a specific SDK rather than using "Project SDK"
* Build the project once using the command line tool  
  As the Build Tool integration in IntelliJ is not perfect, it would help sometime building the project using the command line. And this may solve the symbol after.
* Last option, google it.  
  There would be some cases that can not be solved by performing the above two steps. This may require us to dig a bit deeper.
      
  
  
### 3. Where to set the VM options
* In Windows:  
  JetBrains\IntellijIDEAXX\bin\idea.exe.vmoptions
  
* In Mac:  
  ~/Library/Preferences/IntelliJIdeaXX/idea.vmoptions
    


### 4. Some functions I find quite useful
You can search the following functions in the IntelliJ keymap settings and bind it a key

* Browse Type Hiererchy 
* Parameter Info
* Highlight Usage in Current File
* Find Usage
  There's a function "Call Hierarchy" which is quite handy sometimes.
    
  
### 5. To run Eclipse launch configuration
You may try to use the plugin Eclipser

