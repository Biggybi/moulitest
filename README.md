# Moulitest ![travis](https://travis-ci.org/yyang42/moulitest.svg)

<img align="right" height="230" src="http://i.imgur.com/3p0Xg7Z.png">

This repository contains tests for several projects done at 42.

Tested 42 projects:

* libft
* get_next_line
* ft_ls
* ft_printf
* libftasm

Feedbacks, github issues and pull requests are welcome.

**Note: the moulitest is a test made by humans and may report false positive or false negative. Use it with caution.**

## Quick Start
Create the config file

	cp config.ini.template config.ini

Edit the config file

	vim config.ini # add your configs

Run tests
	
	make

## Advanced use
Run only some tests

	make ft_ls PATTERN=<regexp>
	# e.g. To run only the tests starting with "05" you can use
	make ft_ls PATTERN=^05

Notes
---
GNL

* If the tests stop in the middle, it could mean that your get_next_line is waiting for an input from the file descriptor but nothing is coming.

Credits
---

The test framework and many libft tests are based on the work done by Maxime Bacoux (mbacoux). 
Here is the original repository: https://github.com/Nax/libft-test.  
Thanks to [lefta](https://github.com/lefta) (aka celegran) for his work, especially on the v2.

