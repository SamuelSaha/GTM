# Modern Technical Writing: An Introduction to Software Documentation

**Author:** Andrew Etter  
**Format:** PDF  
**Category:** operations

---

## Page 1

Modern
Technical
Writing
< An Introduction to
Software Documentation >
Andrew Etter

---

## Page 2

Modern Technical Writing

---

## Page 3

Modern Technical Writing
1.Introduction
2.Basics
1.Don'tWrite
2.DefinetheAudience
3.BasicFunctionalDocumentation
4.Style
5.CatalogtheDiff
6.Builda Website
7.HelpOthers Write
8. PublishFrequently
3.Specifics
1.UseLightweightMarkup
2.UseDistributed VersionControl
3. Don'tDuplicate
4.Make Static Websi
5.Rsyne
6. Metrics
7.ScriptYourComplexity Away

---

## Page 4

8.TheLegalProblem
9. Localization
10.ContrivedWorkflow
11.What AboutWikis
4.TheGrandFinale
5. Acknowledgments
6.Legal

---

## Page 5

Introduction
Given the pace of the software industry,I'llprobably regret
callingthisbook Modern TechnicalWriting,but Technical
Writing in 2019 or What CurrentlyPassesas Sane Technical
Writing weren't any better. Books like this one have a
short shelflifeunless a subjectmatter expert meticulously
maintains them, which Idon't intend to do. Still,limagine
the book will hold itsvalue for the next fiveyears—
probably long enough to make writing and reading it
worthwhile.
I had the idea for this book a couple years after I
startedworking as a technicalwriter.I had justfinished
interviewing some very nice, very experienced people
from two massive SiliconValley companies, and we just
could not find common ground. Their impression of
the job was that technical writers interviewed engineers,
took copious notes, wrote drafts in Adobe FrameMaker,
and waited several hours for some arcane process to

---

## Page 6

build those draftsinto printablebooks. These candidates
mentioned page counts,XSLT, Perforce,and gerunds. They
were proud that theirpage numbers were laidout recto-
verso. None of them seemed to give any thought to
their readers'actual needs, preferringtheir own criteria
for what constituted a job well done. They used phrases
like “clear,concise, correct, and complete" and avoided
words like"searchable,""scannable," "attractive,"and most
egregiously,"useful."
These candidates weren't stupid;they were articulateand
pleasant,well-educated and inquisitive.No, Ibelievethey
were products of a dysfunctional profession,a profession
of misplaced priorities,judged fortoo long on meaningless
criteriaby managers who treatthe ChicagoManual ofStyle
likea holy text and would rather produce minimal value
from a lot of work than tremendous value from far less
work. Exceptional technicalwriters are force multipliers
within the software industry.Great documentation makes
new hires productive in days instead of weeks, prevents
thousands of callsto customer support, is the difference
between cripplingdowntime and rock solidstability,and

---

## Page 7

inspires true, fervent love of development platforms.
Technical writing matters,so 1 wrote this book to help
people createdocumentation in a sensibleway.
To be crystal clear, this book is about technical
writing in the software industry. Most of the principles
are universally applicable, though. If a particular
recommendation doesn't seem relevant to your work,
please take a mental step back and try to assessthe high-
levelprinciplesbehind the recommendation. Maybe I'm
completely off base, or maybe some kernel of wisdom is
buried in my insufferableprose. In other words, please
don'tdismiss a good ideabecause of bad execution.
And thanks forreading.
— Andrew Etter
1.Recto-verso just means using slightly different
layoutsforthe "right"and "left"pages of a book.

---

## Page 8

Basics
Like allwriters, technical writers aim to produce content
that theirintended audiences willread and find useful.+
This has to be the goal,because any other goal isabsurd.
Keeping itin your head at alltimes willhelp you produce
more valuable work in any profession.Consider a few
common misconceptions about technicalwriters:
+Technical writersproduce formal documentation.
In thiscase,"formal"means unnecessarily stuffyand
repetitive,the sort of writing that causes people to
skim ratherthan read.When your idealreadersare tee
shirt-cladsoftware developers who mainline Hiball
Energy and spend most of the year looking forward to
Burning Man, it'ssafeto assume a more casualwriting
style.
Note

---

## Page 9

This does not give you license to write in
an unprofessional or sloppy manner. Writing
should not callattentionto itselfby being too
formal or too casual.Occasionally reminding
readers that human beings produced their
documentation is fine.Making readers think
thatthey are reading rough draftsisnot.
+Technical writers produce comprehensive
documentation.
Writing should be the minimum possible length.
Oddly, most students learn this guideline in grade
school and have forgotten it by grad school. If a
help system must be truly comprehensive, itshould
be because readers will accept nothing less,which
is untrue 99% of the time. Huge blocks of writing
look intimidating,and excessivecontent waters down
useful content. Identifywhat the audience actually
needs to know, and includeonly that.
+Technical writers help protect companies from
lawsuits.

---

## Page 10

No, lawyers do that, and believe me when I say that
they're perfectlycomfortable composing their own
indecipherabletext.Technicalwriters,at the absolute
most, should collatelegaleseinto theirwebsites.You
should take content verbatim from actual attorneys
and spend no more time on itthan ittakesto pressCtrl
+ C and Ctrl+ V. Then show them how to update the
content themselves so that you can get back to your
realjob.
+Technicalwritersproduce printdocumentation.
Any piece of print documentation should be an
absolute minimalist Getting Started guide (complete
with requisite legal boilerplate)that directs its
recipients to a web page. People are comfortable
typing www intoa web browser ifthey need help.
Unfortunately, producing content that people will read
and find useful is,like,reallyhard. Here are the basics.

---

## Page 11

Don't Write
Don't write often, anyway. Technical writers,firstand
foremost, are testers and researchers. Your job is to know
what people want to achieve and preciselyhow to achieve
it.Communicating that knowledge isthe laststep of the
process and reallyshouldn't comprise more than 10%
of your time. When people say,"I was writing allday,"
they don'tmean they were intermittentlytyping foreight
straight hours. They mean they spent the entire day
engaged in the writing process.And a big part of that
process isinstalling,configuring,and testingsoftware.In
other words, learning.
Remember, thejob of a technicalwriterisnot to findbugs.
Sure,you willfindbugs, and ifyou'renot aware of any,you
probably don't know the product very well.You should
alsoreport these bugs to developers.But the main point
of a technicalwriter performing testingisnot to improve
product quality,but to increasepersonal knowledge. Your
testing should be centered around making you smarter.

---

## Page 12

Once you have a complete grasp of how something
works, you can stop.Unlike a tester,you don't have to
go any further.You don't have to reproduce trickyissues
or check for unforeseen regressionsin functionality.This
difference makes your testing less tedious and more
selfishthan thatof a formal qualityassurance process,but
because the ultimategoal isto teach othersthe material,
you can pretendto be an altruist.
Be sure to leverage all the wonderful writing that
developers and testers produce, even if it's half-
complete, riddled with typos, and on a wiki page
entitled"integratingwith shamrock =D."Check the source
repository for any filesnamed README .md, and run any
scriptswith the help argument. Google any underlying
open source software,Check Wikipedia for unfamiliar
terms. Take notes, The learning process is time-
consuming, so don't be discouraged ifyour measurable
output is essentiallynil for days or even weeks after
moving onto a new project.
Contrary to popular belief,there are allkinds of stupid
questions, or at leastignorant ones. The goal of allthis

