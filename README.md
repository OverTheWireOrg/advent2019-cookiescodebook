# Cookie Codebook

*The [OverTheWire Advent Bonanza 2019](https://advent2019.overthewire.org) challenge for Friday 13 December 2019*

Elves Inc., the consortium behind Santa's baking goods, wants to surprise Santa
with new varieties of cookies for this Christmas.  With that goal in mind, they
have recently decided to modernize and produce cookies on an industrial scale
using a Smart Cookie Baking Machine.  Unfortunately, the instructions for the
machine were eaten by a reindeer, and nobody really knows how to program this
machine.

After this massive disaster, Elves Inc. needs your help to save Christmas.  In
particular, they need new cookie recipes, written in a variety of programming
languages.  The hope is that at least one of these programming languages will
be able to program the Smart Cookie Baking Machine.

## Teams

As with every massive undertaking, you will be split up in two groups: team Brain and team Brawn.

Team Brawn, a.k.a. the Cookie Taster Team, has the job to:
- select a cookie recipe that needs evaluation, follow the recipe and produce the cookies from the recipe
- take a picture of what the resulting cookies look like
- gather a focus group and have them taste the cookie, then provide a picture of the group's thumbs up/thumbs down evaluation

Team Brain, a.k.a. the Cookie Coder Team, has the job to:
- create a new cookie recipe in a programming language of your choice, and give the cookie a name
- bake the cookies from your recipe
- create a video with step-by-step instructions on how to make your cookies, and provide a link to it.
- take a picture of what the resulting cookies look like
- gather a focus group and have them taste the cookie, then provide a picture of the group's thumbs up/thumbs down evaluation

We leave it up to you to choose which team you want to belong to.

## Practicalities

When you have finished your task, you need to communicate your deliverables to us.
Start by cloning this repository, because you will need to make a pull request later.

For team Brain:
- create a new directory that identifies you. For instance, Santa created the directory *team_Santa*.
- inside this directory, copy the README.md file from the template in the *_template/* directory.
- edit your copy of README.md and fill in: the name of your cookie, your team name, link to your video and the cookie recipe code.
- copy your *cookies.jpg* and *evaluation.jpg* as well (max resolution 640x480)

For team Brawn:
- copy your picture into to directory of the recipe you chose to evaluate, include your name so that the files are unique, following the template: *cookies_&lt;teamname&gt;.jpg* and *evaluation_&lt;teamname&gt;.jpg* (max resolution 640x480)


For both teams:
- generate a public/private key pair that will later be used to send your reward to you. *KEEP THESE FILES SOMEWHERE*

```
openssl genrsa -out private.pem 2048
openssl rsa -in private.pem -outform PEM -pubout -out public.pem
```

- Create a pull request and mention your team name in the comment, and also paste your PUBLIC KEY there.
- now wait until we have a chance to merge your pull request.


## Rewards

We will start sending out rewards (flags) on 17 December 2019.

Since team Brain does more work than team Brawn, the rewards will be higher.
You reward will be sent to you, encrypted with your public key.
To decrypt the encrypted message *reward.b64*, execute:
```
base64 -d <reward.b64 >reward.bin
openssl rsautl -decrypt -inkey private.pem -in reward.bin -out reward.txt
```

