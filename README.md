# Interview-Task

![alt text](https://github.com/olufemiode554/Interview-Task/blob/83acd36e7914affdb870e4f918d4250e844028e2/Assessment%20%20Task/Transformed%20Data/Transforming%20Data%20on%20Excel.xlsx)

Task for the excel Data:

Join queue events: that show Service Users (SUs) joining the chat queue to request a chat, and when they left the queue. SUs are removed from the queue, either by manually removing themselves out of choice, or by manual removal by a practitioner if they are not going to get a chat, or when they are successful and a chat with them is started.

Chat start events: a chat session starting, which can follow either a join queue event or be a booked chat 

Not all SUs have a successful chat, after joining the queue. Only the SUs with a Chat Start event have a chat.

Please provide insight on the queue behaviour, and in particular looking at SU chat attempts, wait times and queue success rates.

How long are people waiting and does this change throughout the day?
Do unsuccessful people make multiple attempts?
What are the demand and success patterns?
I started by creating more columns on the excel table 'JOIN QUEUE EVENTS AND CHAT START EVENTS', Where i wrote formulas to create time (Time_on_Chat),=TEXT(C2-B2,"hh:mm:ss")

I created another column (Day_on_chat) =TEXT(B2,"d/mm")

I created another column (Day_end) =TEXT(C2,"d/mm")

I created another column (Day_diff) ==G2-F2

I created another column (Day_time_diff) =H2&":"&E2

After all this steps, I was able to import the data to SSMS


[Link to Dashboard](https://1drv.ms/p/s!Au_vlCOcdFpRiXz4ThZ1BOzMIXBy?e=RrBecz)
