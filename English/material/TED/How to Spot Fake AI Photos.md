https://www.youtube.com/watch?v=q5_PrTvNypY 

You are a senior military officer and you've just received a chilling message on social media.

Four of your soldiers have been taken, and if demands are not met in the next ten minutes, they will be executed.

All you have to go on is this grainy photo, and you don't have the time to figure out if four of your soldiers are, in fact, missing.

What's your first move?

If I may be so bold, your first move is to contact somebody like me and my team.

I am by training an applied mathematician and computer scientist.

And I know that seems like a very strange first call at a moment like this, but I have spent the last 30 years developing technologies to analyze and authenticate digital images and digital videos.

Along the way, we've worked with journalists, with courts and with governments on a range of cases from a damning photo of a cheating spouse, gut-wrenching images of child abuse, photographic evidence in a capital murder case, and of course, things that we just can't talk about.

It used to be a case would come across my desk once a month.

And then it was once a week.

Now, it's almost every day.

And the reason for this escalation is a combination of things.

One, generative AI.

We now have the ability to create images that are almost indistinguishable from reality.

Two, social media dominates the world and is largely unregulated and actively promotes and amplifies lies and conspiracies over the truth.

And collectively, this means that it is becoming harder and harder to believe anything that we read, see or hear online.

I contend that we are in a global war for truth with profound consequences for individuals, for institutions, for societies, and for democracies.

And I'd like to spend a little time talking today about what my team and I are doing to try to return some of that trust to our online world and in turn, our offline world.

For 200 years, it seemed reasonable to trust photographs.

But even in the mid 1800s, it turns out the Victorians had a sense of humor.

They manipulated images.

Or you could alter history.

If you fell out of favor with Stalin, for example, you may be airbrushed out of the history books.

But then, in the turn of the millennium, with the rise of digital cameras and photo-editing software, it became easier and easier to manipulate reality.

And now, with generative AI, anybody can create any image of anything, anywhere, at a touch of a button.

From four soldiers tied up in a basement to a giraffe, trying on a turtleneck sweater.

(Laughter) It's not fun and games, of course, because generative AI is being used to supercharge past threats and create entirely new ones.

The creation of nudes of real women and children used to humiliate or extort them.

Fake videos of doctors promoting bogus cures for serious illnesses.

A Fortune 500 company losing tens of millions of dollars because an AI impersonator of their CEO infiltrated a video call.

Those threats are real, they are here, and we are all vulnerable.

Before we talk about how we would analyze this image to determine if it's real or not, it's useful to understand how generative AI works.

Starting with billions of images with a descriptive caption like this, each image is degraded until nothing but visual noise is left.

A random array of pixels.

And then the AI model learns how to reverse that process by essentially turning that noise back into the original image.

And when this process is done, not once, not twice, but billions of times on a diverse set of images, the machine has learned how to convert noise into an image that is semantically consistent with anything you type.

And it's incredible.

But it is decidedly not how a natural photograph is taken, which is the result of converting light that strikes an electronic sensor into a digital representation.

And so one of the first things we like to look at is whether the residual noise in an image looks more like a natural image or an AI-generated image.

Here, for example, is our real dog and our AI dog.

And here is the residual noise that I've extracted.

And if you look at this, it's not at all obvious that there's any difference between those two patterns.

But here, in this visualization of the noise, you can see a decidedly different pattern between the natural and the artificial.

Those star-like patterns are a telltale sign of generative AI.

Now, for the mathematicians and the physicists in the audience, that is the magnitude of the Fourier transform of the noise residual.

For everybody else, that detail doesn't matter, but you definitely should have taken more math in college.

(Laughter) Professors can't help themselves.

So let's apply this analysis to this image.

Here's the noise residual that I've extracted.

And there is that star-like pattern that you see in the bottom right.

Our first suggestion that something may be wrong here.

But no forensic technique is perfect.

And so you don't stop after one thing, you keep going.

So let's go on to our next one, the vanishing points.

If you image parallel lines in the physical world, they will converge to a single point, what's called the vanishing point.

A good intuition for that, the railroad tracks.

When I took this photo, the railroad tracks are obviously parallel, but you can see that they narrow as they recede away from me and intersect at a single vanishing point.

This is a phenomenon that artists have known for centuries.

But here's the great thing.

AI doesn't know this.

Because AI is fundamentally, as I just described, a statistical process.

It doesn't understand the physical world, the geometry and the physics.

So if we can find physical and geometric anomalies, we can find evidence of manipulation or generation.

Here in this image, I've annotated four parallel lines on the parallel sides of the wall in our basement photo, and you can see a lack of a coherent vanishing point.

That suggests a physically implausible scene.

Evidence number two.

Alright, what else can we learn?

Surprisingly, shadows have a lot in common with vanishing points.

Here, what I've done is I've annotated a point on a shadow with the corresponding part on the bottom of the rail that is casting that shadow.

And I've extended those lines outwards.

And they intersect, not at a vanishing point, but at the light that is casting that shadow.

