<h1>Scheduling Future tasks - Home Lab</h1>


<h2>Description</h2>
The objective of this project is to familiarize and practice key tasks related to system administration on a Red Hat Enterprise Linux (RHEL) system. This project is comprised of three exercises focused on different aspects of job scheduling and automation using the 'at' command, 'crontab,' and Systemd timers.
<br />


<h2>Utilities Used</h2>

- <b>at</b>
- <b>crontab</b>
- <b>system timers</b>
- <b>VIM text-editor</b>

<h2>Environments Used </h2>

- <b>Redhat Enterprise Linux</b> 
- <b>VMware</b>

<h2>Project walk-through:</h2>

<p align="center">
First, I scheduled a job to write the current date to a file named myjob.txt three minutes from now using the 'at' command. I watched the job in the queue with atq and verified the result by checking the content of the file using cat myjob.txt.: <br/>
<img src="https://i.imgur.com/6tUwOWV.png"/>
<br />
<br />
Next, I interactively scheduled another 'at' job to echo "It’s teatime" into a file named tea.txt at 4:00 PM, placing the job in queue 'g'. I also scheduled another interactive 'at' job to echo "The cookies are good" into a file named cookies.txt at 4:05 PM, placing the job in queue 'b'. I confirmed the scheduling with atq.:  <br/>
<img src="https://i.imgur.com/nkkY2It.png"/>
<br />
<br />
To wrap up, I used "atrm" to remove the job scheduled for teatime. I checked the scheduled jobs with atq before and after the removal.: <br/>
<img src="https://i.imgur.com/EZ2nsWv.png"/>
<br />
<br />
For the second exercise of this project, I scheduled a recurring job to write the current date and time to a file named "my_first_cron_job.txt" every two minutes between 6pm and 11PM from Monday to Friday using 'crontab'. I confirmed the scheduling and verified my work.:  <br/>
<img src="https://i.imgur.com/6VBYUDd.png"/>
<br />
<br />
Next, I used a "while" command to wait until the file was created and then verified its existence.:  <br/>
<img src="https://i.imgur.com/rRksEmY.png"/>
<br />
<br />
Finally, I removed all cron entries and confirmed that my crontab was empty.:  <br/>
<img src="https://i.imgur.com/WFPsjmA.png"/>
<br />
<br />
In the last exercise of this project, I installed the "sysstat" package as the root user, configured it to run every 2 minutes instead of the default 10 minutes, and enabled the new timer.:  <br/>
<img src="https://i.imgur.com/gUA5ipA.png"/>
<img src="https://i.imgur.com/KM1MeSW.png"/>
<br />
<br />