---

## Page 13

testing and research is to be mentally equipped to ask
pointed, intelligentquestions to business development,
product development, quality assurance, customer
support, and ideally,actual users. For business reasons,
thislastgroup might not be accessible,but tryyour bestto
getin touch with some ofthem.
Talking to people isan art.A testermight want to gripe
about a useless or buggy feature,whereas a developer
might anxiously justifyarchitecturaldecisions.A product
manager probably wants to discuss long-term vision and
willbe upset ifyou didn'tschedule a meeting, whereas a
salespersonmight be perfectlyhappy to chat about user
frustrationsfrom adjacentbathroom stalls.A good ruleof
thumb isto treateveryone as busy individualswhose time
isvaluable,but anotherruleofthumb istobreakthisrule
and be more ofa jerkifan essentialemployee isn'tgiving
you the information you need to do your job.Tailoryour
approach to the person,come prepared to meetings, batch
your questions into related sets rather than bothering
people every twenty minutes with individualquestions,
and thank everyone for theirtime. Your contribution to

---

## Page 14

a projectisn'timmediately obvious, so try not to be put
out ifpeople aren'tas forthcoming as you'd like.Technical
writersneed to be grinders,willingto slowly but surely
chip away at the block of ignorance until a beautiful
sculptureemerges—or something likethat,anyway.
After all that testing and research,you have to verify
everything that people told you through additional
testing.Tedious, but essential.At this point, though,
you'rewell on the way to definingyour audience,
Define the Audience
Writers have to make assumptions in order to achieve
anything useful.Bare minimum, we assume that people
can read. Similarly,you should assume that your readers
know how to use a trackpad and won't freezeup when the
Enter key reads Return. Assuming anything lessleads to
writing likethis:
Place your hand on the mouse and, moving your
hand (and arm, as necessary), direct the white

---

## Page 15

cursor on your monitor. Ifyour monitor is not on,
you can turn it on by pressing and releasing the
power button.The power button iconcan be found
in Appendix D: Icons. If your mouse has multiple
buttons, press and releasethe leftmost one. Ifyour
mouse has one or fewer buttons, press and release
either the only button, or the leftsection of the
mouse, respectively.Ifyou are using a trackpad...
Acolleague once argued to me thatyou sometimes have to
targetyour writing to just such an audience. The proper
response to such an assertionisto letyour eyes bulge out
of theirsocketsand shake your head from sideto side,but
ifyou must reply,the simple counter-argument isthis:you
cannot help people who requirethatlevelof hand-holding.
They probably won't read the documentation, and even
if they do, they definitelywon't understand it.There's
nothing you can do forthem. Betterto say:
The Settings menu letsyou adjustmouse sensitivity
and button mappings.

---

## Page 16

This statement involves a lot of assumptions. We're
assuming the reader can find the menu, knows what
mouse sensitivityis,and can infer that some button
behaviors are customizable. We're also assuming the
reader knows the basicsof manipulating a computer and
has the applicationopen. I'm happy to make allof these
assumptions, regardlessof audience.Ifan applicationhas
alot ofbutton groups and only a few arecustomizable,you
might need to be more specific,but the levelof detailis
basicallyfine.Don't get stuck in the quagmire of trying to
help the helpless.Iknow itsounds cold and mean-spirited,
because these are the readers most in need of assistance,
but by cateringto them, you are doing areal disserviceto
the other 90% ofthe population.
Now that we've defined who is not the audience,we
can roughly divide readers into three groups: users,
administrators,and developers.
Users are people who just want to achieve something
with an application,whether it'sresizing an image,
creating a spreadsheet, or sending an email. Users are
typicallyconcerned with inputs and outputs. They type

---

## Page 17

a few things, drag a couple boxes around, and voila, a
monstrosity of a PowerPoint presentationisborn.
Note
A user interfaceisnot a requirement for someone
to be a user. Command line applications have
users,too,people who justwant to copy and paste
some common commands and move on with their
livesrather than mastering the syntax, chaining
commands, and incorporatingregularexpressions.
Administratorsinstalland configureapplications.I'm not
justtalkingabout server administratorsor people with
administrator permissions on a computer, but anyone
whose concerns are setup and maintenance. How much
disk space does the application server fillover time?
Where are the logslocated?How do you recover data in
the event of a crash?What's the simplestway to perform
backups? How do you troubleshoot poor performance?
In consumer applications,the user is often also the
administrator.In business applications,this situationis
lesscommon.

---

## Page 18

Developers extend applicationsor interfaceswith code.
They want to improve some aspect of an existing
applicationor build something new. More than anything,
they need reference materials, short tutorials,and code
samples. Conceptual introductions to a language or
framework are wonderful, and ifyou have the time and
expertise,by allmeans, write them. But programmers
check online language and libraryreferenceshundreds
and hundreds of times. They only read Programming
Python once. Ifyou have to prioritize,go with the former,
Most modern designers fallinto the developer group, as
well.
Knowing which group an audience fallsinto gives you a
reasonable startingpoint,but you stillneed to home in
on actualuse casesin orderto focusthe documentation.
A singleinaccurateassumption about your audience can
lead to a mountain of discarded work. Take the time to
trulyunderstand what your audience wants to accomplish
through conversations,meetings, interviews,analytics—
anything atyour disposal.

---

## Page 19

Basic Functional Documentation
Now thatwe have knowledge and an audience,it'sfinally
time to write. Basic functional documentation (BFD) is
exactlywhat itsounds like:a big...finedeal.Ata minimum,
product documentation should answer the following
questions:
+What isthisproduct? Why would anyone want it?
These two questions are incredibly challenging for
the average technicalwriter,a group of people much
more focused on how than what or why. I'vestruggled
with them many times. But if you can't answer
these questions,you need to go back to the research
phase, because you don't understand your audience
at all.The answer to this question shouldn't come
from a marketing department. Instead,itshould be
an honest, buzzword-free appraisalof capabilitiesand
use cases.

---

## Page 20

+How does thisproduct fitintoa broader ecosystem, if
at all?Does ithave any dependencies?
The answer to thisquestion can bea singlesentence,
an architecture diagram, or a complex discussion
of the various components necessary to create a
coherentproduct stack.Web frameworks are perfect
examples, because it'sso rareto use one in isolation.
They're typicallypaired with severalcomplementary
products,and developers need to know which ones
priorto installing.
-Where can Iacquirethisproduct?Iftherearemultiple
distributionpackages,which should I choose and
why?
One of the nastiest things you can do to readers
is convince them that your product is useful and
desirableand then directthem to a download page
with fourteen different filesand no guidance on
which are appropriate for which users.Some people

---

## Page 21

can distinguish between .zip and .tar.gz, but
many cannot.
-How do I installthe product? What are the basic
configurationoptions,ifany?
For consumer applications,the installprocess should
be so streamlinedthat thissectionbarelyneeds to
exist.For server applications,it'soften the longest,
most criticalpart of the documentation.
+What does a simple,startto finishoperation look like?
This section can be anything from a pictorial
walkthrough to a functionalcode sample—to be clear,
not just a couple snippets—but whatever it is,it
should take the user from nothingto something.It
should be meaty enough to convince readers that
they'velearned something.
And that'sit.The good news is that the principles of
BFD are as applicable to vacuum cleaners as they are
to databases. I created the following example for the

