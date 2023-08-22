# Crawler
Authors: Asukava & Pskytta, Hive Helsinki Alumni
## What?
A web crawler written in Python and using the following:
- beautifulsoup (for HTML parsing)
- SQLite (for database)
- flask (web app framework)

## Why?
Idea is to have a simple web app that we could use through browser to find 5 or more positions
where we could apply to daily.
## What does it do?
- Crawls through a job listing website in search for job postings for
software developer roles.
- It runs once a day and updates SQLite database with new listings it finds.
- There is also a web application that asks email and keywords from user. The
keywords are used to search database on the server for jobs matching those
keywords and returns title and a link to the job posting.

## Deployment
- Deployed on a Oracle Cloud running Oracle Linux Server 8.8. (Full deployment under construction)
Steps we took with the server:
1. create usernames and home folders for both of us.
2. connect to the server via SSH.
3. write scripts to update the server on midnight.
4. create a group for both users to facilitate permission handling.
5. install required services with `yum`
6.

## Useful Information

In case you wish to clone the project we recommend Linux as the operating system.

To create the virtual environment use `python3 -m venv myenv`

To activate the virtual environment use `source myvenv/bin/activate`

To deactivate the virtual environment use `deactivate`

To install the required libraries use `sudo pip install bs4 requests`
