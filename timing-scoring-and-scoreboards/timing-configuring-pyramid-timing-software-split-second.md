# Timing - Configuring Pyramid Timing Software (Split Second)

## **Overview**

Pyramid timing software uses the SGL Version 1 API for sending live data to the SGL database.  The software supports the following services

1. Live Class View with live timing and score data
2. Live Scoreboard Display
3. GetClass – **This feature does not work as of this writing due to bugs in the Pyramid implementation.**

## **Configuration**

To setup V1 API Access for a particular show company database please read and follow the steps in this document

[SGL Timing API Version 1 Setup Instructions](http://docs.showgroundsonline.com/documentation/sgl-timing-api-version-1-setup-instructions/)

Once that is complete, the remaining setup can be completed in Pyramid software

PLEASE NOTE the GetTrips API does not function.

1.  In pyramid software click on the “Header” tab.  Find the Section labeled “Data to ShowGrounds software”.  For the URL enter “http://”\<ip\_address\_from\_step\_1>”:8080/”.  See the example below.  Next enter the token obtained in step 2 above.  IMPORTANT: Make sure to check the checkbox labeled “Send data to site”

    ![](http://docs.showgroundsonline.com/wp-content/uploads/2020/08/img\_5f35ae80c05cd.png)

## **Live Scoreboard Operations**

For real time timing data used on the live page and for graphics data must also be sent to our Scoring Server (SRN).  This server handles real time data more efficiently and is used whenever live data is being presented on live class page or for any form of graphics (Scoreboard, Lower 3rd, Leader Board, etc)

To set pyramid to send data to the SRN server follow these steps

1.  Obtain the IP address of the computer that is acting as the **SGL SRN Server (Score Routing Node)**The simplest way to obtain the IP address of the SRN server is to visit the Ring Settings page in the admin area for a show company.  This url is typically

    http://www.showgroundslive.com/\<showcompany>/admin/RvsRingConfiguration
2.  Click on DAK Control.  Enter the IP address obtained in step 1 and port “12345”.  Also be sure to check the “Send via UDP” check box.

    ![](http://docs.showgroundsonline.com/wp-content/uploads/2020/08/img\_5f35b077a8ec2.png)

&#x20;

### **Input Mapping Details**

Assuming they have 4 inputs in the timer. In the input mapping do the following

1. Input 1 to Photocell A
2. Input 2 to Photocell B
3. Input 3 to Photocell C
4. Input 4 to Stop/Restart   (button for the judges to Start/Stop countdown and Stop/Restart timing)

Make sure the box that says “Combine Countdown with Stop/Restart” is checked.

## **Downloads**

If you do not currently have Pyramid software you can download it here.

[https://www.splitsecond.com/software/Equestrian\_Install\_3\_34.exe](https://www.splitsecond.com/software/Equestrian\_Install\_3\_34.exe)

[http://www.SplitSecond.com/software/EquestrianCompanion\_1\_02.exe](http://www.splitsecond.com/software/EquestrianCompanion\_1\_01.exe)
