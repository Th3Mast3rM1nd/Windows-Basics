# Disk Utilities and Alternate Data Streams (ADS)

```fsutils``` : is set of Programms That manage drives on windows System 

<img width="498" alt="Screen Shot 2021-10-24 at 12 13 12" src="https://user-images.githubusercontent.com/92652606/138590002-04c3eba9-6d63-4a21-8efe-76644260ea1b.png">

``` fsutil fsinfo ``` : get information about the ```fsinfo ``` 

<img width="468" alt="Screen Shot 2021-10-24 at 12 15 19" src="https://user-images.githubusercontent.com/92652606/138590014-84267401-b610-4ec4-b557-6ddfaa01195c.png">

```fsutil fsinfo drives ``` : list all drives on the machine 

<img width="489" alt="Screen Shot 2021-10-24 at 12 16 20" src="https://user-images.githubusercontent.com/92652606/138590020-6cd63a73-3895-4b82-add7-7884f31ff74c.png">

```fsutil fsinfo drivetype C:\ ``` the type of the drive 

<img width="540" alt="Screen Shot 2021-10-24 at 12 17 27" src="https://user-images.githubusercontent.com/92652606/138590027-2d98fd41-612e-4c47-bff4-b37935e879c0.png">


```fsutil fsinfo volumeinfo C: ``` volume info 

<img width="552" alt="Screen Shot 2021-10-24 at 12 19 08" src="https://user-images.githubusercontent.com/92652606/138590037-2591f527-b03a-4bf7-a33d-4608c71c7b0a.png">

# Alternate Data Streams (ADS). 

``` dir /R ``` to identifying ADS

<img width="611" alt="Screen Shot 2021-10-24 at 12 21 38" src="https://user-images.githubusercontent.com/92652606/138590048-ebf128a6-fb35-41d5-925f-e16899a11b77.png">


``` echo this is a stream file > stream.txt:streampart ``` : to create a ADS file 

<img width="777" alt="Screen Shot 2021-10-24 at 12 25 12" src="https://user-images.githubusercontent.com/92652606/138590053-b454af04-efdd-45c2-bf65-89b5934077e0.png">


```  more < stream.txt:streampart ``` to read ADS files 

<img width="651" alt="Screen Shot 2021-10-24 at 12 27 23" src="https://user-images.githubusercontent.com/92652606/138590062-ea7dafd0-5a23-4bff-a07c-55d96370ec0a.png">

