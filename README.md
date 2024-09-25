# R36sGuide
A guide on getting started with you R36s and more.

This guide works on a **Windows 11** computer with the **R36s** with **ArkOS 2.0** and **Panel 4**

Things like **Setting up the R36s for the first time, customizing themes, custom boot & loading images, changing it's appearance on the outside, PortMaster and installing Stardew Valley** are covered here.

[Setting up your R36S for the first time](#setting-up-your-r36s-for-the-first-time)

[Custom boot and loading images](#custom-boot-and-loading-images)

[Customizing your R36s on the outside](#customizing-your-r36s-on-the-outside)

[Updating PortMaster](#updating-portmaster)

[Installing Stardew Valley](#installing-stardew-valley)

[Making your own case for the R36s](#making-your-own-case-for-the-r36s)

[Printing your own shell and full dissasembly of the device](#printing-your-own-shell-and-full-dissasembly-of-the-device)

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

Now, open the BMPs folder, and you'll find around 5 other images. These are the preloaded loading screens that come with the console. You can delete them all of you don't want them, and just add the logo image from before. 

I haven't tested it yet, but if you add several BMPs on this folder, they may randomize which boot screen you get (based on what I've seen).

**Customizing your loading screens**

For this, you will need to go to your EASYROMS partition and search for the "launchimages" folder. There you'll find a .ascii, a .gif and a .jpg

![Captura de pantalla 2024-09-18 112221](https://github.com/user-attachments/assets/8e5179bd-eb50-4c5b-8af1-56e3ae44e40a)

As you may have noticed, this means you can also add a GIF as your loading image. You can later select this option on your EmulationStation menu.

What you need to do is as easy as modifying the name of your new custom images (whether is a JPG or a GIF) to "loading" and just change the old one for the new one.

So congrats, you're done!

# Customizing themes

_Note: this works for the R36S-name themes although it's only tested in the Epic Noir one. For the other themes, this is NOT your place LOL_

You can do this two ways.

First, you can choose to create your own theme from "scratch", in that case, I will leave a link below for the Albedo Theme. As far as I can tell, it works, although I couldn't get rid of the scanlines on the images, but that might just be a me issue. 

For the Albedo go here: https://github.com/mluizvitor/es-theme-albedo/tree/main

Now, there's a way easier way to customize your themes.

You need to pick one of these:

![Captura de pantalla 2024-09-18 112416](https://github.com/user-attachments/assets/295dc429-5d90-42c3-9547-e2916eeefb67) you will find these in EASYROMS > themes

I think it works with all of the shown above, but you need to find where the art posters are located with each theme. I've found the easier ones are the **epic, epicnoir & switch** themes, although this guide is mainly for the epic and epicnoir, you can easily apply this obtained knowledge for the rest.

You need to go into your theme (epicnoir in my case) and find the art folder

![image](https://github.com/user-attachments/assets/e7cdf235-ee78-4ce0-900d-cd40ffc46e53) then, just get into posters

![image](https://github.com/user-attachments/assets/74d1e3bb-5f6f-4898-84df-5ba3ed82bb82)

In there you will find a lot of images in .jpg format, with the abreviations for each system.

![image](https://github.com/user-attachments/assets/bfccf84e-a841-4d62-b440-035551702de7)

So, you need to find as many images as systems you want showing in your device. Make sure they are 640x480px so they look correctly. Also,a nice thing to keep in mind is the darkness of our pictures. Themes like Epic Noir have a darker part on the left so you can actually read the white font, so I suggest you go into photoshop and add this shade manually, something like this:

![Captura de pantalla 2024-09-09 175237](https://github.com/user-attachments/assets/fde6e555-9609-435f-8f4f-178ff23411f2) ![image](https://github.com/user-attachments/assets/601f17e5-9ac9-4fe4-a507-3ffadebd2753)

Once you're happy with what you got, save them in .jpg format, and find the abreviation for each system you want, and use that as it's name. (nds for nintendo DS, gba for GameBoy Advance, auto-allgames for all games, custom-collections for your custom collectios, etc).

Then just get all your images with the right names and paste them into the **posters** folder. If done correctly, this should replace the old for the new images, and you will be done.

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

To use Wifi on your R36s you need a Wifi Dongle and most likely a USB A to USB C adapter. You can look at this list to see which Wifi dongle works for you (https://docs.google.com/spreadsheets/u/0/d/1gWxtr-GmwWop-_qGUq022RXxK2aTLpPg9Qra68TQLI8/htmlview#) I used this one (https://www.amazon.es/dp/B008IFXQFU?ref=ppx_yo2ov_dt_b_fed_asin_title) and it worked perfectly. They are as cheap as 7€ so it's totally worth the trouble of not setting ports up manually, which, if you ask me, it's a nightmare.

Once you've set up your dongle on your computer or whatever it requires, you can connect it to your console. On **Options** scroll down to the **Wifi** option. Get in (if you can't, maybe you have the latest version of ArkOS (August 2024), that has a bug there. While I can't provide you with a fix, there's some people who have had the same issue and just downloaded a previous version of ArkOS or actually found a fix, which I'm sure you can find somewhere on reddit or gitHub), set up your wifi, password and all, and you're done. You'll probably notice the console starts making weird sounds, that means you're doing it right, and you should get prepared for more.

Now, once your Wifi is setup, in Options, find PortMaster, enter, and it will tell you updates are available. You need to install them, accept the terms and conditions, etc. Beware, your device will start screaming, quite literally, I suggest you lock it somewhere while it does it's thing because it can get ANNOYING. 

Once it's stopped the screaming, that means it's done. Now you'll see that in all ports you can find like 400 new games. Some are ready to install, some require files and it will tell you so. I suggest looking at the PortMaster wiki (https://knulli.org/systems/portmaster/) for more info.

# Installing Stardew Valley

In PortMaster, you need to find Stardew Valley in the All Ports section. Make sure you wifi is on and connected, or else this won't work. I've found that if I scroll down to the S, the device collapses, so I suggest to scroll up and start from the bottom.

Then, once you find it, you click on it, and click on Install or Reinstall. This will take a while and your device will scream (again).

Meanwhile, you need to own Stardew Valley first on Steam. Go there and change it to the compatibility version.

Open Stardew Valley on Steam and go to Properties

![Captura de pantalla 2024-09-09 181432](https://github.com/user-attachments/assets/f5eca0f8-9078-4bdb-8153-8e553fdf91a4)

In properties, find BETAS

![Captura de pantalla 2024-09-09 183333](https://github.com/user-attachments/assets/b3c74a74-49b3-4da0-aca5-15f48ab99ba2)

And in BETAS choose the compatibility option

![Captura de pantalla 2024-09-09 183411](https://github.com/user-attachments/assets/5b323a63-a9d8-4e10-94fe-0bb3e907fb57)

Install it and just in case, once it's done, open it to see everything runs correctly. Close it and move on to the next step.

Now you need to open the Steam console, press **Windows + R** and write this: steam://open/console

Now you need to give the command: download_depot 413150 413153 4264972535478467767

There's a chance that may give out an error. In that case, go to this page (https://steamdb.info/depot/413153/manifests/) and find the latest manifest number, change the last number for that one.

It's important you don't exit the Steam console while it downloads as you may get this error:

![Captura de pantalla 2024-09-09 183042](https://github.com/user-attachments/assets/9340ef06-5166-4925-a607-93c18f51fe37)

You won't recieve any kind of feedback that it's downloading, instead, you'll just see this if it's actually doing it:

![image](https://github.com/user-attachments/assets/8dc59ac4-16ee-4ff7-95fb-0d46b1e581fd)

And this if something went wrong and you need to change the manifest:

![image](https://github.com/user-attachments/assets/28c05275-0873-49c3-83a2-373d0f43643b)

It will take a while to download (a long while) but you'll know it's done once you see this:

![image](https://github.com/user-attachments/assets/2e735f4e-9b4f-453a-90cd-073508734173) (you will just get it once probably, I got impatient)

Copy the adress it's giving to find the depot on your computer, it will get you here:

![Captura de pantalla 2024-09-09 183805](https://github.com/user-attachments/assets/928f636d-e85a-4522-9076-69990e75ec5b)

Save it for later, and insert the SD card from your device onto your computer. You need to find the **ports** folder in EASYROMS. if everything went right while installing Stardew on the R36s you should see this:

![Captura de pantalla 2024-09-09 184110](https://github.com/user-attachments/assets/b460c6b8-90d8-4969-8935-d30fcff15b5b)

Follow **ports\stardewvalley\gamedata** and copy all from the depot in there.

Once that's done, look if you can find this file in EASYROMS\tools\PortMaster\libs

![Captura de pantalla 2024-09-09 184629](https://github.com/user-attachments/assets/647a4eea-6e16-4bce-871f-d56096de5671)

If you dont, you can download it here (https://github.com/PortsMaster/PortMaster-Hosting/releases/download/large-files/mono-6.12.0.122-aarch64.squashfs) add it to EASYROMS\tools\PortMaster\libs once you got it.

Now take out the SD card, insert it on your console and see if Stardew Valley works.

If it does, great! and if it doesn't (like what happened to me) here's how you can fix it:

Delete ALL the new stuff you just added to ports. This should be all you're left with:

![Captura de pantalla 2024-09-09 184935](https://github.com/user-attachments/assets/0dbabd21-df21-42df-b715-6964b668f994)

And in **ports\stardewvalley\gamedata** you should ONLY have a .gitkeep, nothing else. If that is done, you don't need to touch anything else.

Now you need to find where Stardew Valley is installed in your computer. I found it by looking in Archivos del programa x86 (your equivalent for english speakers) and searching for Stardew Valley.

![Captura de pantalla 2024-09-09 185922](https://github.com/user-attachments/assets/770465cc-ffae-4f09-b9ba-19e10b640c22)

In there, you will find this:

![Captura de pantalla 2024-09-09 185958](https://github.com/user-attachments/assets/142af826-0476-482f-969b-257272826387)

So, copy ALL of that, and paste it in **ports\stardewvalley\gamedata** in EASYROMS. You should be left with something like this:

![Captura de pantalla 2024-09-09 190123](https://github.com/user-attachments/assets/a9d23ee0-dbac-4b68-8d19-3d89d6df6856)

Check again on **tools\PortMaster\libs** for the file mentioned previously, and if you have it you are officially done. Put the SD back on you device and enjoy.

Note: It will take a long time to load, every single time you open it. As long as you get the Loading, please wait message, it's all good, don't worry.

# Making your own case for the R36s

Of course, I had to make a custom case for my device.

I found this on Thingiverse: https://www.thingiverse.com/thing:6412954

You will find there's two versions, one for adding magnets and one that doesn't allow that. Mine's the latter.

For this one, you will need to print both parts and sand the closing part down, opening and closing it a few times as well so you'll be able to open it properly. 

However, when I updated my shoulder buttons to the better version, it didn't fit anymore, so here's my remix for the better shoulder buttons: https://www.thingiverse.com/thing:6777902

You will end up with something like this:

![image](https://github.com/user-attachments/assets/7ad0a98e-868c-4505-ad0e-1fc65d86d9b8)

As you can see, I added some padding to the screen part so it had 0 chances to break. It fits with little wiggle room, so you can be sure your device will be safe

# Printing your own shell and full dissasembly of the device

Did you want your device on another color, but painting it isn't working for you?

Did Aliexpress shops give you a short but hurtful answer to you asking for a shell?

![Captura de pantalla 2024-09-18 120421](https://github.com/user-attachments/assets/43667488-084c-47aa-8710-36f1e6a8cfef)

Well, look no more! u/firezenk did this shell (see reddit post here: https://www.reddit.com/r/R36S/comments/1fiucg8/full_case_replacement_for_r36s_available_for_3d/) and I'm going to teach you how to **CAREFULLY** dissasemble everything, including the screen.

You'll need: two (small but different sizes) screwdrivers (I have absolutely no idea about the specifications for them, just see what fits lol), a thin yet sturdy plastic, hands, and patience. And please: don't ask your father for help as I did (specially being a grown ass woman, shame on me) since they may have the bright idea to put pressure on the screen and end up breaking it. 

To start with one of the most important things: TAKE OUT YOUR SD CARD. It may seem a dumb thing to remind, but you need to this first, since taking out the board will be imposssible and you may break it.

First thing you've got to do is look at the back of your device:

![IMG_20240925_144033](https://github.com/user-attachments/assets/f381f809-2117-45c9-b3cd-7c84c944fbcf) (please, ignore the fact that it's incomplete, I literally had no time or will to finish it since someone broke my screen)

You'll find 6 screws, remove them carefully, and take out the bottom half of your console. BE CAREFUL: I am detatching the battery later since it's easier this way for me, so if you haven't done that first: TAKE IT OUT CAREFULLY and set both halves on a desk.

Now, you'll see this:
![IMG_20240925_144312](https://github.com/user-attachments/assets/9d7160ad-8246-4ed6-90f1-5e83806c1636)

Your battery is still atatched, so carefully, pull the connector out, might be easier if instead of directly pulling on it, you wiggle it a bit.  

Once that's done, we move on to disconnecting the screen.

![IMG_20240925_144335](https://github.com/user-attachments/assets/f2f878f6-56fd-42c5-856f-cac96a712a97)

As you can see, there's a white connector with a black sort of clip. Pull that clip up, like this:

![IMG_20240925_144341](https://github.com/user-attachments/assets/7cc1210d-7453-4965-a8ae-cc9ba5acbf0d)

And then free up the connector taking it out:

![IMG_20240925_144350](https://github.com/user-attachments/assets/0e8d5fb0-6c7e-4f74-9922-a14c60db6507)

Now, once that's done, I reccomend taking out the joysticks first. You'll see there's two screws for each of them, that are slightly smaller than the others, so use your smaller screwdriver for this.

![IMG_20240925_144440](https://github.com/user-attachments/assets/e36ccb54-295b-4702-b27e-b4f9b71fa617)

And for the last of the screws, you'll find two attatched to the board:

![IMG_20240925_144359](https://github.com/user-attachments/assets/eae68d71-f836-4f7c-a342-07d7c68a030c)

Unscrew them and take out the board carefully.

WARNING: the first time it may be a little harder to do, so I recommend you pick a flat screwdriver and pull up carefully from both of the upper corners. You'll need to be careful every time since the usb and minijack ports are on the lower part and they are inside holes in the shell.

Here you may encounter a similar issue than me (trust me, it's happened more than once and the first time I panicked):

![IMG_20240925_144657](https://github.com/user-attachments/assets/a628e16a-011f-4bab-bdf3-cae08cf4583a)

Your joysticks dedided being connected was too much work. But, don't worry, they work exactly as the screen connector, you can pull the small black clip up (this one is on the bottom part for the left joystick) and insert the connector back in on the opposite side of the clip, close it, and you're done with that.

So, now you will be left with this:

![IMG_20240925_144638](https://github.com/user-attachments/assets/9a4d6b63-da6a-4036-a6fb-3878116a414a)

From here, you can choose to change your buttons (see this for what I used when modding the original shell: [Customizing your R36s on the outside](#customizing-your-r36s-on-the-outside)) or do more extreme stuff like taking out the screen.

In case that's what you want to do, I can't stop you (if I could've stopped myself I would) so I'll teach you to do it carefully and properly.

Make sure you're on a plain and clean table, and you have lot's of time available. 

Then, pick up your plastic tool of choice (u/firezenk recommended me a guitar pick, which was too short for my liking, or the plastic that comes with your new SD cards, which was what worked for me) and see if you can wiggle it there without putting that much pressure on the screen. It's just patience from there. You'll need to get it under here (which in my case is red, and in yours will be the color of your device:

![IMG_20240925_144727](https://github.com/user-attachments/assets/ddc16b59-dadc-4363-9781-89c3df896fc4)

You'll see that there are 3 pieces of black double sided tape that is there to stay. My personal recommendation is wet your plastic tool with a drop of alcohol every now and then and the job will be done faster. Aim for the double sided tape until the screen is free. Be careful, because it comes out outwards, so don't drop it. It may take a while, for me it was 3 long hours, but for the love of god, no matter how impatient you get DON'T PUT ANY KIND OF PRESSURE ON THE SCREEN or you will end up like this:

![image](https://github.com/user-attachments/assets/c9184b8c-cd10-434b-a556-6da5de11a4ff) and from here is either a screen replacement or a new device haha.

So, with that out of the way, here's how to change the back buttons. You'll see this:

![IMG_20240925_145205](https://github.com/user-attachments/assets/5b916f7a-4931-46f0-bc53-76eb70576f05)

You'll find that the buttons are connected to the shell by too little knobs on each side. What you need to do is with your hands, pliers, teeth, or whatever you may find, squeeze the sides of the button on the inside sond push out until they come out. There's literally no other way, and it's harder than it seems.

Once the buttons are out, inserting new ones is just a matter of skill and placement.

And now your device is fully disasembled: Time to add a new shell.

Going to the post I mentioned before will guide you here: https://cults3d.com/en/3d-model/gadget/front-case-replacement-for-r36s for the top part & https://cults3d.com/en/3d-model/gadget/rear-case-replacement-for-r36s for the back.

I printed the top shell at a 100% infill, with tree supports at 0.12mm quality and with the display looking to the buildplate-

I printed the back also at 100% infill, tree supports, 0.12mm and with the inner part looking to the buildplate.

I used Smartfill's Crystal Red PLA (https://www.smartmaterials3d.com/placrystal#/2-tamano-m_750g/26-diametro-175_mm/215-color-crystal_red) because I wanted to keep the retro transparency vibe.

For this print, you will need to print the buttons that come with the Cults3D files, because the originals won't fit it. Personally, I edited them to be a bit higher than they came since they're more comfortable to me.

Also, for the back you'll find two files. One's for the classic buttons (the ones that come with the device) and the other is for the improved shoulder buttons (which kindly u/firezenk did when I suggested it).

And with all that here's the final ressult:

![IMG_20240925_145526](https://github.com/user-attachments/assets/b2682649-3cf6-49e4-b6a6-13f9f609befb)![IMG_20240925_145533](https://github.com/user-attachments/assets/b2567c4e-e87f-4cb2-811a-f9140af2f6db)![IMG_20240925_145538](https://github.com/user-attachments/assets/3e0dd151-66c1-4ebd-a77e-81f864f33f27)![IMG_20240925_145543](https://github.com/user-attachments/assets/743ed9b4-40f8-4154-837c-3f6ced938550)




