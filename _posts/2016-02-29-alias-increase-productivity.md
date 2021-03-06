---
layout: post
title: Be more productive in your day, save time
excerpt: "Using aliases to increase productivity."
tags: [productivity, alias, terminal]
modified: 2016-02-29
comments: true
---

The time is complicated. We can not stop the time, homever we can use in a better way to be more productive. The focus idea is to think that we can always improve how we perform our tasks.
This concept can be applied to any field of everyday life, today I'll give you an example of how to automate repetitive tasks that run in my terminal.


### The objective

The aim of this method is use the least amount of time to perform the tasks, so every second counts. In addition to saving time with this method we avoid typing errors.

### The trigger

The trigger post comes from the need of a teammate.I thought, 

>I can teach you how to configure the alias but this way only you would be benefited. 

So I decided to write a mini tutorial so everyone can see benefit from this tool and even better they can be self-sufficient.

### The method

The example I'll use is related to commands that I use daily in my terminal.
I set the `.zshrc` alias file, this file is generated by the [ZSH](http://ohmyz.sh/) shell. You can install this shell from here http://ohmyz.sh/, personally I recommend.[ZSH](http://ohmyz.sh/)  already provides functions, helpers and many other things that just make me and you more productive.
However, it is not necessary to install ZSH, if so you can use your configuration file, as example `.bashrc` that will be in your HOME directory.

Open your config file with your favorite text editor. In my case i have an alias to open it so here are the two alternatives that i use:

##### With alias:

{% highlight bash %}
cbs
{% endhighlight %}

The meaning of this is "Config Bash Sublime"

##### Without alias:

{% highlight bash %}
subl .zshrc
{% endhighlight %}

Remember you need located in your HOME directory.
Now you have to add the following code to the file, I will provide you three examples.

- git status

{% highlight bash %}
alias gs='git status'
{% endhighlight %}

- git pull -  -rebase origin master

{% highlight bash %}
alias gprm='git pull --rebase origin master'
{% endhighlight %}

- Config bash sublime

{% highlight bash %}
alias cbs='subl /Home/Directory/.zshrc'
{% endhighlight %}

After you have added the files you have to do is reload your configuration file by running the following command:

{% highlight bash %}
. ~/.bashrc
{% endhighlight %}



We are now ready to use the alias so that when you run gs receive the status of the repository without typing the entire command.
I hope it is useful and can extend your creativity with this simple but powerful functionality.