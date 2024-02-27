---
toc: False
comments: True
layout: post
title: Ashwins CPT Individual Review
description: 
type: tangibles
courses: {'compsci': {'week': 14}}
---

## My Feature
For the CPT project I created a chest opening simulation based of the game Clash Royal. I also worked on the Login/Signup system and creating user roles such as admins. I also added things like a page to view our backend user database in the frontend, and a way to edit/delete users which would update our database. My individual feature displays 2 chests, one gold, and one legendary (Both from the game). If a user clicks the Gold chest, a function generates 8 random cards from the card database, and adds them to the logged-in user's collection. The other chest generates 4 cards, with a higher rarity. I created a seperate database for each users collection, so that t collection displayed would be based on the user you are logged in as. This database assigns card IDs to User IDs. Our team teach this trimester was JWT Admin/User roles. For this I created the admin role and with Dante's help making sure that the admin role was displayed in the cookie, I made it so only Admins could delete users. 

## What Is Clash Royale
Clash Royale is a very popular mobile game based around cards. There are about 120 cards in the game curently, and each card has a rarity and elixir cost, along with its seperate stats. Rarity can vary between, common, rare, epic, ledgendary, and champion, each one increasingly rare. There are several chests that can be won by winning battles, and each chest gives some cards to the player. Our enitre project followed this theme, and we created features like a deck builder, a tornament tracker, a custom survay, and a deck information page.

<Br>

## Collage Board Requirments

| Collegeboard Requirements | Me |
|------------------|------------------|
| Instructions for input from one of the following: the user, a device, an online datas stream, a file.  | I met the imput requirement by allowing a user to choose what chest they would like to open, and requiring them to click on the chest to generate the cards. <img src="https://Ashwinv93.github.io/CompSci/images/chest.png" alt="Description of Image"/>  |
This is the event listener that checks for when a user clicks on the image of the chest, and calls for the API when the imput is triggered.
<img src="https://Ashwinv93.github.io/CompSci/images/EventListener.png" alt="Description of Image"/>  |
| Use of at least one list (or other collection type) to represent a collectino of data that is stored and used to manage program complexity and help fulfill the users purpose.  | I met this requirment by using our database that contains all the data of each card in the game. This includes a photo of the card, the name, the elixer cost, the rarity, and the max level. Apart from that database, I also created another database that lets users save their collection of cards to their acount.
<img src="https://Ashwinv93.github.io/CompSci/images/database2.png" alt="Description of Image"/>|
| At least one procedure that contirubted to the program's intened purpose where you have defined: the name, return type, one or more parameters:  | This procedure has a name(post), a return(response), and parameters(self): <a href="https://ibb.co/pjDPHxs"><img src="https://i.ibb.co/d49cNr3/procedure.png" alt="procedure" border="0"></a>  |
| An algorithm that includes sequencing, selection, and iteration that is in the body of the selected procedure  | This function shows the sequencing, selection, and iteration through a list of meme images: <a href="https://ibb.co/Zg02DK5"><img src="https://i.ibb.co/3FnRZW2/sequencing.png" alt="sequencing" border="0"></a>  |
| Calls to your student-developed prodcedure:  | calling queryImages: <a href="https://imgbb.com/"><img src="https://i.ibb.co/SnW6Kyf/calling.png" alt="calling" border="0"></a>  |
| Instructions for output (tactile, audible, visual, or ) based on input and program functionality  | This code is the fetch that displays the image based off the users inputted image and top+bottom text: <a href="https://ibb.co/Q8WJmkJ"><img src="https://i.ibb.co/28zFKSF/fetch.png" alt="fetch" border="0"></a>  |


Imput:

- Use of at least one list (or other collection type):

