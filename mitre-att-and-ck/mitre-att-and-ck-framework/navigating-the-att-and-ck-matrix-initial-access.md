---
cover: >-
  https://images.unsplash.com/photo-1523961131990-5ea7c61b2107?crop=entropy&cs=srgb&fm=jpg&ixid=MnwxOTcwMjR8MHwxfHNlYXJjaHw2fHx0ZWNofGVufDB8fHx8MTY0NjU5NDQzNA&ixlib=rb-1.2.1&q=85
coverY: 0
---

# Navigating the Att\&ck Matrix - Initial Access

So for the most part, these two \[Reconnaissance and Resource Development], were added on later in the process of developing the Mitre Att\&ck framework. It is updated on a pretty routine basis. These help provide information on how adversaries start to carry out their operation.&#x20;

But what they want to get to is this initial access. This is number one, this is how they get into the system. This is really important. So this initial access, this is a start of their campaign. This is where they're trying to get into your network. They do that via techniques such as drive-by compromise and phishing.

Let's look at phishing because people are very familiar with phishing. With phishing, you have these techniques. If you open this up, it gives you a definition of what phishing is just like before. But I want you to notice over here, the act of ADDIE for this technique. Here are the sub techniques. If we click on one of these, one type of fishing is spearfishing attachment. And again, it has its own ID dot 001 sub-technique of phishing. The tactic is initial access. This is the goal tactic.&#x20;

![](../../.gitbook/assets/phishing.PNG)

Now platforms. These are the known platforms in which spear phishing works. Now the reason why I have Linux, Windows, and Mac OS is because those are the most common ones on the internet. Yes, there are other operating systems out there, but they're targeting these particularly because they have more information about these. What this means here is that the spear phishing attachment sub-technique applies to Linux, Windows, and Mac OS. To get more information about other operating systems, they're updated here.

![](../../.gitbook/assets/platforms.PNG)

Once again, this is invaluable for our SOC analyst data sources. This is telling you how you can detect spear phishing attacks or attempts. If you have access to application logs, application log content, or network traffic, that's how you can monitor for spear phishing.&#x20;

And then this, CAPEC ID. If we open this in another tab, you'll see that it's the Common Attack Pattern Enumeration and Classification. Meaning this is a well known attack. And this is a generic definition of what spear phishing is. So you can click on this to get more information.

![](../../.gitbook/assets/capec.PNG)

As we scroll down, you start to see procedure examples. Now what does this mean? What we're looking at are groups in a G right there, that means groups. This is a group that is known to use spear phishing. The group admin@338, has sent emails with malicious word Microsoft Office documents attached. So they're telling you about this group here.&#x20;

![Spear Phishing Procedure Examples](../../.gitbook/assets/procedure\_examples.PNG)

If I click on this group ID, I get more information about that known threat group. This is again, one of the benefits of the attack framework. It maps out the the TTPs, techniques, tactics and procedures for known threat groups. These are all the techniques that are used by this particular threat actor. They do a lot of different things on the system.&#x20;

![Threat group admin@338](../../.gitbook/assets/admin@338.PNG)

This is a type of software they use. This s, this is a type of software. Just like with our tactics and techniques, each group has an ID. Then, attribution for who provided the information about the threat group and other metadata you see here.&#x20;

![Software utilized by admin@338](../../.gitbook/assets/software.PNG)

Same thing with software, but click on this s here. This is BUBBLEWRAP. You can see this is a backdoor. It has its own ID. Here's the associated software right here. The type is malware, and the platform it impacts is windows. So once again, good information. Now you know that you can look at Windows platforms for the software BUBBLEWRAP.&#x20;

![](../../.gitbook/assets/bubblewrap.PNG)

Alright, now, here's some of the techniques that are used for BUBBLEWRAP, as you see right here. And you can see groups that use the software.

Here are the techniques that are used by BUBBLEWRAP. It can communicate using SOCKS, T1095. It can communicate using HTTP or HTTPS, T1071. You see how this works. So you know, you could get caught up in a almost like a Google search. You look for one thing, and you end up to minutes later at something that you didn't even intend to go to. You want to be sure that you rein it in a little bit, and not get too caught up into all the links that you have here.&#x20;

![](../../.gitbook/assets/techniques\_and\_groups.PNG)

At the very bottom, you also find references to get more information about the adversary. So essentially, Mitre gives you the high level overview or the metadata. Then, you can click on this reference link and read more information that's provided by FireEye. Okay, so this is a threat group.&#x20;

![BUBBLEWRAP References](../../.gitbook/assets/references.PNG)

Let's go back again. And back to our sub-technique of spear phishing. Again, read information about it. Procedures, all the groups, etc. You can see between some groups in the procedure examples is some software. S, software keeps going down here. Other groups use this because it's highly effective. If an organization doesn't have a public presence, meaning their web servers, mail servers and all other services are hosted out in the cloud, then the adversaries are going to use other techniques to get inside the organization. Spear phishing is probably one of the most effective. You send it to the right number of people or the right people to open an attachment or click a link, and it impacts the organization.&#x20;

![Spear Phishing Attachment Procedure Examples](../../.gitbook/assets/procedure\_examples.PNG)

Now, once again there are mitigations to all of your techniques. Sub-techniques are going to have mitigation documented. You can see here these are some mitigations to put in place to help minimize the impact of spear phishing. The mitigation links have more information about these as well.&#x20;

![Spear phishing attachment Mitigations ](../../.gitbook/assets/mitagations2.PNG)

Right, and then detection units and insights into email gateways. This is a really great resource for SOC. They can see if they have the proper insights and are obtaining the proper logs in order to provide a more comprehensive insight into the organization. Detections are going to help you identify when an attack is imminent, or about to occur, or attempt to occur. Your antivirus may prevent someone from opening a malicious document. In that case, you're going to get a virus alert, an antivirus alert. Then you can take action based on that.&#x20;

![Spear phishing attachment Detection](../../.gitbook/assets/detection2.PNG)

You can see there's a lot of information and references about this because spear phishing is a very, very common technique. Red teams, the good hackers will tell you that this is one of their last resorts. If they can't get in otherwise, this is almost always going to work. Not always, but almost always.&#x20;

![Spear phishing attachment references](../../.gitbook/assets/references2.PNG)
