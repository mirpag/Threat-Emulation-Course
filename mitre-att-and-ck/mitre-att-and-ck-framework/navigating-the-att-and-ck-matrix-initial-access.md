---
cover: >-
  https://images.unsplash.com/photo-1523961131990-5ea7c61b2107?crop=entropy&cs=srgb&fm=jpg&ixid=MnwxOTcwMjR8MHwxfHNlYXJjaHw2fHx0ZWNofGVufDB8fHx8MTY0NjU5NDQzNA&ixlib=rb-1.2.1&q=85
coverY: 0
---

# Navigating the Att\&ck Matrix - Initial Access

Reconnaissance and Resource Development were added on later in the process of developing the Mitre Att\&ck framework. These help provide information on how adversaries start to carry out their operation.&#x20;  The goal of Initial Access is to get access to a system or data to carry out their mission. They do that via techniques such as drive-by compromise and phishing.

With phishing, there are techniques line the ones below. Click on one of the techniques and it gives you a definition of phishing. Notice the sub-techniques. Click on a sub-techinique like spear-phising attachment. Each sub-technique has its own ID. The tactic is initial access. This is the goal.&#x20;

![](../../.gitbook/assets/phishing.PNG)

Below are the known platforms in which spear phishing works. THe reason it has Linux, Windows, and Mac OS is because those are the most common ones on the internet. Yes, there are other operating systems out there, though they're including these particularly because Mitre have more information about them. What this means here is that the spear phishing attachment sub-technique applies to Linux, Windows, and Mac OS. To get more information about other operating systems, they're updated here.

![](../../.gitbook/assets/platforms.PNG)

Data sources to detect spear-phishing are invaluable for a SOC. It provides information about data sources that can detect spear-phishing - whether successful or unsuccessful. If you have access to email messages, its content, and attachment, that's how you can monitor for spear-phishing.  A web proxy also helps because it could block the malicious domain within the email if a user clicks on it.&#x20;

The CAPEC ID means the TTP is a well known attack and this is a generic definition of spearphishing.  Clicking on the link provides more information.

![](../../.gitbook/assets/capec.PNG)

Scroll down and there are procedure examples. What does that mean? The "G" is displaying groups that are known to use spearphishing. The group admin@338, has sent emails with malicious word Microsoft Office documents attached so they're telling you about this group's behavior to obtain initial access. Accordingly, if an organization is the type the group is known to attack, additional controls should be in place to mitigate, detect, and alert on malicious spear-phishing email.&#x20;

![Spear Phishing Procedure Examples](../../.gitbook/assets/procedure\_examples.PNG)

Click on the group ID to get more information about that known threat group. This is again, one of the benefits of the att\&ck framework. It maps out the the TTPs, techniques, tactics and procedures for known threat groups. Those are all the techniques that are used by this particular threat actor.&#x20;

![Threat group admin@338](../../.gitbook/assets/admin@338.PNG)

This is a type of software they use. Just like with our tactics and techniques, each group has an ID. Then, attribution for who provided the information about the threat group and other metadata you see below.&#x20;

![Software utilized by admin@338](../../.gitbook/assets/software.PNG)

Same thing with software. This is BUBBLEWRAP and it is a backdoor. It has its own ID. The type is malware, and the platform it impacts is Windows. Now a threat hunter can analyze Windows platforms for the software BUBBLEWRAP if it is used by threat actors known to target similar organizations.&#x20;

![](../../.gitbook/assets/bubblewrap.PNG)

Alright, here's some of the techniques that are used for BUBBLEWRAP, as you see right here. You can see Groups that use the software.

Here are the techniques that are used by BUBBLEWRAP. It can communicate using SOCKS, T1095. It can communicate using HTTP or HTTPS, T1071.

*NOTE: Be careful not to fall down the rabbit hole and get caught up in the many links that are available on the Att&ck site.*&#x20;

![](../../.gitbook/assets/techniques\_and\_groups.PNG)

At the very bottom, are references to get more information about the adversary so, essentially, Mitre gives you the high level overview or the metadata. Then, you can click on the reference link and read more information that's provided by FireEye.&#x20;

![BUBBLEWRAP References](../../.gitbook/assets/references.PNG)

Let's go back to the sub-technique of spear phishing. Again, read information about it. Procedures, all the groups, etc. Other groups use this because it's highly effective. If an organization doesn't have a public presence, meaning their web servers, mail servers and all other services are hosted out in the cloud, then the adversaries may use other techniques to get inside the organization. *Spear-phishing is a very effective method of initial access into an organization*&#x20;

![Spear Phishing Attachment Procedure Examples](../../.gitbook/assets/procedure\_examples.PNG)

There are mitigations to all of the techniques. Sub-techniques are going to have mitigation documented. Below are some mitigations to put in place to help minimize the impact of spear-phishing.&#x20;

![Spear phishing attachment Mitigations ](../../.gitbook/assets/mitagations2.PNG)

The detections listed in the att&ck framework are a great resource for SOC analyst and threat hunters. They can see if they have the proper insights and are obtaining the proper logs in order to provide a more comprehensive insight into the organization. Detections are going to help identify when an attack is imminent, or about to occur, or attempt to occur. Antivirus may prevent someone from opening a malicious document.  Any alert for spear-phishing should be investigated to determine if it is a known threat actor targeting the organization. That should send of alarm bells and a thorough review of logs and threat hunting should occur.&#x20;

![Spear phishing attachment Detection](../../.gitbook/assets/detection2.PNG)

There's a lot of information and references about this TTP because *spearphishing is a very, very common technique used by threat actors*. Red teams, the good 'ackers will tell you that this is one of their last resorts. If they can't get in otherwise, this is almost always going to work. Not always, but almost always.&#x20;

![Spear phishing attachment references](../../.gitbook/assets/references2.PNG)
