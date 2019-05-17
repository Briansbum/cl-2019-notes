who?
from where?

operability is the ability to
diagnose
restore
monitor
failover
cleardown
specialness
inspection
reporting
security

users don't always care about these things

operability is long term customer experience and service viability and not short term feature delivery
addressing these things early helps us to make the spend associated with the service more sustainable and lower the load on individuals

#### continuous delivery

**books:**
continuous delivery - jez humble & dave farley 2010
continuous delivery with windows and .NET - matthew skelton & chris o'dell 2016

Needs:
*   good engineering practices
*   fast feedback from pipelines
*   team ownership of software and services
*   software/infrastructure needs to be aligned to make CD as easy as possible (microservices helps with this)

#### case study

GOV.UK
700+ people across 70+ teams and 7 locations
time critical delivery (brexit)

A complicated env with:
*   a need in increase speed + safety of delivery
*   multi year programme
*   brexit

At this point the presentation was going quickly

They had to manage lots of people with different ideas of what continuous delivery is

They were trying to force a "one size fits all" architecture approach <-- I'm guilt of this

Defining the platform is important, and telling people about the definition is even more important

Things conflux did to help:

Focus on the "operator experience"
How are the ops/support people managing to deal with caring for systems

Defining the platform - runbook dialogue sheets
Big A1 sheet on a table with everything that operators will need/need to know in order to make using the service simple/less painful

github.com/skeltonthatcher/run-book-template

endpoint healthchecks, make certain that everything has a healthcheck. nothing is too small for a healthcheck
