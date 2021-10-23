# Scheduled Tasks 

allows us to schedule computer programs or scripts to run at pre-defined times or upon certain triggers.

``` schtasks ``` : Enables an administrator to create, delete, query, change, run and end scheduled tasks on a local or remote system.

<img width="698" alt="Screen Shot 2021-10-23 at 20 32 20" src="https://user-images.githubusercontent.com/92652606/138567870-045cbe5e-f422-4a63-b949-bf2056b817d5.png">

``` schtasks /create ``` : To create a new Task 

```/tn ``` : task name 

``` /tr ```: task run ( which means the program )

```/sc ``` : specifies the schedule frequency.
                       Valid schedule types: MINUTE, HOURLY, DAILY, WEEKLY,
                       MONTHLY, ONCE, ONSTART, ONLOGON, ONIDLE, ONEVENT.

<img width="907" alt="Screen Shot 2021-10-23 at 20 35 05" src="https://user-images.githubusercontent.com/92652606/138567884-f9ff6c90-045e-4783-966c-e61336e985aa.png">

``` schtasks /run ```: to run a task 

<img width="690" alt="Screen Shot 2021-10-23 at 20 38 49" src="https://user-images.githubusercontent.com/92652606/138567893-8ea42348-821b-40df-9aa5-445f445dbf3f.png">


``` schtask /delete ``` : to delete a task 

<img width="698" alt="Screen Shot 2021-10-23 at 20 39 47" src="https://user-images.githubusercontent.com/92652606/138567897-b054d676-14f5-4fea-8ec2-8cac4bc54fc6.png">




 
