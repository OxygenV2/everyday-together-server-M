# Mainichi Issho Portable(Everyday Together) minimal server.
This is a mainichi issho server with a path for requested UPDATE.YML file by the game.
Currently there isnt any other files other than UPDATE.YML as there is no other known file or url requested by the game.
Currently it seems that the game does connect to the server it just doesnt get any expectable response from it:/

# Tutorial how to put custom server into the game
Requrements:
- A Laptop or pc
- PPSSPP (Latest Version)
- Copy of Mainichi issho Portable
- Stable Network

## Tutorial
### Step 1
Open PPSSPP then click Settings and navigate to Networking Tab. Toggle Enable networking/WLAN to ON scroll down and put in any username into infrastructure tab.
### Step 2
Go Back to main menu and click Load... navigate to directory you downloaded Mainichi Issho to choose it and click open. The game should now load up. Use Google Translate if you dont understand japanese! Also ingame it uses O button as confirmation button! Then it will ask you to connect proceed with it.
### Step 3
You now should be greeted with this message! Use Google Translate(or any other translator) to translate everything. It will ask you for Your gender,birthday,blood,type,and nyavatar you can put anything you want.
<img width="953" height="533" alt="image" src="https://github.com/user-attachments/assets/a1bbd1dd-89ab-4934-90f2-0c4ebaf9997d" />
After that you will be greeted with the intro. You need to watch it before going into the game itself.
### Step 4
After intro you will see Toro, Press O to open the menu
<img width="966" height="538" alt="image" src="https://github.com/user-attachments/assets/15465369-48e3-4a20-87ee-7d4d5bbc3fd8" />
navigate using arrow keys to the 3rd button press it with O and then a submenu will open choose the 1st option<img width="957" height="537" alt="image" src="https://github.com/user-attachments/assets/be099fed-4416-432d-aead-36c2fef2bef1" /> This will open the shop or atleast try to.
It WILL Error and thats what we need. Error That should appear:<img width="960" height="539" alt="image" src="https://github.com/user-attachments/assets/2ed1688d-44c4-4326-9748-f866f937b96d" />
After the error press X or O To exit out of this error  (depending on your settings by Deffault the Confirmation button is X and so the Back button will be O) After that you should get some popups about failed connection just ignore them and proceed, you should now be back at the main menu
### Step 5
Now click on the Debug Button thats located on top of the PPSSPP window
<img width="960" height="1008" alt="Group 10" src="https://github.com/user-attachments/assets/db011121-de07-4e38-88f3-a512a5bee307" />
From the opened menu select Memory Viewer.<img width="445" height="669" alt="image" src="https://github.com/user-attachments/assets/fd1c828b-59b2-4f63-820d-96716f8d375a" /> 
after that Memory Viewer will open.
### Step 6
Once in memory viewer click on search and type in https:// (write it all lowercase) and click search button
<img width="1579" height="783" alt="image" src="https://github.com/user-attachments/assets/70890a42-ba19-461a-aac4-6403d4f7966a" />
Once in Memory Viewer make sure to only touch these strings <img width="1579" height="783" alt="11Group 11" src="https://github.com/user-attachments/assets/4f20fca8-0ccc-4c19-affe-316983b593b1" /> They contain the actual url needed. Double click them and change the URL to https://oxygenv2.github.io/everyday-together-server-M/p/ or your custom server if you have one.
How its Supposed to look like after changing url:

- 0x9188120 <img width="592" height="103" alt="image" src="https://github.com/user-attachments/assets/504ceb8c-81de-4c07-b4d3-412843df6f13" />


- 0x09408138 <img width="585" height="111" alt="image" src="https://github.com/user-attachments/assets/c3d6a97b-78b6-4f20-a3b6-90420ba66e1e" />

- 0x94D1FDC <img width="590" height="97" alt="image" src="https://github.com/user-attachments/assets/bd74eed7-e63e-4daa-8b90-9d7db9926431" />

After Everything is done exit out of Memory Viewer. And head to the Shop again. It May show a different error this time (ffffffff) or just not show but by looking at the log we can see that it did connect to our server! just didnt get any respond that it wanted :/ Currently thats the farest i can get it to work



# Aditional
If for some reason you want to use the Update or the Refresh Button located at the very end of the main menu You can use that too It will be just a little complicated because the Emulator(PPSSPP) doesnt have a required function that the game is trying to run.
## Step 1 Aditional
Open Debug menu on top of the ppsspp window and click Break This will stop the game this is needed for a short time then open Debug menu again on top of the ppsspp window and open Disassembly and click on a random line so it will get blue(selected).
Once in there press Ctrl+F or if youre on a Mac Command+F then type in 088FAAC8.
You will see a bunch of lines and the one you need is the one that was found with that address right click it and press Assemble Opcode and type in "nop" click okay and repeat the same process for 088FAB30 and 089034A8.

after that close disassembly window then open debug menu and hit Run.
## Step 2 Aditional
After Everything is done head to the update menu and click it and select the first option that appears <img width="944" height="528" alt="image" src="https://github.com/user-attachments/assets/9f2fdcba-5cbc-416b-94aa-9b07021dd14d" />
It will then get stuck and it will be frozen thats fine click Debug on top of ppsspp window then Click break then open Disassembly click on a random line press Ctrl+F or for Mac Command+f and type 088FAC2C then on the line that was found right click on it and click on Assemble Opcode and type "nop"
then close Disassembly click on Debug on the Window and Press Run wait a bit and you're done!
## Please Note that everything in this tutorial is not permanent as it involves editing memory and that after restarting the game you will need to redo everything.








