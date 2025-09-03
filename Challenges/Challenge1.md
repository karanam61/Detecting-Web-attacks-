Web attacks Challenge 1 :

<img src="./media2/media/image1.png"
style="width:6.5in;height:2.43056in"
alt="A screenshot of a computer AI-generated content may be incorrect." />

We’ve go the source and destination Ips . Let us start with log
management to see if there any additional exchanges between the Ips.

<img src="./media2/media/image2.png"
style="width:6.5in;height:3.50347in"
alt="A screenshot of a computer AI-generated content may be incorrect." />

Port 443 says its being communicating through https .

Status code is 500 meaning . **500**: your app/code crashed. So most
probably the attack isn’t successfyk but we should cross check it at
Endpoint detection and check for processes to see if there’s anything
returned . Also the response size is 0 .

Let us look at the request now :

<https://172.16.17.13/?file=../../../../etc/passwd>

This suspicious as a random cloud provider is requesting for
etc/password file going up the heirar

<img src="./media2/media/image3.png"
style="width:6.5in;height:3.04653in"
alt="A screenshot of a computer error AI-generated content may be incorrect." />

Seems like the source Ip address belongs to a company called Tencent
cloud which is obviously webhosted .

<img src="./media2/media/image4.png"
style="width:6.5in;height:3.41389in"
alt="A screenshot of a computer AI-generated content may be incorrect." />

And just 1/94 security vendor flagging .

The destination is a letsdefend.io company webserver owned by
letsdefend.io

The traffic is from the internet .

**Last Login:**

Feb, 19, 2022, 01:01 PM

Now when I check the process , webbrowser history I couldn’t see
anything that is suspicious .

<img src="./media2/media/image5.png"
style="width:6.5in;height:3.63333in"
alt="A screenshot of a computer AI-generated content may be incorrect." />

<img src="./media2/media/image6.png"
style="width:6.5in;height:2.90486in"
alt="A screenshot of a computer AI-generated content may be incorrect." />

As the suspicion was on Local file inclusion the terminal has to be
accessed to go up or down the hierarchy .

As there is nothing that supports the alert it is not a true positive it
is a false positive as we don’t see anything suspicious .

<img src="./media2/media/image7.png"
style="width:6.5in;height:2.94514in"
alt="A screenshot of a computer AI-generated content may be incorrect." />

It was a possible LFI attack but wasn’t successful .
