---
layout: post
title: Putnam Lab QR code inventory 
date: '2024-04-23'
categories: Protocols
tags: [Inventory, lab organization, QR code Protocol]
---

Materials: 

- Computer
- Cryo babies printer paper
- Printer with black ink
- Scissors


#The goal

1. Each freezer and fridge has a QR code on the front that brings you to the inventory spreadsheet for the location you are looking at.
2. You will scan this QR code and search for what shelf you are looking for.
3. Once you find the box you are looking for you can can that box to get a full inventory metadata list for the project that the box you have falls under. 
4. You will be able to scan and update spreadsheets in real time if you remove samples. 
5. Additionally, there are three QR codes around each working location that you may scan when you are looking for something in that location.
6. You will also be able to update the inventory by scanning them as you use resources or restock anything!


Set up: 

There are two possible set ups

1. Directly in Google sheets
2. Using [QR monkey](https://www.qrcode-monkey.com/#)

####Directly in Google sheets

Pros: Faster, ability to create bulk QR codes, ability to print many QR codes at a time wasting less paper, static QR code (meaning it will not change unless the document is deleted), able to put QR code on excel (all in one place) no seperate documents needed to keep things together

Cons: Less information about guaranteed life of QR code, no personalized logo

####Using QR monkey

Pros: Customizable (ability to put Putnam lab logo), guaranteed for life static QR code, 

Cons: Takes longer to create as a new one needs to be created for each different metadate link individually


Protocol for google sheets

- Using [Putnam Lab Master Cold Storage Inventory](https://docs.google.com/spreadsheets/d/1IMYmnNsN4D9cFbgLVdGKz67Albb3LxEyBh2GMtREMPU/edit#gid=2010168651) there will be a column on the top right that states "Link to sample metadata"
- You will add the link for the metadata of the project that correlates with the samples in the box to this column
- To the right there will be a column that states QR code
- In order to generate a QR code you will first you will put the formula

> =ENCODEURL(A1)

You will replace A1 with the cell that contains the link to the sample metadata that you intend on making a QR code for.

Once that is completed you will now select the cell and in the fx bar at the top of the google sheets document. Enter the following command before the ENCODEURL(A1)

> ="https://api.qrserver.com/v1/create-qr-code/?size=150x150&data="&

The updated formula will look like this 

> ="https://api.qrserver.com/v1/create-qr-code/?size=150x150&data="&ENCODEURL(A1)

You are almost done! Now in order to turn this into a functioning very beautiful QR code you will add in the word "IMAGE" for a finished formula looking something like this 

> =IMAGE("https://api.qrserver.com/v1/create-qr-code/?size=150x150&data="&ENCODEURL(A1))
 At this point you should see a QR code 

You can select all the QR codes you would like and can also select their sample box label and can print all on cryogenic paper that will stick on the box.



###The other option is to do it in [QR monkey](https://www.qrcode-monkey.com/#)

To do this you will...

1) Select the link to the google sheet needed and enter it into where it says link

2) You can select customize in order to enter the Putnam lab logo

3) In order to print multiple at a time, I recommend making a google sheet with the label of what the QR code includes.

4) These can be printed, cut, and placed on the box 
















