# Attack surface in cloud service models
## Category
### Emerging real-world attacks targeting hypervisors
#### covert channel
When one of VM Virtualbox is invade, the data may be transmit through the covert channel.

Thus, the data in other VM Virtualbox will be stolen. That's scary

The following figure illustrates the covert channel between VM Virtualboxes.

![image](https://user-images.githubusercontent.com/75050655/227123271-abea08cc-9bf1-4fc4-a6de-d93760796ee2.png)

#### Side-channel attack
It refers to guess sensitive information with known information.

Its concept is same as guess one's thought through observing one's behavior.

For example, a hacker can guess what application runs on the victim's device through its CPU utilization, battery status etc.

Although it is NOT find an exact correct solution (since hacker just guess it), the hacker may have the idea which is came up with the guess.
##### Ref
https://en.wikipedia.org/wiki/Side-channel_attack

## Summary
![image](https://user-images.githubusercontent.com/75050655/227120275-a30e20ff-1aba-44aa-a606-639ef29f4f14.png)
