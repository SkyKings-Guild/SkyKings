# Tickets
The following describes how tickets work, and how to set them up.

## Creating & Editing a Panel
To setup a ticket panel, simply do `k!tickets panel create`. The bot will then take you through an interactive setup, and create your ticket panel.

![Example Ticket Panel](https://user-images.githubusercontent.com/49261529/113605552-ad320b00-95fb-11eb-9f05-12eeff7b45a8.png)

To edit a ticket panel, simply do `k!tickets panel edit <panel> <option> <value>`. For example, if you wanted to set a transcript channel, you would do `k!tickets panel edit <panel> transcript_channel #transcripts`.

![Example Panel Edit](https://user-images.githubusercontent.com/49261529/113606571-0cdce600-95fd-11eb-8f27-8905dfc6a5e5.png)

To see a full list of options, simply run `k!tickets panel options`.

## Deleting a Panel
If you wish to delete a ticket panel, just run `k!tickets panel delete <panel>` and confirm you would like to delete the panel.

### Warning
This will remove all tickets associated with this panel from the database, meaning you will not be able to manage them.

## Making Tickets
To create a ticket, simply go to your ticket panel and react to the message with `📩`. The bot will then either make a ticket, or tell you that it can't.

![Example Ticket](https://user-images.githubusercontent.com/49261529/113606254-9c35c980-95fc-11eb-979e-c9ad460c8523.png)

## Managing Tickets

Managing tickets is quite simple. 

To close a ticket, either react with 🔐 to the message at the top of the ticket, or run `k!tickets close` within the ticket.

To rename a ticket, run `k!tickets rename <new name>` within the ticket.

To add someone to a ticket, run `k!tickets add <member>` within the ticket.

To remove someone from a ticket, run `k!tickets remove <member>` within the ticket.

To save a transcript of a ticket, react with 📝 to the ticket closing message.

To reopen a closed ticket, react with 🔓 to the ticket closing message.

To delete a ticket, run `k!tickets delete` within the ticket, or react with 🗑 to the ticket closing mesage.
