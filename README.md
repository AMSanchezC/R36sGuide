# R36sGuide
A guide on getting started with you R36s and more.

This guide works on a **Windows 11** computer with the **R36s** with **ArkOS 2.0** and **Panel 4**

Things like **Setting up the R36s for the first time, customizing themes, custom boot & loading images, changing it's appearance on the outside, PortMaster and installing Stardew Valley** are covered here, so if you don't find what you're looking for at first, keep scrolling, I'm new to making guides on gitHub and don't know how to link contents.

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

Now, just click **Write** and wait while it loads. It may take 5 to 10 minutes, don't worry, it'll be fine. Once that's finished, you should find these two things, if all went good:

![image](https://github.com/user-attachments/assets/0e75cf11-5c4e-43d1-96de-88ab9f619f14) ![image](https://github.com/user-attachments/assets/5c5b7323-d745-4b39-a3e5-4d3d93078b78) (although EASYROMS will be empty)

Now, we need to go to this page (https://github.com/AeolusUX/R36S-DTB/tree/main/New%20Screens) and download the files for **panel 4** (not the 60Hz version, that one doesn't work). We should be left with **6 files** we are gonna get into our **BOOT partition**.

![Captura de pantalla 2024-09-13 115731](https://github.com/user-attachments/assets/13c60edf-8546-44e2-9360-f6e4002b7748)

Just copy and paste them into **BOOT** and it all will be done.

Extract your new SD card and insert the old one again into the reader. Now, take all the files in **EASYROMS** and copy them to a folder in your computer. This will take around an hour and it will be around 46gb.

Insert your new SD onto the console, turn it on, and let it do it's thing for a few minutes. You will see the main manu once it's done. Turn off the console and take out the SD card again.

Once all the files are on your computer, change cards again, and you can finally store or discard the old SD card. Choose all the files you just copied to your computer, and copy them back into **EASYROMS** . This will also take around one hour, so sit back and relax.

Once that's done, congrats!, you finished, put the new SD onto your console and enjoy!

_All this info and links were taken from this video btw, if anything fails, it's because I might've missed something, it all should be here https://www.youtube.com/watch?v=gd5-HvKJrOs_

# Custom boot and loading images

Do you want to add a custom boot or loading image? Well, you've come to the right place.

You will need to find 2 images, set them to 640x480px and save the loading screen one as a .jpg and the boot one as a .bmp (24 bits). The latter can be done with paint.

**Adding your custom boot images**

First, make sure you have a 640x480px image in a .bmp format. This is archievable by doing so on paint. You just add your image, edit it as you wish and then just click "save as > BMP Image" and make sure you choose this:

![image](https://github.com/user-attachments/assets/bb12a300-d57c-45ba-b178-14e3fe3a27f3) (I know it is in spanish, but just make sure the 24 bit part of it it's present)

Also, to save time, directly save it as "logo".

Now, open your **BOOT** partition, and there you'll find something that looks like this:

![image](https://github.com/user-attachments/assets/076037dc-78de-49f4-8b06-1300e8829a11)

We will be changing the "logo.bmp" for our new one, which, if they're named the same, can be done with a simple copy and paste.

Now, open the BMPs folder, and you'll find around 5 other images. These are the


# Customizing themes

_Note: this works for the R36S-name themes although it's only tested in the Epic Noir one. For the other themes, this is NOT your place LOL_

You can do this two ways.

First, you can choose to create your own theme from "scratch", in that case, I will leave a link below for the Albedo Theme. As far as I can tell, it works, although I couldn't get rid of the scanlines on the images, but that might just be a me issue. 

For the Albedo go here: https://github.com/mluizvitor/es-theme-albedo/tree/main

Now, there's a way easier way to customize your themes



# Customizing your R36s on the outside

_Some may have seen my post on Reddit about how I got custom buttons made and also changed it's color, so I thought it would be nice to share all the files I used and other stuff to help others customize it to the max_

This is how my R36s looks like now, for reference:

![image](https://github.com/user-attachments/assets/aff45a09-7085-4847-9b86-cbf800447c3a) ![image](https://github.com/user-attachments/assets/1aac2e89-edab-4438-bea5-232e96f9614c)

**Printing the buttons**

For the D Pad I used this (https://www.thingiverse.com/thing:6477050) you'll find two models, I used the V3 one, and it sits slightly higher than the original one, making it way more comfortable to use. 

For the shoulder buttons I used this (https://www.printables.com/model/794361-r36s-shoulder-buttons). They have definetly made my user experience wayyyy better since now they make a lot less noise, don't click on accident when putting the console on a table and are in general way more comfortable to use.

And for the rest of the buttons I used this (https://www.thingiverse.com/thing:6477054) you will find 3 models. For the FN, SELECT, START I used the v2, for ABXY I used the convex ones. Keep in mind these fit tightly sometimes, and at first they will make a lot more noise than the original ones, but with a few days of play, they'll be almost completely silent again.

In case you might be looking for the filaments I used here's the list:

For the D Pad & shoulder buttons: https://www.amazon.es/ZIRO-Filamento-Impresora-1-75mm-Multicolor/dp/B0BG252MCH?pd_rd_w=qO2xj&content-id=amzn1.sym.facf7f17-8601-4d92-88f5-b69918861ce5&pf_rd_p=facf7f17-8601-4d92-88f5-b69918861ce5&pf_rd_r=D7V9EEQ0JMKQ9SVXNW0C&pd_rd_wg=Jvbk2&pd_rd_r=8170cfad-8d5c-450b-8c80-a8bc663eb4ef&pd_rd_i=B0BG252MCH&psc=1&ref_=pd_bap_d_grid_rp_0_2_t

Select button: https://www.smartmaterials3d.com/iris#/2-tamano-m_750g/26-diametro-175_mm/206-color-tanzanite

Start button: https://www.smartmaterials3d.com/silk#/2-tamano-m_750g/26-diametro-175_mm/209-color-silk_blue

FN button: https://www.smartmaterials3d.com/iris#/2-tamano-m_750g/26-diametro-175_mm/221-color-alexandrite

A button: https://www.smartmaterials3d.com/pla-glitter-filamento#/2-tamano-m_750g/26-diametro-175_mm/105-color-red_glitter

B button: https://www.smartmaterials3d.com/pla-glitter-filamento#/2-tamano-m_750g/26-diametro-175_mm/107-color-green_glitter

X button: https://www.smartmaterials3d.com/pla-filamento#/3-tamano-l_1000g/26-diametro-175_mm/31-color-silver

Y button: https://www.smartmaterials3d.com/silk#/2-tamano-m_750g/26-diametro-175_mm/203-color-copper

**Painting your R36s**

You may have noticed my case is painted. My reasoning? I saw there were blue and green versions, and I was stuck with classic purple, so I asked sellers on alliexpress if they'd sell the shell separetedly and this is the response I got:

![image](https://github.com/user-attachments/assets/d4bc065b-a841-4488-9035-e8f1224e8f86)

So I decided to take matters into my own hands, I used AK's Cobalt Blue and got to work. It looks way easier said than done, because I faced some complications.

![image](https://github.com/user-attachments/assets/0b957184-2ca0-40f8-8af7-0321e960760a)

Firstly, you need to dissasemble it COMPLETELY. I didn't want to remove the screen in fears of damaging it, so I didn't, but now I have some unpainted parts. You will need to use the smallest paintbrush you have available since there are a lot of small parts a big one can't get to. The back part is easy enough, but the front is where it gets tricky.

Make sure you don't paint the SD card hole or the charging holes, and specially the OFF/ON & Volume buttons, as they may not fit well later and may not work properly. However, to fake the whole painted look on parts that you may not feel comfortable painting, you will need to paint both rims of the shell, avoiding to gat paint on the outside. 

As for the screen part, a small paintbrush should get easily into the little spaces it can, and the rest, just paint the borders of the plastic sitting on top of it, that way, when you look at it from the front, looks like you painted it all.

I suggest no more than 2 layers of paint, although 1 would be best, because more might make the pieces not fit together again. So I suggest getting a paint that covers well with few layers (Vallejo won't do, been there, done that). To make sure you're using the right paint, try painting the battery cover first, as it can easily be cleaned.

# Updating PortMaster

