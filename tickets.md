# Tickets
The following describes how tickets work, and how to set them up.

## Creating & Editing a Panel
To setup a ticket panel, simply do `/tickets panel create`. The bot will then take you through an interactive setup, and create your ticket panel.

![Example Ticket Panel](https://user-images.githubusercontent.com/49261529/113605552-ad320b00-95fb-11eb-9f05-12eeff7b45a8.png)

To edit a ticket panel, simply do `/tickets panel edit`. The bot ~~should~~ will display options and possible values.

![Example Panel Edit](https://user-images.githubusercontent.com/49261529/113606571-0cdce600-95fd-11eb-8f27-8905dfc6a5e5.png)

To see a full list of options, simply run `/tickets panel options`.

## Deleting a Panel
If you wish to delete a ticket panel, just run `/tickets panel delete` and confirm you would like to delete the panel.

### Warning
This will remove all tickets associated with this panel from the database, meaning you will not be able to manage them.

## Making Tickets
To create a ticket, simply go to your ticket panel and select the button. The bot will then either make a ticket, or tell you that it can't.

![Example Ticket](https://user-images.githubusercontent.com/49261529/113606254-9c35c980-95fc-11eb-979e-c9ad460c8523.png)

## Managing Tickets

Managing tickets is quite simple. 

To close a ticket, either select the `Close Ticket` button at the top of the ticket, or run `/tickets close` within the ticket.

To rename a ticket, run `/tickets rename` within the ticket.

To add someone to a ticket, run `/tickets add` within the ticket.

To remove someone from a ticket, run `/tickets remove` within the ticket.

To save a transcript of a ticket or reopen a ticket, click the corresponding buttons.

To delete a ticket, run `/tickets delete` within the ticket, or select the delete button after the ticket has been closed.
