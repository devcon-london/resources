# Problem: Real time leader boards

## Scenario

We have a user population of 7 million people worldwide, each of whom has a method of syncing data from a fitness device (like the Fitbit for example) to the cloud via their mobile device (iOS and Android). We have been briefed to create a way for users to participate in leader board style games based on this data. We will be provided with a real-time feed of the sync data from the cloud servers.

## Requirements

- Devices can be configured by the owner for the frequency of syncing to the cloud. This can be every 30 seconds, minute, 5 minutes, 20 minutes or every hour.
- Each game will have its own leader board, which ranks people depending on calories burned for the duration of their participation in this game. E.G. if the game started on 1st Jan then only calories earned from this point onwards count for this game.
- Each game can have as many users as wish to sign up
- Each game has a finite time to exist – the default being 2 weeks. After 2 weeks the game leader board will still be visible but no scores will be updated
- Each user must be able to participate in as many games as they wish as easily as possible.
- Any user can invite anyone else to join a game
- Leader board views must be correct as quickly as possible once any user syncs relevant data
- Leader boards are publicly visible – anyone can see them
- There are 3 views on any given leader board
- Contextual, that is my position with the surrounding 10 people. E.G. is I am in position 25 I see the section of the board from position 20 to 30
- Friends, that is a subset of the leader board showing scores for me and my friends, in the correct order. Assume there is a service we have access to that when supplied with a user id returns all the friends ids for that user.
- Full. The whole leader board can be displayed and paged through