---

## Page 22

overpriced glass cone that I use to make my morning
coffee:
Manual drippersgiveyou totalcontrolover how you
brew your coffee.You can customize the temperature
of the water,the rateatwhich you add water,and the
sheer amount of water to arriveat your definition
of a perfectcup. Ifyou aren'tpicky and justwant a
cup of decent coffeein the morning, a conventional
machine is a better option. This method does not
produce espresso.
Because of their unique shapes, drippers often
requirespecializedfilters,You alsoneed a gooseneck
kettle in order to more precisely control the
flow of water. Some electrickettleshave built-in
thermometers. Ifyours does not,use an instant-read
thermometer. A digitalscaleletsyou measure the
amount of coffeeand water you use in the brewing
process, which helps with day-to-day consistency.
Finally,you need a burr grinder to reduce your whole
beans to a nice,uniform grind.The totalcost of this
setuprangesfrom $150 -500.

---

## Page 23

You can buy allof these products from Amazon. A
manual burr grinder will save you a lot of money
compared to an electricmodel, at the cost of your
time and muscles. Avoid cheap blade grinders,as
their inexact grinds ruin good coffee.Most other
components are of comparable priceand quality.
Once you have everything, adjust your grinder's
settingsuntil you arrive at a grind that is coarser
than espresso,but much finer than French press,
Vary this settingover time untilyou arriveat your
favoritegrind,and then make note of it.You can do
the same thing with your water temperature. 200 °F
isa good startingpoint.
To brew a cup ofcoffee...2
In very littlespace, | answered each BFD question. BFD
givesyou a baselinelevelof content for which to strive,
but it also has the happy side effect of keeping you
focused.Because the above example documentation isfor
a glasscone, I only provided the levelof detailrequired
to "operate"that cone. I didn'tdelve intohow to adjusta

---

## Page 24

burr grinder or electrickettle,justthat you should arrive
at semi-fine coffeegrounds and 200 °F water. Links to
grinder and kettledocumentation (ifany exist)would be
greatadditions.
Tip
Whenever possible,don't write from memory.
Verify content as you write it. If the
documentation involves shell commands or code
snippets,copy and paste them aftervalidating that
they work.
Style
I hate the overbearing nature and rigidity of
comprehensive styleguides,but I'dbe remiss ifIdidn'tat
leastmention style,Don't worry, I'llkeep itquick:
+Consistency isking. You sound unreliableifyou use
“Postgres”at the beginning of a sentence,"postgres"in
the middle of a sentence, and "PostgreSQL" in one or

---

## Page 25

two random locations.Abbreviations are fine,but use
them consistently,ideallyafterintroducingthem:
PostgreSQL (Postgres)is a popular open-source
database.
Likewise, if you call something a dialog in one
document, don'tcallita pop-up in another.
-Bias towards including headers, tables,lists,diagrams,
and images. These additionsmake your writing more
approachable and simpler to scan than paragraph
after paragraph of prose. For example, almost all
descriptionsof how to do something should include
an ordered list.In my coffee example, would an
unordered list(or a table) have improved the second
paragraph?
+Use inlinestylesto offsetimportant text.Typically,
technicalwritersuse bold for user interfaceelements
("Click Save."); italicsfor emphasis ("You must save
your work before shutting down."); and monospace

---

## Page 26

for filepaths, terminal commands, and code ("Run ./
bin/script.sh.").
-For the sake of clarity,try not to verbify obscure
nouns, An extreme example: "Grep it."vs,“Use grep to
search the file."
+Copy edit,but don'tobsess over it.A straycomma or
dangling prepositionisn'tthe end of your credibility.
You can probably finda typo in thisbook. More than
one,actually,
Catalog the Diff
One of the most important functions of a technical
writer is to record changes to a product. Good change
logsconvince people to upgrade,inspireconfidencein the
directionof a product, and help developers takeadvantage
of new features,What's new? What's different?What was
removed? How do I upgrade? Any "gotchas"to be aware
of? Ifa featureissimple,justnoting that itexistsisoften
betterthan adding new documentation on how to use it;

---

## Page 27

people can figureout how to use simple featureswithout
the help of documentation, but not if they don't know
to look forthem. More than anything else,change logs
should be terse,minimalist, and eminently scannable.
Marketing departments often use these documents to
write theirown, hyped-up copy foradvertisements or blog
posts,but your own appraisalof differencesshould use a
more neutral tone, In six months, the features described
in the change log willno longer be so novel,but they will
stillbe online. Readers shouldn't have to parse a corny
salespitch about the incrediblepotentialof a new feature
in order to learnthat push notificationsarrivedin version
1.8.2,
Build a Website
I mentioned earlierthat you should build and host a
website, not distributePDFs, but itbears repeating.Even
the best documentation, like software, eventually goes
out of date. PDFs get downloaded onto hard drives and
then sitthere likeday-old bagels,growing more and more

---

## Page 28

staleuntilthey'reactivelyharmful. You can never update
them. Even ifsomeone downloads updated versions,every
modern web browser savesthe new filesas Admin_Guide
(1) .pdf rather than overwriting the old files.The whole
situationgives me the chills.Hosting your content on a
website gives you the power to fix inaccuraciesalmost
instantlyand keep your content in sync with the latest
software release.
Shipping an HTML help system with the software itself
isbarelybetterthan PDFs,OK, the documentation doesn't
go out of date, because it ships alongside itsassociated
software,but you're stillunable to fixpotentiallycritical
issuesuntilthe next software version ships.And that'sif
you can convince people to upgrade. Ifyou must ship a
help system, a minimalist user guide typicallysuffices.4
Ifyou're contractuallyobligatedto provide more...well,I
recommend followingthe letterof the law,not the spirit.
Help Others Write
However you decide to write and distribute your

---

## Page 29

documentation, you should do itin a way that encourages
others to contribute. The realityof the profession is
that even a largeteam of writerscannot possiblyknow
everything worth knowing about an application,and
most companies do not have a large technical writing
team. The open-source softwaremovement, mod scene in
PC games, and birthofa millionobscurewikis have proven
that people willhappily share theirexpertiseand passion
ifan easy,hospitableway of doing so exists.Strangerswill
do it for free,and coworkers will do it even if it isn'tin
theirjob descriptions.I'vehad colleaguesargue thispoint
with me, but no, people reallywillcontributeifyou justlet
them,
Evenif you only have 500 unique visitorsto your site,a 1%
contribution rate works out to fiveextra people helping
with the documentation. I'lltake that help. You likely
have more readers and a higher contribution rate,so don't
dismiss this idea as something that only applies to larger
projects.Itappliesto allprojects.
Ultimately,the job of a technicalwriter is to ensure the
qualityof the documentation. Hopefully you createa lot

---

## Page 30

of ityourself2,but whether you write itor not islargely
irrelevantto the end product. Quality is relevant.With
qualityas the objective,the contributionsystem should
not be so open that people can just insert half-baked
additions.A review process must exist.
Admittedly, the easiestway to help strangerscontributeis
to justcreatea wiki and be done with it.Wikis have some
realappeal,but I don't believethey'rethe best option in
most cases.We'lldiscusswhy later.
Publish Frequently
Publishing should not be a specialevent. It should not
be challenging.Itshouldn'trequireanything more than
a quick sanity check and a glance at the build log.
Something about your process isbroken ifyou need more
than a minute to verifythat content isready to post to a
production website.
Many ways of catching problems exist.For large,complex
help systems, you can use a continuous integration system

---

## Page 31

to run a seriesof build testsafterevery commit or merge.
This method islikelyoverkillformost help systems, where
the testing should occur manually during the review
process.Reviewing contributionsto the documentation is
more complex than justasking,"Isthiscontent accurate?
Isthe writing well-organized?”Italsomeans buildingthe
finishedproduct and ensuring that the change has not
introduced any new errorsor warnings.
Even simple automation is effective,likea Cron job that
checks out and builds the documentation every hour,
writes the build log,and posts the resultant content to
an internal staging server.Unlike software development,
the process doesn't need to be especially elegant or
sophisticated,justsimple and functional.
1.Regarding creative writing: entertaining people is
useful, too...
2.Not always the best assumption if your writing
appears online.

---

## Page 32

3.I'm not actuallygoing to cover the process,because for
a morning ritual,it'sembarrassingly complicated.«—
4.One that isn'tdetailedenough to contain any critical
bugs.«-
5.Your jobisinjeopardyifyou don't...”

---

## Page 33

Specifics
Now that we've discussed the basic things technical
writers should do, we can delve into the nitty-grittyof
how to do them.
Use Lightweight Markup
Someone once said,"XML islikeviolence:if itdoesn't solve
your problem, you aren’tusing enough of it."But whoever
saidthiswas definitelya) a developerand b) not writing
XML by hand.
Because writing XML by hand iscrazy,in the same way
thatwriting any significantweb applicationin JavaScript
iscrazy.Application developers should write TypeScript,
Dart, CoffeeScript,or practicallyanything elseand then
compile to JavaScript.Likewise, ifXML is a part of your
publishing pipeline,you should write lightweightmarkup
and then build to XML. The entirepoint of lightweight

