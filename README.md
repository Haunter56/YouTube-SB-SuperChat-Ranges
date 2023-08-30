# YouTube-SB-SuperChat-Ranges
Instructions and import code for a range workaround for Streamer.Bot version 0.2.0

I have tried to put it in the format that will be used for the Streamer.Bot wiki

## **Description** 
 
With this you will be able to have actions trigger based on ranges that you set. The ranges for Super Chats are not triggering at the moment in version 0.2.0   


## **Import Code** 

[Streamer.Bot Code](https://github.com/Haunter56/YouTube-SB-SuperChat-Ranges/blob/main/super_chat_ranges.sb)


## **Installation** 

In Streamerbot select the Import button from the top left menu.

Drag and drop the file or copy the text from the file and paste all the text into the Import String field.

![image](https://github.com/Haunter56/YouTube-SB-SuperChat-Ranges/assets/107263697/de8995f3-9bba-4ce0-a437-0ecf9d328602)



There should be 8 actions.



## **Configuration** 


### C# Compiler
Make sure to add System.dll to the C# compiler within Settings > C# Compiler > Common References > Right-Click > Add reference from file...

![image](https://user-images.githubusercontent.com/107263697/220821729-181e6c95-874d-4dbe-a19a-4ed0c6afee96.png)


![image](https://github.com/Haunter56/YouTube-SB-SuperChat-Ranges/assets/107263697/0d165dd7-fcc6-4ec8-b3ca-483f9a51d324)


This will help make sure all the C# code found in the sub-actions compiles. To make sure, go into the action called "Super Chat Range Event and Settings" > Double-Click the "Execute Code" sub-action > click "compile" to make sure it compiles

![image](https://github.com/Haunter56/YouTube-SB-SuperChat-Ranges/assets/107263697/5ae5e4ff-5271-484b-9179-da828548a578)


![image](https://github.com/Haunter56/YouTube-SB-SuperChat-Ranges/assets/107263697/c97b852f-21fb-4977-81a2-3cdb3277d431)


### Range Settings
In the "Super Chat Range Event and Settings" update the arguments for your desired ranges. There are 6 total that can be triggered
Ranges 1-5 and the MAX range. Each number will be triggered at the number amount you input, OR if it is BELOW the input number and ABOVE the previous range.

![image](https://github.com/Haunter56/YouTube-SB-SuperChat-Ranges/assets/107263697/de1a97fd-f4d0-4a52-a936-0aed74bb295a)

If you want to have less ranges, just "disable" the range sub-actions so they turn red starting from range 5, then 4, and so on.

FOR EXAMPLE - If you want to only have 3 separate ranges $0.00-$5.00, $5.01-$25.00, and $25.01+ you would do the following:
- Update range 1 to 5
- Update range 2 to 25
- Disable ranges 3 through 5

![image](https://github.com/Haunter56/YouTube-SB-SuperChat-Ranges/assets/107263697/98a38afe-3458-443c-b689-c3b3b0daf885)



### Actions Configuration

There are two options to configure your action triggers.
- The import will come with some actions that have triggers attached to them already. Feel free to use those and add your own sub-actions, BUT you don't have to if you already have some actions.
- If you would like to use your EXISTING actions for the ranges, here is what you do:

1. Restart Streamer.Bot
2. Find the action you want for the range you want to assign
3. Right-Click in the `Triggers` section and go to `Custom` > `YouTube` > `Super Chat Range` > `[YOUR DESIRED RANGE #]` and assign the trigger

![image](https://github.com/Haunter56/YouTube-SB-SuperChat-Ranges/assets/107263697/ebf066f5-37dd-4e62-bd9c-b3184a1d1da1)

4. Then delete whatever extra actions that were imported that you don't need.

### Testing Actions (Optional)
You can "test" the trigger which uses the value of 42 for the amount by right-clicking the trigger:
![image](https://github.com/Haunter56/YouTube-SB-SuperChat-Ranges/assets/107263697/d79f3649-c6ed-4d91-9707-b0b9babca00b)

You can also create a test trigger and put in the amount you want to test

![image](https://github.com/Haunter56/YouTube-SB-SuperChat-Ranges/assets/107263697/567ac7e4-11fc-4483-b471-59dddab93f51)



![image](https://github.com/Haunter56/YouTube-SB-SuperChat-Ranges/assets/107263697/ce811501-5fa9-4745-acf7-f72d21e39ef4)

Then right-click the trigger to test:

![image](https://github.com/Haunter56/YouTube-SB-SuperChat-Ranges/assets/107263697/3454f719-713f-4525-9dc8-0e88a6d31747)





## Contributors
[Haunter](https://www.youtube.com/channel/UC9qO6-NFvWwhde5o2B_DMzQ) 👻
