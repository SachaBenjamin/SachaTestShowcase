# Research for a quick look at QA Automation to test market.voxies.io

## Step 1 : Getting general Knowledge about how QA Automation work and the Softwares needed

I spent the first few minutes on Google and GPT trying to find what I would need to start testing a website with web3 / blockchain integration like the market.voxies website. I settled on Node.js and Playwright to run the automation tests. Node.js was bundled with the Node Package Manager that allowed me to install everything needed (Playwright, Playwright-test). I did all of this using CMD prompt.

<img width="1664" height="472" alt="2025-08-01 17_19_48-2025-08-01 16_53_57- png" src="https://github.com/user-attachments/assets/20381da0-2be8-484c-a6b1-7e3cfcae734b" />

## Step 2 : Deciding and identifying what I would test 

After everything was installed, I decided to focus on testing the header buttons of the website. I wanted to test the buttons straight away but ran into some errors (Playwright couldn't find them). I needed to make sure they are able to be seen by the script first so I created a js file called "Button-Test" then with the help of some research and GPT produced a script to identify all the buttons in the header. Once the result came in I compared it to the actual website to see if it matcthed, and it did. 

<img width="1142" height="607" alt="2025-08-01 17_26_45-C__Users_sacha_voxies-automation_button test js - Notepad++" src="https://github.com/user-attachments/assets/6aa2f1df-cb28-4f14-bcba-4823198125ac" />
<img width="1920" height="993" alt="2025-08-01 17_47_06-Editing SachaTestShowcase_README md at main · SachaBenjamin_SachaTestShowcase - " src="https://github.com/user-attachments/assets/5419f9b9-84fe-48ed-98da-24c60ce4bc5a" />



## Step 3 : Testing all the buttons 

With all the buttons correctly identifiable by Playwright, it was time to test them. I modified the script used to find the buttons to actually click them. The test ran successfuly this time and all header buttons of market.voxies were visible and clickable! 

<img width="1180" height="785" alt="2025-08-01 17_33_42-C__Users_sacha_voxies-automation_button test js - Notepad++" src="https://github.com/user-attachments/assets/73cc04f4-6d6a-48ae-afca-5c5714264a20" />

## Next Steps 

The next step would be to test every single buttons of the website, the filters etc. (Basically every interactive elements) Then it would involve testing logins and blockchain purchases. I've research it and it is possible to use Automation to run test using test wallets. It would simulate a user making a purchase, then the script is able to navigate Polygonscan, enter the transaction hash and verify the result. I think we can even query the hash directly using a library like ethers.js. The script can compare the sender and receive, make sure everything matches then validate the transaction. 

<br>
<br>
<br>

# Showcase for Giftogames Workflow

I built this workflow and bug template from scratch for Giftogames’ QA pipeline. I've mainly used Jira and Google Sheet to set it up.

### Workflow 

Here is the Workflow for Giftogames, I've set up a workflow for bugs, feedback and tasks that the developers use on their day to day tasks.

<img width="1864" height="787" alt="Workflow" src="https://github.com/user-attachments/assets/9157b099-7876-405c-a33a-410acc6fd68d" />



### Board

This is the Board, where all the relevant bugs, tasks and feedbacks are displayed : 

<img width="1706" height="1021" alt="Board" src="https://github.com/user-attachments/assets/584727f0-ee78-4385-a163-ea1c2258378e" />



You can use filters to only show bugs, tasks or feedbacks :

![Filters](https://github.com/user-attachments/assets/34a5b377-bb4f-4b06-bb74-1720b59cdda3)



### Bug Fields

All the different fields the QA testers have to fill to enter a bug : 

![Fields](https://github.com/user-attachments/assets/5f4d05c3-6cae-43b4-ac6d-3a0456237728)


### Bug Template 

A detailed template for entering bugs, useful for new testers that might join the project later as we scaled it up : 

<img width="1156" height="1008" alt="Template1" src="https://github.com/user-attachments/assets/74b2a852-0526-40fa-9836-19eabb878d17" />

<br><br>

<img width="1176" height="1030" alt="Template2 png" src="https://github.com/user-attachments/assets/fad71a6c-2ff8-4783-8ede-887cb09b6345" />

<br><br>

<img width="1183" height="1033" alt="Template3 png" src="https://github.com/user-attachments/assets/8a9303db-df81-4213-b5c1-b052a08c2409" />

### Smoketest Template

The Smoketest template I have build for testing the build before pushing a major update. Every single action you can do in the game is listed with a status, then if failed a bug is added on excel that redirects to the Jira for clear visibility. Here is some part of the smoke test (It would be too long to list everything) : 

Start of the Smoketest : 

<img width="971" height="824" alt="2025-07-28 19_20_25-Smoketest 1 1 0(11) xlsx - Google Sheets - Brave" src="https://github.com/user-attachments/assets/162a3a98-0412-46ee-be7f-39d3a059de7f" />

End of the Smoketest : 

<img width="971" height="824" alt="2025-07-28 19_21_55-Smoketest 1 1 0(11) xlsx - Google Sheets - Brave" src="https://github.com/user-attachments/assets/87beda5c-0801-4855-aef3-3d9e4d08b45e" />






