# Threat-Model-101
My notes on how to perform a threat model

Reference: https://arstechnica.com/information-technology/2017/07/how-i-learned-to-stop-worrying-mostly-and-love-my-threat-model/

Questions I ask myself:
1. What are you doing?
- The thing that you are trying to do, and what information is involved
2. What can possible go wrong? And who do you need to protect the not desirable action from?
- How what you are doing can expose information that is not desirable and from whom (script kiddie, professional hackers vs nation state actors)
3. How likely is it that the underiable can happen and what are you going to do about it?
- Is it easily exploitable from a easy to access tool vs series of conditions that needs to met to make this happen
- Identify changes that can be made either config or coding wise to prevent the underiable
4. How much time and effort is it required to
    a. place controls (legacy applications)
    b. fix the issue.
5. Did you do a good job of it?
- Re-assessing to see how much risk was reduced.


Thoughts:
1. For issues like SQLi, it doesn't make sense to spend a lot of effort threat modeling - since the issue can be addressed by using safe libraries for e.g parameterized queries vs spending time threat modeling.