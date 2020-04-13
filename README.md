# Codify

A Judgesystem for Coding Challenges.

## Getting Started

Download the Zip file and unzip to server directory.

## Prerequisites

Should have PHP,MySQL server installed with latest browser.

## Installing

1. Configure the username,password of SQL server in following files.
	- includes/dbConnector.php
	- judger/judge.py
2. Run the judgesystem.sql file to build Database.
###### For Linux only (Additional Steps)
- Type following commands
```
	sudo apt-get install python3.7
	sudo apt install python3-pip
	pip3 install coderunner
	pip3 install mysql-connector
```
- Open [includes/submit.php](https://github.com/manoharc07/judgesystem/blob/master/includes/submit.php) in line 22 with *exec* function  replace the line with following
`exec('..\judger\env\Scripts\python3 ../temp/'.$codefile.' '.$prob_id.' '.$lang.' '.$user.' >> ../temp/submissionlog.txt');`


## Deployment

- Open http://localhost/judgesystem or http://servername/judgesystem
- You need to sign up before logging in.
- To upload problems use following credentials.
	- **Username**:  admin
	- **Password**:  admin

## Built With

* Built using PHP,MySQL,Jquery.
* [XAMPP](https://www.apachefriends.org/download.html) - Development Environment.
- [Codemirror](https://codemirror.net/index.html) - JS and CSS based Editor.

## Authors

**Manohar C**- *Initial work*

## Acknowledgments
- Thanks to [Codemirror](https://codemirror.net/index.html) and [Judge0](https://judge0.com/) for development tools.
* *This is prototype and is not suitable for largescale deployment.*