And again, this is a physical phenomena that you expect in natural images.

And because AI fundamentally doesn't model the physics and the geometry of the world, it tends to violate these physics.

Let's apply this analysis to our image.

Here I've annotated four shadows on the bottom from the soldiers' shadows to their legs.

And you can see that the lines aren't even close to intersecting.

Not one, not two, but three anomalies.

We now have a very good indication that this image is not authentic.

The most important thing I want you to take away from this is that while it may not be easy, it is possible to distinguish what is real from what is fake.

I think this image is a bit of a metaphor for how a lot of us feel.

We feel like hostages.

We don't know what to trust anymore.

We don't know what is real.

What is fake.

But we don't have to be hostages.

We don't have to succumb to the worst human instincts that pollute our online communities.

We have agency, and we can effect change.

Now, I can't turn you all into digital forensics experts in ten minutes.

But I can leave you with a few thoughts.

One, take comfort in knowing that the tools that I've described and that my team and I are developing are being made available to journalists, to institutions, to the courts to help them tell what's real and fake, which in turn helps you.

Two, there is an international standard for so-called content credentials that can authenticate content at the point of creation.

As these credentials start to roll out, they will help you, the consumer, figure out what is real and what is fake online.

And while they won't solve all of our problems, they will absolutely be part of a larger solution.

Three, please understand that social media is not a place to get news and information.

(Applause) It is a place that Silicon Valley created to steal your time, your attention, by delivering you the equivalent of junk food.

And like -- thank you.

(Applause) And like any bad habit, you should quit.

(Laughter) And if you can't quit, at least do not let this be your primary source of information, because it is simply too riddled with lies and conspiracies and now AI slop, to be even close to being reliable.

Four.

Understand that when you share false or misleading information, intentionally or not, you're all part of the problem.

Don't be part of the problem.

There are serious, smart, hard-working journalists and fact-checkers out there who work every day, because I talk to them every day, to sort out the lies from the truths.

Take a breath before you share information, and don't deceive your friends and your families and your colleagues, and further pollute the online information ecosystem.

(Applause) We're at a fork in the road.

One path, we can keep doing what we've been doing for 20 years, allowing technology to rip us apart as a society, sowing distrust, hate, intolerance.

Or we can change paths.

We can find a new way to leverage the power of technology to work for us and with us, and not against us.

That choice is entirely ours.

Thank you.

(Applause) Latif Nasser: We're doing rapid-fire questions, you ready?

Roughly what percent of images online do you believe to be fake?

Hany Farid: Depends on the platform.

Signal-to-noise ratio is getting close to one.

Stay off of Twitter, of X, and stay off of everything else for that matter.

LN: So what do you think?

HF: I would say we're getting close to 50 percent.

LN: Can you differentiate between things that have, like, Instagram or TikTok filters or Photoshop versus fully AI generated images?

HF: Yes, but it's becoming increasingly more difficult.

LN: Are there any websites a layperson can use to check?

HF: No.

By the way, this is a secondary problem, which is now people are creating fake things, then going to fake sites to authenticate them.

And it's all getting very weird, don't do it.

LN: Last one, most important one.

In CSI crime shows, when they say enhance, can you do that?

(Laughter) HF: Yes.

LN: OK, great.

Hany Farid, everybody.

- chilling
- executed
- grainy photo
- bold
- applied mathematician
- authenticate
- damning
- spouse
- gut-wrenching
- photographic
- a capital murder case
- escalation
- escalation <=> escape
- amplifies
- conspiracies
- actively promotes
- and collectively
- contend
- profound
- profound consequences
- institutions
- democracies
- offline
- Victorians
- manipulated
- Stalin
- airbrushed out
- airbrushed
- millennium
- manipulate
- tied up
- basement
- giraffe
- turtleneck
- supercharge
- nudes
- humiliate
- extort
- bogus
- illnesses
- Fortune
- impersonator
- infiltrated
- vulnerable
- descriptive caption
- degraded
- noise
- array
- reverse that process
- diverse
- semantically
- consistent
- incredible <=> unbelievable
- decidedly
- sensor
- residual
- extracted
- visualization
- decidedly different pattern
- telltale
- audience
- magnitude
- Fourier transform
- definitely
- forensic
- vanishing
- parallel
- converge
- railroad tracks
- narrow
- recede
- intersect
- statistical
- geometry
- physics
- geometric
- physical
- anomalies
- manipulation
- annotated
- implausible
- shadows
- corresponding
- authentic
- metaphor
- hostages
- succumb
- instincts
- human instincts
- We have agency
- forensics experts
- credentials
- authenticate
- roll out
- Silicon Valley
- the equivalent of junk food
- riddled
- lies and conspiracies
- slop
- a fork in the road
- rip us apart
- sowing distrust
- sowing <=> swallow
- intolerance
- leverage
- Roughly
- Signal-to-noise ratio
- differentiate
- distinguish
- filters
- versus
- layperson
- enhance
- 