---

## Page 34

markup isto make iteasierto produce well-formed XML,
and we need XML in order to buildwebsites.
Why is lightweight markup so superior? Consider the
followingAsciiDoc:
= My Title
This introductory paragraph contains a
link to
https: //www.google.com[Google].
[source, ruby]
puts "Here is some code."
== My Section
* List item
* Another list item
Here is the corresponding DocBook, an XML-based
markup language:

---

## Page 35

<?xml version="1.0" encoding="UTF-8"?>
<!DOCTYPE article PUBLIC "“-//OASIS//DTD
DocBook XML V4.5//EN"
"http://www. oasis-open. org/docbook/
xm1/4.5/docbookx.dtd">
<?asciidoc-toc?>
<?asciidoc-numbered?>
<article lang="en">
<articleinfo>
<title>My Title</title>
</articleinfo>
<simpara>This introductory paragraph
contains a link to
<ulink url="https://www.google.com">
Google</ulink>.</simpara>
<programlisting language="ruby"
linenumbering="unnumbered">
puts "Here is some code.”
</programlisting>
<section id="_my_section">
<title>My Section</title>
<itemizedlist>

---

## Page 36

<listitem>
<simpara>
List item
</simpara>
</listitem>
<listitem>
<simpara>
Another list item
</simpara>
</listitem>
</itemizedlist>
</section>
</article>
The AsciiDoc content is human-readable in raw form,
straightforwardto learn,and weighs in at 179 characters.
The DocBook content is challenging to parse even with
syntax highlighting,requires specializedknowledge of
odd tags,and contains 723 characters.That's four times
the number of characters for the exact same content.
As we discussed earlier,one of the tenets of modern
technicalwriting isthat everyone isa contributor.Storing

---

## Page 37

content directlyin XML-based languages like XHTML,
DocBook, and DITA dramaticallyreduces people'sabilityto
contribute.
What about specializededitors?MadCap Flareand Adobe
FrameMaker, two popular authoring applications,provide
you with WYSIWYG editorsforthe rapid creationof well-
formed XML. But they cost $1,448 and $9991, respectively,
and are only availableforMicrosoft Windows, Rather than
being mere deterrents (likewriting in XML), specialized
applications actuallyprevent people from contributing.
Amazing text editors are availableon every operating
system, mostly for free,and writers can use whichever
they like.Populareditorsinclude:
-Atom
+Sublime Text
-Notepad++
+TextWrangler
+gedit
-Vim
+Emacs

---

## Page 38

Note
The steeplearningcurve on Vim and Emacs issuch
that I don't recommend them formost people,but
theirpower and flexibilityareundeniable.
MicrosoftWord isa wonderful choiceforcreatingrésumés
and a horriblechoice for creatingdocumentation, Itslone
purpose in this world—one that, again, it reallydoes
perform admirably—is to createshort,attractivePDFs that
can be consumed and discarded, Documentation with any
sortof lifespanneeds to be kept in version control,which
Word's DOCX fileformat (a compressed collection of XML
files)activelyopposes,Documentation should liveonline,
and Word's abysmal HTML export is totallyunsuitable
for creating websites.You have to stylecontent in Word
as you write it,rather than taking advantage of the
naturalseparation of content and style,of HTML and CSS.
Even though most companies provide licensesto their
employees, Word stillcosts money and is only available
forWindows and macOS. For documentation, lightweight
markup isfreeand superiorin every meaningful way.

---

## Page 39

Plenty of lightweight markup languages exist, but
only three are really worth discussing: Markdown,
reStructuredText,and AsciiDoc.
Markdown
Markdown is simultaneously incredible and infuriating,
wonderful and maddening. It'sthe most widely used
lightweight markup language in the world? and has
the cleanest syntax, but it also has a limited set of
featuresand no defined standard.These deficiencieshave
led to a couple dozen "flavors"of Markdown, including
MultiMarkdown, Markdown Extra, GitHub Flavored
Markdown, and a recent standardizationeffortcalled
CommonMark. Each flavor adds features, some of which
areimplemented acrossmultipleflavorswith inconsistent
syntax. The more maddening part, though, is that
almost every Markdown parser(and many exist)processes
whitespace just a littlebit differently.Nested lists,for
example, might have odd spacing in one flavorand not in
another.

---

## Page 40

