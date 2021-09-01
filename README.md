# Assistant
## Create assistant

Only need create account in [IBM Cloud](https://cloud.ibm.com/). When you have account, only need create a service of *Watson Assistant*:
- Click on bar search and write *Watson Assistant*:![image](https://user-images.githubusercontent.com/48229215/131759109-a8d5dd30-f788-4868-9ac3-f82f7fc718d2.png)
- Now, just select a plan and put a name to the service. En my case I'm using a free plan
- Click in the option *Launch Watson Assistant*:![image](https://user-images.githubusercontent.com/48229215/131759398-88409beb-f189-4013-9895-61906551c54d.png)
- By default you have a skill with name *My first skill*. If you want create you personal skill, only select the option *Skill* -> *Create skill* -> *Dialog skill*->complete the form->*Create*
### Intents - Entities - Dialog
Now, the first version only need configured this:
- Intents: The intention that the user has when interacting with the bot.
- Entities:"Variables. These are the entities that go together with the intent. For example, "I want to make a reservation for {a trip, a flight, a hotel}". Trip, flight and hotel are entities and making a reservation is my intention.
- Dialog:Dialog flow programming. It works sequentially, this means that it looks for conditionals in each one. If it finds an intention, if it finds an entity or a combination of both, the bot will answer something in particular.
#### Intents
In this project i have three intents:
- store.locatios: Where is the store?
- store.hours: What are your store hours?
- store.order.new: Order something

#### Entities
- Size: Small - Medium - Large

#### Dialog
In this case in each node I put a condition, this conditios is recognize the intent.
