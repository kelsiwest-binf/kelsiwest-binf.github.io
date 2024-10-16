---
layout: post
title: "Installing Python 3.12 On Mac M3 Pro"
date: 2024-09-14
description: Setting up my new computer with a (some would say) much needed upgrade.
---

<p class="intro"><span class="dropcap">I</span> recently purchased a new laptop to help with my education and coding endeavors during my "down time" aka laid off from a tech company. So today, I'm starting the process of installing or updating some of my favorite tools, one of which will be Python (version 3.12).🐍</p>

We're starting from the *very* beginning here.👩🏼‍🔧 But you have to start somewhere! The goal is to get my personal laptop to have all the tools, pipelines, and repositories like I had on my previous work laptop.

---
### Tutorial Roundup
The tutorial I'll be following is from GeeksforGeeks. It is written by a contributor, naveenarora. 
Find the tutorial [HERE](https://www.geeksforgeeks.org/how-to-download-and-install-python-latest-version-on-macos-mac-os-x/).
<br />
---

To avoid redundancy, I've only shown my code and copied any instructions that I had issues with or commented on.

#### Anything marked with 🐄Hold Up🐄 is where I had issues or went a little bit off the path of instructions.
#### Anything marked with 🤠Tidbits🤠 is helpful info I found out along the way.

Here goes nothing!
<br />

## Installing Python on Mac M3 Pro, macOS Sonoma v14.4

### 1. Open up terminal:
{%- highlight ruby -%}
Kelsis-MacBook-Pro ~ %
{%- endhighlight -%}

#### 🤠Tidbits🤠
`Kelsis-MacBook-Pro` is the name of my computer. Your name will be different!
<br />
<br />

### 2. Start bash:
{%- highlight ruby -%}
Kelsis-MacBook-Pro ~ % /bin/bash
{%- endhighlight -%}


### 3. Install Homebrew by running these lines of code:
{%- highlight ruby -%}
bash-3.2$ /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)" 
bash-3.2$ (echo; echo 'eval "$(/opt/homebrew/bin/brew shellenv)"') >> /Users/kw/.zprofile 
bash-3.2$ eval "$(/opt/homebrew/bin/brew shellenv)"
{%- endhighlight -%}

### 4. Open a new terminal and run these lines of code to add Brew to your profile:
{%- highlight ruby -%}
Kelsis-MacBook-Pro ~ % (echo; echo 'eval "$(/opt/homebrew/bin/brew shellenv)"') >> /Users/kelsiowest/.zprofile
{%- endhighlight -%}

### 🤠Tidbits🤠
Your username should go where `kelsiowest` is.
<br />
<br />

{%- highlight ruby -%}
Kelsis-MacBook-Pro ~ % eval "$(/opt/homebrew/bin/brew shellenv)"
Kelsis-MacBook-Pro ~ % brew install python 
Kelsis-MacBook-Pro ~ % python3 --version Python 3.9.6
{%- endhighlight -%}


### 5. Use Brew to now install Python 3.12:
{%- highlight ruby -%}
Kelsis-MacBook-Pro ~ % brew install python 
Kelsis-MacBook-Pro ~ % python3 --version 
Python 3.9.6
{%- endhighlight -%}


#### 🐄Hold Up🐄
You will see that when I do `Kelsis-MacBook-Pro ~ % python3 --version`, it gives me `Python 3.9.6`.
This is because the default version installed on a Mac is Python 3.9.
But the version we just installed through `brew install` was Python 3.12, as shown in our terminal.

![image info](/assets/images/terminal_1.png)

In order to access the Python 3.12 we just installed, we can do two things:
1. Call Python 3.12 by simply using `python3.12`
2. Change the default `python3` or `python` command to redirect to our newly installed Python 3.12.

Because lots of different codebases and Git repositories require different versions of Python, for my use case, I'm fine with just using `python3.12` if that version is needed, and I can call `python3` if I need the default version 3.9.
<br />

Overall, I'm surprised how smoothly that went. Probably because I don't have any other junk or dependencies to mess things up yet! All in due time. 🕸️
<br />

## Final Marks

| Factor                        | Score |
|-------------------------------|-------|
| Clarity                       | 4.5   |
| Organization                  | 5     |
| Visual Aids                   | 5     |
| Examples                      | 5     |
| All Links/Files Provided Work | NA    |

<br />

## Overall Ranking

#### 🌵Sharp as a cactus spine – Very clear, easy to understand.   
<br />
<br />


