---
toc: False
comments: True
layout: post
title: Ashwins CPT Individual Review
description: 
type: tangibles
courses: {'compsci': {'week': 24}}
---

## My Feature
For the CPT project I created a chest opening simulation based of the game Clash Royal. I also worked on the Login/Signup system and creating user roles such as admins. I also added things like a page to view our backend user database in the frontend, and a way to edit/delete users which would update our database. My individual feature displays 2 chests, one gold, and one legendary (Both from the game). If a user clicks the Gold chest, a function generates 8 random cards from the card database, and adds them to the logged-in user's collection. The other chest generates 4 cards, with a higher rarity. I created a seperate database for each users collection, so that t collection displayed would be based on the user you are logged in as. This database assigns card IDs to User IDs. Our team teach this trimester was JWT Admin/User roles. For this I created the admin role and with Dante's help making sure that the admin role was displayed in the cookie, I made it so only Admins could delete users. 

## What Is Clash Royale
Clash Royale is a very popular mobile game based around cards. There are about 120 cards in the game curently, and each card has a rarity and elixir cost, along with its seperate stats. Rarity can vary between, common, rare, epic, ledgendary, and champion, each one increasingly rare. There are several chests that can be won by winning battles, and each chest gives some cards to the player. Our enitre project followed this theme, and we created features like a deck builder, a tornament tracker, a custom survay, and a deck information page.

<Br>

# Collage Board Requirments

| Collegeboard Requirements | Me |
|------------------|------------------|
| Instructions for input from one of the following: the user, a device, an online datas stream, a file.  | I met the imput requirement by allowing a user to choose what chest they would like to open, and requiring them to click on the chest to generate the cards. <img src="https://Ashwinv93.github.io/CompSci/images/chest.png" alt="Description of Image"/> This is the event listener that checks for when a user clicks on the image of the chest, and calls for the API when the imput is triggered. <img src="https://Ashwinv93.github.io/CompSci/images/EventListener.png" alt="Description of Image"/>  |
| Use of at least one list (or other collection type) to represent a collectino of data that is stored and used to manage program complexity and help fulfill the users purpose.  | I met this requirment by using our database that contains all the data of each card in the game. This includes a photo of the card, the name, the elixer cost, the rarity, and the max level. Apart from that database, I also created another database that lets users save their collection of cards to their acount. It does this by mapping a users ID to the IDs of the cards in their collection. <img src="https://dantea-tech.github.io/student/images/CBcard.png" alt="Description of Image"/> <img src="https://Ashwinv93.github.io/CompSci/images/database2.png" alt="Description of Image"/>  |
| At least one procedure that contirubted to the program's intened purpose where you have defined: the name, return type, one or more parameters:  | This is one procedure I created that is what is triggered when the common chest is opened. The name is "get" and the parameter is "self". The return type is the response which converts the card data into json. <img src="https://Ashwinv93.github.io/CompSci/images/class.png" alt="Description of Image"/>|
| An algorithm that includes sequencing, selection, and iteration that is in the body of the selected procedure  |  This line is included in the procedure above. It is sequencing and sorting out cards in out database that have a rarity of common, rare or epic only and generating them. **cards = db.session.query(ClashRoyaleCard).filter(ClashRoyaleCard.rarity.in_(["common", "rare", "epic"])).order_by(func.random()).limit(8).all()**. After that 8 random cards are selected and only those 8 are displayed. The for loop iterates throught the cards generated and adds them to the collection for the user who is logged in. |
| Calls to your student-developed prodcedure:  |  This fuction in my frontend calls my backend prodcedure to populate a users collection based on what has been added to the database. It fetches the data and displays it or returns an error message. <img src="https://Ashwinv93.github.io/CompSci/images/call.png" alt="Description of Image"/>  |
| Instructions for output (tactile, audible, visual, or ) based on input and program functionality  |  This function populates the container I created, with the cards outputed from our database. This is a visual output since it just displays the images of each card. <img src="https://Ashwinv93.github.io/CompSci/images/function.png" alt="Description of Image"/> This is the displayed output <img src="https://Ashwinv93.github.io/CompSci/images/output.png" alt="Description of Image"/> |

<br>

# Video

| Collegboard Requirements | My Video |
|------------------|------------------|
| Input to program  | Seen in video, clicking on chest to run function  |
| At least one aspect of the functionality of your program|  A collection system demo'd in video which allows users to save the cards they collect from opening chests |
| Output produced by program:  |  The cards being generated into the container after click imput. They cards are also being outputed in the collection page, as more cards are collected  |
| My video does not have: | Any voice narration  |
| My video is: | Less than 1 minute in length and less than 30MB in file size.  |

[Link to my Video](https://drive.google.com/file/d/1T-40wnZCRUhn4pRfP3aoibgGuVOzfnhp/view?usp=sharing)
