ACT 1
=================================

*TH walks in; DC either hard at work or playing Tetris*
TH: Hi, Are you Derek?
DC: Yes, Can I help you?
TH: Yea, I'm your new boss. My uncle John just hired me.
DC: John the owner?
TH: Yep, my uncle, he hired me today.
DC: Nice to meet you, boss.
TH: So let's get to work; Uncle John said that we need to set up three new servers: database, web and app.
DC: Sounds like a lot of work; we'd better get started!
TH: *You'd* Better get started. I'm going to go check out how well my new office chair swivels.

*TH leaves; DC goes into explanation on what needs to be done*

** start each server manually, start installing software, etc** 

TH: You done? What's taking so long?
DC: This is grunt work... It takes so long to do each system by hand.
TH: Actually, I was just reading in Information Week about something called Puppet. Not sure exactly what it is but let's use it.
DC: OK... I guess I can give it a shot
TH: You can find me in my office... Just knock first...

*TH leaves and DC pulls up some scary documentation*

ACT 2
=================================
DC: This is madness; I want to manage my systems, not manage puppet!
DC: *Technical stuff on why puppet blows chunks*
*TH walks in*
TH: Sounds like things are going great!
DC: Not really, I appreciate the layer of abstraction that Puppet gives me but now instead of managing my systems I'm too busy managing Puppet! Surely there's a better way!!

*Angelic music plays as "Ansible" shows up on the projector*
DC: Wow, I seem to have forgotten everything about Puppet already (*TODO* feel free to replace this line with something actually witty)

*DC sets up ansible*

ACT 3
=================================

TH: This is great! I might just get a raise because of how well this project is progressing.
DC: Yep, the tagline is "Automation even a manager can understand"
TH: There just seems to be one thing missing; I can't quite place my finger on it...
DC: I Know!
*DC runs ansible ansibleservers -m yum -a 'name=cowsay state=latest' *
TH: Awwww yea!

==FIN==