Using only "vanilla"Markdown syntax allows for broad
compatibility,but you miss out on featuresliketablesand
"fenced"code blocks.Using a flavorof Markdown means
you might have to rework your source filesifyou ever
want to switch to a differentflavor,but the levelof effort
in such a switch would likelybe low. GitHub Flavored
Markdown is a popular and finechoice for simple web-
based help systems. Here'swhat itlookslike:
# My Title
This introductory paragraph contains a
link to
[Google] (https: //www. google.com).
***puby
puts "Here is some code."
## My Section

---

## Page 41

- List item
- Another list item
Markdown's popularity means that many specializedtext
editorsexistforit.The bestare:
+MarkdownPad (Windows)
-iAWriter (macOS)
+ReText(Linux)
reStructuredText
reStructuredText (RST) comes from the Python
community. Unlike Markdown, it has an actual,
standardized implementation. It's also feature-rich,
supporting tables, footnotes, and a wide variety of
directivesfor code and other content blocks. With this
wealth of featurescomes a syntax that has more than
a few rough edges. Whereas you can learn Markdown
in minutes, learning RST takes an hour or two. This
might not seem likea big deal,but when you're trying

---

## Page 42

to empower contributors,the learning curve can be an
unfortunate barrier.This book iswritten in RST.
The main appeal of reStructuredTextisthatitisthe source
language forone of the best documentation generators in
the world: Sphinx. We'll discuss Sphinx later.Here's what
RSTlooks like:
My Title
 
This introductory paragraph contains a
link to “Google
<https://www.google.com>*_.
+. code:: ruby
puts "Here is some code."
My Section

---

## Page 43

- List item
- Another list item
AsciiDoc
AsciiDoc is popular in the Linux community and is the
language with which I have the leastfamiliarity.Quite a
few O'Reillytechnology books arewritteninAsciiDoc.
Summary
AsciiDoc is semantically equivalent to DocBook and is
thus a straightforward,obvious improvement to existing
DocBook toolchains.This equivalencelikelymakes itthe
bestchoiceforcreatingbooks,especiallyones thatrequire
complex formatting.RST isa decent all-purposelanguage,
but itslackof popularitymeans thatitwon't evolveatthe
same pace as Markdown. |am quiteconfidentthatthe next
great documentation sitegenerator will use a flavorof
Markdown as itssource language, so choosing Markdown
gives you a certainmeasure of future-proofing.At time

---

## Page 44

of writing, however, Markdown is missing many useful
featurescompared to AsciiDoc and reStructuredText.
Online editors with live previews exist for Markdown,
restructuredText,and AsciiDoc.These editorsare helpful
for testingout features,learning language syntax, and
deciding which you prefer:
-dillinger.io(Markdown)
+rst.ninjs.org(reStructuredText)
+asciidoclive.com(AsciiDoc)
LaTeX
LaTeX is a powerful markup language with complex
syntax that I purposely didn'tmention untilnow. Ifyou
need it,you already know that you need it.Ifyou don't
need it(and few outsideof academia do),itsonly purpose
isas a stopinyour publishingpipelineon theroad toa PDF.
More on the pipelinelater.

---

## Page 45

Use Distributed Version Control
All sorts of people, most of them much smarter than
me, have extolled the virtues of distributed version
control systems (DVCS) like Git and Mercurial over
centralizedsystems. The basicsare that DVCS have better
performance, allow forofflinework, and are superiorfor
concurrent work on the same file.For technical writers,
the most important reason to use DVCS isthat developers
preferthem.
Because versioncontrolsystems are designed forsoftware
development, each and every one of them isoverkillfor
the typicaldocumentation workflow. For example, you'll
probably never need git reflog. So why worry about
which system you use, when they can all do the job?
Because when you selectPerforce,Subversion, or CVS, you
are basicallyconfessing to potentialcontributorsthat you
can'tbe bothered to use modern tools.

---

## Page 46

Atlassian Bitbucket and Stash are both excellent web-
based interfaces for managing remote repositories.
GitHub and GitHub Enterprise are also great options.
While the defaultuser interface,git-gui,isdecent,Iprefer
Atlassian SourceTree and GitHub Desktop. The terminal
isalways there ifyou need advanced functionality.Many
peopleeven preferitforbasic,everyday operations.
Ifyou have the opportunity to storeyour documentation
in the same repositoryas itscorresponding product source
code,stronglyconsiderdoing so,The approach has some
realappeal:
-Documentation and code branches stayin syne.
+Developers are more likelyto contribute ifthey don't
have to clone a separaterepository,
Of course,thisapproach alsohas some cons:
If a repositoryis large (e.g.2 GB), checking out the
entire repository just to access the 40 KB ./docs
directorycan dramaticallyslow down documentation
builds.

---

## Page 47

+Onerous commit hooks and pull request submission
policies,designed to keep a code base stable,can make
even simple documentation changes a chore.
«If your product is composed of code from many
repositories,a single documentation repository
offerssimpler builds and a more cohesive writing
experience.
Wherever you store your documentation, place a file
named README. md in the root of the repository(or in ./
docs). This Markdown fileshould include:
+A quick summary of the product being documented
Instructions on how to build the documentation
locally
-Instructionson how to contribute
Don't Duplicate
Along with accurate driving directions and videos of
frolickingpuppies, links*are one of the most wonderful
things the internethas given us.The most popular sites

---

## Page 48

on the internet are devoted, in fact,to the sharing of links
between friendsand strangers.Making proper use of links
letsus attaina sort of Holy Grailin technicalwriting:
The core idea here isthat you should break your writing
into bite-sizedpieces,often calledtopics,none of which
overlap in content. Doing so means that ifthings change
—and things always change—you only have to update
the documentation in one place,Many topics are short,
whereas others are quite long. What topics should be
is relativelycomplete in their discussion of a particular
subject.Unlike books, where you can assume in chapter
seven that the reader remembers chapter six, topics
assume very littleknowledge of other topicsand include
plentyoflinks.
Unfortunately,the nature oflanguage and learningmeans
thatsome amount of duplicationisalways going to occur.
But for the most part,linking liberally,arranging topics
in a sensibleway, and trying to adhere to a singlesource
model isa good idea.reStructuredText and AsciiDoc even

---

## Page 49

allow you to embed fileswithin other files,which further
aidsreusability.
The worst duplication sin of all is to store similar
copies of the same documentation in version control.
The root cause here is typicallythe desire to have one
version for coworkers and another for customers, and it
inevitablyleads to a maintenance nightmare. Instead of
multiple copies,the better approach is to use a feature
sometimes called“conditionaltext."Conditional text lets
you selectivelyinclude or exclude files(or portions of
files)in the finaloutput. AsciiDoc supports conditional
text under the name “conditional inclusion macros."
reStructuredText supports itthrough Sphinx with the . .
only:: directive.Unfortunately, this feature is not
presentinMarkdown, Attempts toadd itcan be charitably
describedas "hacky,"so ifyou relyon conditionaltext,you
might want to selectanother language.
Make Static Websites
I have perhaps an irrationalbias towards staticwebsites.

---

## Page 50

I love them. I love their speed, simplicity,portability,
and security.You can host staticwebsites practically
anywhere, including Amazon S3 and GitHub Pages.
They have no server-sideapplicationdependencies, no
databases,and nothing to install,so migrating the entire
siteisas easy as moving a directory.Because allithas to
do isservepages (ratherthan generatethem dynamically),
the server needs very few hardware resources.You can test
staticwebsites on your localcomputer without installing
anything and compress and ship them with software
applications(although you shouldn't unless you have to),
There's no WordPress instance for someone to hack or
comments sectionforbots to spam. Nothing ever crashes,
because there'snothing to crash.2
Sure,you could manually createa simple staticwebsite,
but to do anything complex, you'll want to use a
generator. The basics are that you provide a staticsite
generator with content (lightweightmarkup) and a theme
(templated HTML and CSS), and itprocesses everything
intoa working website.To update the site,justmodify the
content and processeverythingagain.

---

## Page 51

Many staticsitegenerators exist,far too many to list.In
fact,I'm sure some new, amazing staticsitegenerator is in
development rightnow, and Ialready feellikea jerkfornot
mentioning it.But ifIhad to suggest a few:
+Hexo
Any one of these tools can create a beautiful, functional
documentation website, Jekyllis the most popular. That
said,IfavorSphinx fortwo major reasons:
-It was specificallybuilt for documentation, rather
than blogsor marketing sites,so ithas a robust system
forgenerating nested navigation menus.
+It features JavaScript-based search out of the box.
Every other tool in that list(except MkDocs) does

---

## Page 52

not have out of the box search and relieson Google
Custom Search, Swiftype, Algolia,Lunr, or some other
searchsolution.Adding a searchsolutionto a static
siteoftenmakes ita whole lotlessportable,so Sphinx
has the rightideahere.
Whichever tool you select,take the time to customize
the theme. Focus on navigation and approachability,Find
a designer and ask for help with colors,typefaces,font
sizes,page width, and spacing.This customization isyour
chance to differentiateyour content from the thousands
of ugly,disorganizedsitesof the world, so don'tjustuse
the default theme. Ifyou don't have the skillsto do this
customization yourself,you might need to hire someone.
It'sthatimportant.
And make sure you have a search solution.
Ifmaking a staticwebsite sounds likea lotof work, well,
itisn't,but an even simpler solution exists:GitHub wikis.
The secretwith GitHub wikis isthat they‘rereallyjusta
collectionof lightweightmarkup filesthat you can edit
using your favoritetext editoror through a web browser.

---

## Page 53

GitHub wikis support Markdown, reStructuredText,
AsciiDoc, and some other languages that you shouldn't
use.
You don'tget a lotof flexibilityin how the resultingpages
are organized—just an alphabeticallist—but you can make
a tableof contents on the home page and have a highly
functional sitewith very littleeffort.You losethe ability
to make your website beautifuland unique, and GitHub
wikis do not have search.But those might be worthwhile
trade-offsforsimple sites.This way, atleastyou'restoring
lightweightmarkup filesin a DVCS. You can always create
a bettersitelaterusing those same files.
Rsync
Staticsitegenerators typicallyregenerate the entiresite
for even simple changes. This behavior helps ensure that
the changes didn'thave any unforeseen consequences and
that the sitewillwork properly.However, italso means
that copying your new siteonto an older version of the
site (via FTP or SCP) can result in removed or renamed

---

## Page 54

filesnot being overwritten and persistingon the server.
The easy solutionisto deletethe old sitefrom the server
beforecopying overthenew site,but a toollikeRsync can
save you the hassle.Rsync transfersonly the filesthatneed
to be added or updated, and itdeletesstalefiles.Rsync is
often used to keep staging and production serversin,well,
sync.
Ifyou use Windows, you probablyneed Cygwin to take
advantage of Rsync, On macOS and Linux, installationand
usage ismore straightforward.
Note
If you use Amazon S3, the AWS Command Line
Interface has a sync function that works similarly
to Rsync.
A slightlymore complicated alternativeis to configure
your production server as a remote repository and push
the finished site to it,which accomplishes the same
thing: new filesget added, existingfilesget updated

---

## Page 55

(ifnecessary),and stalefilesget deleted.Unsurprisingly,
GitHub Pages uses thismethod.
Metrics
If you aren'tkeeping an eye on documentation metrics,
you'remaking a huge mistake.User researchiswonderful,
but knowing exactlywhich pages are most popular, your
site'sbounce rate,and common behavioralflows are all
invaluable. Create a Google Analytics account, add the
provided tracking code to your staticsite theme, and
check the numbers regularly.I'm sure other toolsexist,
but Google Analytics is simple, free,and the industry
standard.I'veneverused anythingelse.
Metrics rarely serve as an obvious pointer to the correct
course of action.Rather, they serve as a valuable check
against your thoughts and intuition.Ifyou create what
you think isan amazing bit of documentation, and sure
enough, it'sone of the most popular pages on the site,
perfect!If it'snot very popular, maybe no one can find
it,or maybe it'snot as useful as you thought. Deeper

---

## Page 56

investigationmight reveala major flaw,a minor tweak, or
a reasonable explanation that requires no change at all.
But not having metrics and using only your own criteria
forsuccess can be disastrous.
Note
Customers often frown upon a native application
“phoning home"—especially to a third-party like
Google—with usage metrics. Gathering these
metrics from a native applicationrequires costly
development work, which is yet another reason
why onlyhosting your documentation on a website
isthe betterapproach.
In the software industry,you often hear the questions,
"What does good look like?”and "How do you measure
success?" For a documentation website, any answer
should include some mix of metrics, bug numbers®,
reader feedback, alignment with corporate strategy (if
applicable),and finally,personal intuition.If you have
accessto metrics from other teams, comparative analysis
often yieldsthe most valuable insights.How does the

---

## Page 57

number of documentation bugs compare to the number of
callsto customer support? Do the most-used featuresof
the product correlatewith the most-visitedpages of the
documentation?
I'm sure other ways of measuring success exist. I'm
probably just ignorant to them. Detecting the difference
between good and great documentation is an incredibly
hard, unsolved problem, but that doesn't mean we can give
up trying to solve it.Consider the following statements
from two hypotheticaltechnicalwriters:
"In my professionalopinion, the content is clear,
concise, correct, and complete. The language is
professional,conforms to our styleguide,and projects
a strong brand. Some of the tables were too wide
for print,so we now enforce a two-column limiton
alltables.Overall,I'm happy with the quality of the
documentation."
-"The applicationlogs show that the product only has
1,300 users,yet the documentation received 2,400
page views lastmonth, In thatsame timespan, readers

---

## Page 58

reported six inaccuracies, all of which I resolved
within 72 hours. The fivemost popular search terms
returnthe pages Iwould expect,and the designteam
recentlyhelped me optimize the header margins for
readability.Overall,I'm happy with the qualityof the
documentation."
I sincerely hope that you find the second argument
more compelling. In any field,opinions become more
crediblewhen you attach quantitativemetrics to them.
Documentation isno different.
ScriptYour Complexity Away
If you go against my advice and decide to create and
distribute PDFs, you might have to create a so-called
publishing pipeline.Publishing pipelines are the steps
through which lightweight markup filesbecome print-
ready documents. Alllightweightmarkup languages build
to HTML, but the journey to PDF often requiresan extra
step—hence the pipeline.You probably have to build
to LaTeX first,then LaTeX to PDF. LaTeX installersare

---

## Page 59

massive 1.8 - 2.5 GB downloads, so if you use a set of
machines to build your documentation, consider using
justone as the PDF machine.
Pandoc is a marvelous tool for converting between
markup formats. It callsitselfthe Swiss Army knife of
markup converters and can convert to and from a huge
number of formats. Unfortunately, these conversions are
rarelyperfect.Ifone day you decide thatyou'd ratherwrite
in AsciiDoc insteadof Markdown, expect to perform some
manual cleanup afterrunning the conversion script.
For simplicity,Pandoc conceals the LaTeX step, which
makes the creationof PDFs prettystraightforward:
pandoc your-document.md -f markdown_github
-o your-document.pdf
Note
You can even convert to the Microsoft Word
document format by specifying .docx instead
of .pdf.

---

## Page 60

Unfortunately, this method only works if all of your
content is in a single file—unlikely.More likelyis that
you'llneed todo something likethis:
pandoc title.txt 1.md 2.md 3.md 4.md -f
markdown_github -o your-document.pdf
Note
If you want to customize the way the PDF
looks, doing so requires a new LaTeX template
and is extremely complex. If customization is
important,considerusing a toollikewkhtmltopdf
or PhantomJS so that you can use CSS instead
of LaTeX for styling.Whatever you do, don't
compromise the look of your HTML in order to
have more attractivePDFs. Everything you do
should be geared towards more useful,accessible
websites.
You stillwant HTML, though, so you should include a
second buildcommand inthe same script:

---

## Page 61

jekyll build --source source --destination
build/html1
You might need to check out severalremote repositories
before building, rename or move files, or run a
supplemental script.The point is that your lightweight
markup filesshould be as simple as possible.Don't require
people to conform to sillyguidelines in theirwriting (or
worse, write in XML) just so your build scriptis a little
easierto understand, Ifany part of the technicalwriting
process should be complicated,thisisit.You might need to
read a book on Windows PowerShell, Bash, Rake, or Grunt.
1.Lightweight markup goes in (simple).
2.A scriptchecks out a Git repository,appliesa custom
theme, compiles LESS filesto CSS, converts Markdown
filesto AsciiDoc,and finallyruns the build commands
(complex).
3. A staticwebsite comes out (simple).
Commit the buildscriptto the documentation repository
and use README .md to explain what itdoes and which
dependencies it has. In this case, I might listPandoc

---

## Page 62

and Jekyll as dependencies and provide links to their
installationdocumentation.
Ifyou use Rsync, you probably don't want to include itin
your build script.Making a separate"publish"scriptthat
callsRsync givesyou the opportunity to manually verify
that the help system opens and functions properly before
you send itto a remote server.This final,ten-second sanity
check isworthwhile.
The Legal Problem
Unfortunately, doing your job well might actuallycause
lawsuits. I'veheard unsubstantiated rumors of patent
trollsusing publicly-availabletechnicaldocumentation as
evidence of infringement.In thiscase,the open, forward-
thinking spiritof enabling users to contribute to the
documentation can be financiallydisastrous for your
company. You might need to keep your source filesin
an internalrepository,rather than GitHub. Further, you
might need to protectyour documentation website behind
a customer login page. You should stilluse lightweight

---

## Page 63

markup and distributedversion controlso thatcoworkers
can contribute,but the generalpublicmight not be ableto.
In short,assholesruin everything.
Localization
Localization, the process of translating documentation to
other languages,isa nightmare. Ifyou ever thinkyou need
to doit,interfacewith management and perform a careful
cost-benefit analysis, because the process is expensive,
time-consuming, error-prone, and tedious. Once you've
arrived at what you believe is an accurate estimate for
company costs,tripleit.Now you havea realisticestimate.
Ifyou try to keep alltranslationsof the documentation in
sync at alltimes,you can'tpublish very often,which leads
to lower qualitydocumentation. To fixa bug in your native
tongue, you update the content,build,and publish.To fixa
bug ina translatedcopy ofthe documentation, you update
the content, manually send itto a translationcompany,

---

## Page 64

wait days or weeks to receive the updated content, build,
and publish.
Because publishing in a singlelanguage isso simple, you
can work with increasedvelocity.You can improve large
chunks of text,reorganize pages, fixawkward wordings,
and generallytreateverything as a working draft.Writing
content for translationmeans meticulous review of new
content,because any inaccuracy has to go through costly
revisions.Itmeans rarelyrefactoringold content because
of the sheer expense involved in translatingitinto eight
differentlanguages again.2 It means delaying software
releasesbecause it'sCarnivalin Brazil®and the Portuguese
translationswon't be ready foranother week.
Lest you doubt me, consider this common open source
localizationworkflow:
1.Write a script that callsgettext, a translation tool,on
each of your lightweightmarkup files.This operation
produces a collectionof POT files.What POT stands
for doesn't reallymatter. Conceptually,POT filesare
just line by line splitsof your source filesinto two

---

## Page 65

strings:the originalone, and an empty one for the
translatorto fillin.They look likethis:
msgid "My name is Andrew."
msgstr ""
msgid “Another paragraph."
msgstr ""
.Stillusing gettext,generate setsof PO filesfrom the
POT files,one set per language. Send the PO filesto
the translationcompany, who will inserttranslated
content into the empty strings.PO fileslook nearly
identicalto POT files:
msgid "My name is Andrew.”
msgstr "Je m'appelle Andrew."
msgid "Another paragraph.”
msgstr "Un autre paragraphe."
.When the translationcompany returns the PO files,
commit them to version control.

---

## Page 66

4.Then you—sadly, this is not a joke—convert the PO
filesto MO files,again with gettext.MO filesarebinary
compilations of PO files.Because PO filescan be rather
large,you compile them to MO filesto improve the
speed atwhich a machine can processthem. You don't
need to commit the MO filesto versioncontrol.
5.Buildand publish the translatedhelp system from the
MO files.
6.Repeat these steps each time you need to update the
translatedhelp system. Even though it might feel
as ifyou'reoverwriting the translatedPO fileswith
new, blank ones, the PO fileswill retain their existing
translations.The translationcompany can then fillin
the gaps createdby new or modified content:
msgid “My name is Andrew."
msgstr “Je m'appelle Andrew."
msgid "A new section."
msgstr ""

---

## Page 67

msgid "Another paragraph."
msgstr “Un autre paragraphe."
You don't have to follow this workflow.2 In fact,your
static site generator might not even support building
from MO files.I'veonly provided itas an example of the
complexities involved in the localizationprocess,I'm not
being melodramatic; itreallyisa nightmare,
For a method that uses common tools (i.e.Git),you might
try:
1,Send your lightweightmarkup filesto the translation
company as-is,Tag the latest commit in your
repositoryto mark thispoint in time.
2. When the translated files return, run a linter on
the files,because invariablythe translationcompany
will have messed up the whitespace on your
documentation. Then commit the translatedfilesto
version control.
3.Build and publish the translatedhelp system.

---

## Page 68

4.When you want to update the translatedhelp system,
make a new branch and usegit rebase to squash all
work between now and your tagintoa singlecommit.
Then send the diffto the translationcompany, along
with the latestlightweight markup filesfor both
languages.
5.Delete the temporary branch and mark the latest
commit in the repositorywith a new tag.
Remember, you have to repeat this process for each
language.Some specializedsoftware applicationspurport
to simplifythe translationprocess—and to be fair,I'm sure
they do help a bit—but until computers can accurately
translate between languages, localizationwill remain
messy and expensive.
Contrived Workflow
This section provides an end-to-end, functional example
that conforms to allof my guidelines,with a few detours
to make itmore realistic,

---

## Page 69

1.You get hired ata software company. Congratulations!
2.Three weeks (or months) later,you are wise and
knowledgeable about the company's products and
users,You also have your health insurance allsorted
out.
3.You create four different files in GitHub
Flavored Markdown: about.md, tutorial.md,
concepts.imd,and process.md.
4.YouinstallSphinx withpip install sphinx.
5.You create a directory structure and Sphinx
configuration file(conf.py) by running sphinx-
quickstart.
6.You try to build these Markdown files into
a help system with Sphinx, but Sphinx uses
reStructuredText, not Markdown. You curse several
times.

---

## Page 70

7.You use Pandoc to convert the filesfrom Markdown to
reStructuredText,but afterexamining the resultant
files,you decide you hate RST and would rather
continue to write in Markdown.
8.No problem, you createa scriptthat converts allof
your Markdown filesto RST and then builds with
Sphinx. This way, you can write in Markdown, but still
take advantage of Sphinx. The scriptlookssomething
likethis:
find . -name \*.md -type f -exec pandoc
-f markdown_github -t
rst -o {}.rst {} \;
sphinx-build -b html ./source ./build
9.The scriptworks, but you stillneed to builda TOC tree
(table of contents) for Sphinx. You createa filecalled
index.rst and embed the converted content from
about .md within thatfileso thatyou have towriteas
littleRST as possible.index. rst lookslikethis:

---

## Page 71

10.
11.
++ toctree::
:maxdepth: 1
tutorial
concepts
process
-- include:: about.rst
Everything looks pretty good, so you createa new
repositoryon GitHub, clone the empty repositoryto
your computer, and add your documentation to it.
When you commit your files,you noticethatyou need
to edit .gitignore to ignore build (thebuilthelp
system) and *.rst (the converted RST files)except
index.rst. .gitignore looks likethis:
build/
source/*.rst
!source/index.rst

---

## Page 72

12.
13.
14,
15.
You realizethat anyone who views the repositoryon
GitHub willhave no ideawhat itis,how to build it,or
how to contribute to it,so you add README. md to
the repositoryroot.
You decide that the defaultSphinx theme stinks,so
you download a new one and point conf. py at it.
Then you decide that one stinks,too,and take the
time to learnhow to buildyour own.
Once you're happy with how everything looks,you
harass your IT department untilthey give you the
subdomain docs.yourcompany.com. When they ask
what sort of server you need and what you need
installed,you tellthem thatyou builta staticwebsite
and justneed a directoryforfiletransfers.They're
superimpressed.12
You transfer the finished help system to
docs.yourcompany.com and areofficiallya published
writer.

---

## Page 73

16.Three days later,some developers approach you
about a change to the documentation. You tellthem
you're busy and that they should submit a pull
request.They too aresuper impressed.41
17.Promotions and financialwindfallsensue.
What About Wikis
Admittedly, a wiki is simpler than the system I just
described.Anyone can figureout how to edit a wiki,
which is a killerfeature until it isn't.Wikis have huge
benefitsand huge drawbacks. They certainlyhave a place
in technicalwriting,but you should think carefullybefore
selectingone.
Users don't need to installany applications,clone any
repositories,or learn any strange workflows to contribute
to a wiki. They can spot an issue, click Edit, and fix it
within ten seconds.The process isremarkable. Also,every

---

## Page 74

major wiki has out of the box search,a huge improvement
over most staticsitegenerators.
One major problem, however, is that wikis are web
applications.If you decide to create and host one, they
require maintenance over time. And ifyou've ever worked
at a company with an internalwiki,you know how often
they crash or slow down. Yes,Wikipedia has proven that
wikis can scale to a huge number of users with good
reliability,but that scalingis the resultof a ton of hard
work from some very smart people,people whose job itis
to manage the site.Personally,Iwant tospend the smallest
possible percentage of my time managing a site. I'drather
test,research, write, and curate content. Static sites are
indisputablysimpler to manage.
To be blunt, writing on a wiki sucks. Mercifully,some
wikis use lightweight markup, but itisoften a mangled
form that incorporates a subset of HTML tags and barely
qualifiesas "lightweight."Others use a WYSIWYG editor,
so the experience islikeusing Microsoft Word without all
the convenient keyboard shortcuts.Everything in a web
browser is so ephemeral, ready to be flushed at any time.

---

## Page 75

I'velostat leasta few pages of work to connectivityissues
and Firefoxcrashes.Writing lightweightmarkup ina text
editor is faster,easier,and safer.GitHub wikis, which
I mentioned earlier,are an exception to this rule (and
several others in this section).
Wikis are fantasticfor livingdocuments that grow over
time and never need to be marked as belonging to a
particularsoftware version.Many software as a service
applications fit this description, Supporting multiple
versionsof your documentation—for example, version 3,1
and 3.2—is trivialwith distributedversion control.Doing
the same on most wikis requires specializedplugins and
some manual shufflingof content.
Version control systems like Git do an amazing job
trackingchanges over time.You can view the change log
for individualfiles,easily"blame" others for problematic
content, see related changes that have been lumped
into commits, and merge disparatecommits easily.With
most wiki software, you can only view the change log
for individualpages. Pullrequests in distributedversion
control serve as a built-inreview process for changes.

---

## Page 76

Because most wikis follow the “last person to edit
wins" policy,you might not even notice a destructive
change to the documentation. Wikipedia amelioratesthis
problem with a sophisticatedanti-vandalism bot that
uses machine learning to improve over time. Given my
expected lifespan,I'm confident that I could never create
such a bot.Your mileage may vary.
Ever gotten work done froma plane,train,park,or hipster
coffeeshop that refuses to offerwirelessinternetaccess?
Not with a wiki, you haven't,With distributedversion
control and staticsitegenerators,you have everything you
need to write,build,and review changes locally.When you
have connectivityagain,you can push your changes and
update the website.
In short, for a wiki to make sense, your documentation
should be uncontroversial and never need to be versioned.
You alsoshouldn'tmind writingin an inferioreditor,only
working online, and maintaining a piece of enterprise
software.

---

## Page 77

10.
.As of September 2015.
.Source: conjecture.<
.The default"gridtables”are horrifying,but CSV tables
and listtableswork well.«
.Please don't callthem hyperlinks.-—
.Aside from the serveritself,anyway.
.Number reported, severity of each reported bug,
average time to resolve,etc..—
.Translation memory can only help so much.»
.Or Golden Week in Japan, etc,<
.And probably shouldn't.
To show you how impressed they are,IT buildsyou a
Linux VM with 256 MB of RAM and 3 GBof disk space
and refusesto giveyou superuser privileges...

---

## Page 78

11. But they stilldon'tsubmit the pullrequest.

---

## Page 79

11. But they stilldon'tsubmit the pullrequest.

---

## Page 80

The Grand Finale
Having finallyfinished this book, I'm a bit depressed—
turns out everything I know about technicalwriting can
be covered injustover 10,000 words.
The point,Iguess,isthat technicalwriting doesn'tneed to
be complicated. Technical writers have justspent several
decades convincingpeople thatitshould be.No partof the
job iseasy in execution,but allof itshould sound easy in
theory:
1.Learn everything about a subject.
2.Write down exactlywhat an audience needs to know
and no more.
3.Make the content beautiful,discoverable,scannable,
and searchable.
4.Consider everything a draft,and iteraterelentlessly.
5.Make contributionsimple.

---

## Page 81

I wish I had something more all-encompassing to
say, something that would tie technical writing into
storytellingor poetry or life.But no, technicalwriting isa
job likeany other,andI believethisbook can help you do it
a littlebitbetter.

---

## Page 82

Acknowledgments
Even a relativelyshort and simple book like this
one is a colossal task. Many thanks to my wife,
family,and colleaguesfor theirinvaluablefeedback and
encouragement throughout the process.
I'dalso like to thank all the readers who helped make
thisbook such a success.Ifyou enjoyed Modern Technical
Writing, pleaseconsider leavinga review on Amazon.com.

---

## Page 83

Legal
© 2016 Andrew Etter
Allrightsreserved
