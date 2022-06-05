# This is my take on the challenge given by Babbel for their Senior Product Analyst role.


# Case Study for Product Analytics

# Candidates

## Instructions

ThiscasestudyisbasedonactualdataandbusinessproblemsfromBabbel.Itisconfidential
and should not be shared.

Thisisyouropportunitytoshowoffbothyour **dataanalysis** and **visualization** skillsandyour
ability to **communicate** your findings to an audienceof typical stakeholders in a compelling way.

Pleaseworkthroughthebelowcasestudyandprepareapresentation(Powerpoint,Keynote,or
comparable)towalkamixedaudiencethroughyourresultsduringyourcasestudyinterview.
You’llhave **20-25minutes** topresent.Afterwards,therewillbeabout 20 minutesoftimefor
questionsanddiscussion.InlightoftheCOVID-19pandemic,pleasebepreparedtopresent
yourslidesremotelyusingGoogleMeet(formerlyHangouts)andensurethatyourbrowserisset
up for screen sharing.

Imagineyouraudiencewillbeyourtypicalstakeholdergroup(aswellaspotentialteammates):

likes straight to the point, likes actionable, likes easy to read.

Weexpecttheentirechallengetotakeyou4-5hours,butyoumaydedicateasmuchtimeas
you like.Pleasenote that weexpect youtosubmit your presentation **withinoneweekof
receivingthiscasestudy**. Feelfreetochoosewhatevertoolyouliketoanalyzeandvisualize
thedataattached,mayitbeExcel,Pythonoranythingelse.Incaseyoudonotmanagetowork
through all questions, just let us know what you’d like to do.


## Learning Engagement in the Babbel Ecosystem

Babbelisaqualityleaderwhenitcomestolearningalanguageviadigitalself-study.Webuild
ourproductforthosewhoareaimingtobecomeconversationalinalanguageandarewillingto
pay for achieving this goal.

Our products offera portfolioofLearning Experiences– differentfeaturesofferinglearning
activities with a stand-alone learning value proposition. Our main learning experiences are:

- **Lessons** – shortunitsthatintroducevocabularyandgrammarviacontextualcontent,
    including exercises
- **Review** – vocabulary review to practice previouslyintroduced words and phrases
- **Audio experiences** such as Podcasts
- **Games** – fun and casual ways to practice vocabulary
- **LiveClasses** – Digitallive classroom (60min)witha teacheranda smallgroupof
    students
Therespective learningcontentfor theseisdesignedbyourteam oflinguistic expertsand
language teachers, and specifically tailored but not necessarily available ineach learning
language.

### Task

Aproductteamapproachesyouto **analysehowBabbellearnersusinggamesareengaging
withotherlearningexperiences** andidentifypossibleavenuesforimprovement.Theoverall
goal of the team is to activate learners in their early learning journey.

Pleaseusethe attacheddatasetandthefollowingguidingquestionstoanalysethelearning
engagement performance of games, and point out optimisation potential:

1. Giventhe datayouhaveavailable, how wouldyouoperationalisetheteam’sgoalin
    terms of specific metrics?
2. How do games perform differently across learner segments?
3. Howaregamesbeingusedinconjunctionwithotherlearningexperiences?Howdoes
    this behavior relate to the team’s overall goal?
4. Assume that the team is planning to build a game aimed at activating new learners.
    TotestifthegameachievesthisgoaltheteamplanstoreleaseitasanA/Btestbutis
    unsurehowandwhereexactlytoexposenewsubscriberstoit.Fromyourexperience
    andinsightsgatheredfromthedatasetprovidedhere,whatwouldyousuggesttothe
    team? Are there any risks they should be aware of?

Beyondthedatayouhaveathand,whatkindofmetricswouldyouusetomonitorthelearning
engagementacrossdifferentlearningexperiences?Whatkindoftrackingwouldneedtobein
place for this?


### Data

Thedataset“learning_sessions.csv”containslearningsessiondataofsubscribersintheirfirst
weeks with Babbel. Each row represents a unique learning session.^1

```
Columnname Definitions
```
```
uuid String, user identifier
```
```
subscription_started_at Timestamp of the start of the subscription (in UTC)
```
```
age String, age bracket of the user
```
```
motivation String,answertoquestionduringregistration:Whatisthemainreason
you want to learn a new language?
```
```
subscription_type The last node visited by the visitor (Registration funnel consists of 8
nodes.)
```
```
geo_area String, indicates the geographic areas that the subscription was
purchased from
● ESM (English speaking other than U.S.A)
● GSM (German speaking)
● FIM (French speaking)
● SPM (Spanish speaking)
● USA
```
```
learning_activity String, indicates the learning activity used in the session
```
```
learning_os String, indicates the operating system of the user’s device
```
```
learning_language String, indicates the language the user is learning
```
```
session_ended_as String, state in which the session was ended(completed, aborted,
missing)
```
```
session_started_at Timestamp of learning session start (in UTC)
```
```
session_local_started_at Timestamp of learning session start in user’s local timezone
```
```
time_spent Float, minutes spent learning
```
(^1) The data hereiscloseto whatyouwouldbefacinginanactualanalysisbutwehavesampled,
anonymised it, and changed some details here and there so as not to expose any sensitive information.


