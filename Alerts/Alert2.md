Web Alert 3 :

<img src="./media1/media/image1.png"
style="width:6.5in;height:3.10069in"
alt="A screenshot of a computer AI-generated content may be incorrect." />

This is the scenario here

As usual we will examine the IP on virus total –

<img src="./media1/media/image2.png"
style="width:6.5in;height:2.82917in"
alt="A screenshot of a computer AI-generated content may be incorrect." />

Nothing on virus total but this isn’t enough for deducing nothing’s
malicious .

Gathering client details :

<img src="./media1/media/image3.png"
style="width:6.5in;height:3.73681in"
alt="A screenshot of a computer AI-generated content may be incorrect." />

Let us check the logs now .

<img src="./media1/media/image4.png"
style="width:6.5in;height:2.63958in"
alt="A screenshot of a computer AI-generated content may be incorrect." />

<img src="./media1/media/image5.png"
style="width:6.5in;height:2.66736in"
alt="A screenshot of a computer AI-generated content may be incorrect." />

Attacker initially established trust with the victim by sending some
legitimate requests without any malice you can see the request urls
being completely normal until the alert Url
.<img src="./media1/media/image6.png"
style="width:6.5in;height:2.95486in"
alt="A screenshot of a computer AI-generated content may be incorrect." />

The request url ?s is kinda suspicious as it looks like ls . But I don’t
think it is with malicious intent as it may be triggered with skil-‘ls’
. Let us check the process

<img src="./media1/media/image7.png"
style="width:6.5in;height:3.29306in"
alt="A screenshot of a computer AI-generated content may be incorrect." />

EDR confirming multiple requests .

<img src="./media1/media/image8.png"
style="width:6.5in;height:2.99792in"
alt="A screenshot of a computer AI-generated content may be incorrect." />

The terminal history doesn’t show any ls command being executed so I
don’t think anything is suspicious here . But I deduced the ?s to be
malicious so I lost points there .

The lesson from this is don’t have threat finding mindset but rather
look everything as normal alert then escalate .

<img src="./media1/media/image9.png"
style="width:6.5in;height:2.67569in"
alt="A screenshot of a computer AI-generated content may be incorrect." />
