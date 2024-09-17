# R36sGuide
A guide on getting started with you R36s and more.

This guide works on a **Windows 11** computer with the **R36s** with **ArkOS 2.0** and **Panel 4**
# Setting up your R36S for the first time
First thing you need to do, is changing your SD card. I suggest looking at this list (https://docs.google.com/spreadsheets/u/0/d/1gWxtr-GmwWop-_qGUq022RXxK2aTLpPg9Qra68TQLI8/htmlview#gid=0) to see which ones are compatible, as not all of them are. You will also need an SD card reader, and a computer, obviously. A 128gb card will do wonders, you don't need more although you are free to add a bigger one.

Insert the original SD card (the one that comes with the console) onto your card reader. You will see that it comes with two partitions. You will most likely see these things:

![image](https://github.com/user-attachments/assets/a992f25b-bdd9-407c-8a0a-6e70d53be573) ![image](https://github.com/user-attachments/assets/f1bb8280-e31d-488b-97bd-83cedaef69c0)

Open this page on your browser (https://aeolusux.github.io/ArkOS-R3XS/tools/dtbIdentify.htm) It will help you identify your screen. You need to find this file:

![image](https://github.com/user-attachments/assets/015e1e2a-933d-41d1-a48a-4faeef1f0565) It is located on the **R36S-OS partition**.

And load it into the page you previously opened. It will most likely tell you your screen is Panel 4, as it's the most common one apparently.

![image](https://github.com/user-attachments/assets/1b92e954-1ebb-43fc-9b53-19132287e746)

Now, once your screen is identified you will need to download the corresponding OS. For that, you will need to go to this page (https://github.com/AeolusUX/ArkOS-R3XS?tab=readme-ov-file) and download the Panel 4 (V5) files. They will take a while to download, so be patient.

While that is downloading, you can start preparing your new SD card for new partitions. For this, you can download this app (https://win32diskimager.org).

You can now safely remove the old SD card from your reader (but keep it close, since you will need it again) and insert the new one. Make sure it is completely empty before starting the process. Now, open **Win32DiskManager**. It should look something like this:

![Captura de pantalla 2024-09-13 115116](https://github.com/user-attachments/assets/8fcba118-f734-465e-954d-d785ea0d3be6)

For the Device, choose where your SD card is located on your computer, and on the image file you will need to add this:
![Captura de pantalla 2024-09-13 115250](https://github.com/user-attachments/assets/6e96d3d3-b621-458f-aaee-0744b57dd9e2) which you previosuly downloaded. It may come compressed, so you should de-compress it first if that's the case.

Now, just click** Write** and wait while it loads. It may take 5 to 10 minutes, don't worry, it'll be fine. Once that's finished, you should find these two things, if all went good:

![image](https://github.com/user-attachments/assets/0e75cf11-5c4e-43d1-96de-88ab9f619f14) ![image](https://github.com/user-attachments/assets/5c5b7323-d745-4b39-a3e5-4d3d93078b78) (although EASYROMS will be empty)

Now, we need to go to this page (https://github.com/AeolusUX/R36S-DTB/tree/main/New%20Screens)





