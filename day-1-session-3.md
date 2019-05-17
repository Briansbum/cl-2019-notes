##### Kris Buytaert
@krisbuytaert

What has ops (automation) got to do with Dev?

damon edwards and john willis <- podcast

CLAMS
Culture
(Lean)
Automation
Monitoring and Measurements
Sharing

NoOps? YOLO Ops?

Kris doesn't like hype

##### History:

*   Europe:
    *   Starting from  Ops
    *   improved arti quality
    *   less pain / more stability

*   US:
    *   Push from development
    *   Faster platforms
    *   Faster change

##### Transistion cases:
###### Case 1, Chaotic Ops:
Initial State

    Complete chaos
    v. v. low reproducibility
    No Automation
    CI is only on one dev's desk
    Ops are only fighting fires
    No standardisation between environments

0 -> 3 months

    Build using Jenkins + build servers
    CI for IaC
    Testing code
    Staging for Infra code
    Take the config out of the code
    Upgrade whilst still deploying

0 -> 6 months

    Stack alignment (50 -> 1 jdk/jboss)
    IaC all the things
    90% reproducibility
    Standardised builds

Conclusion

    Get ops to automate
    Get them using the same tools as the devs
    Devs can help the ops people improve (they're on the same toolchain)
    Collaboration ++
    Velocity ++

###### Case 2, CI by Devs:
Initial State

    Some devs have tests that do nothing/little
    Some dev teams are doing "CI"
    Deployments are chaos
    Ops nag about arti quality

0 -> 18 months

    Found the first ops person in the business
    Others were mostly David Brent
    Most of them not in the office
    Focus on one team, move them to a different city
    Teach them Agile
    Adopt IaC
    First success @ 18 months
    Move those people back to their original teams once they're excited

18 -> 24 months

    Old ops people are now Agile nutbags
    Peach kanban for ops and scrum for devs
    Writes tests for his IaC

Conclusion

   Starting with dev made rollout slower
   Ops should not be spending all of their time firefighting

###### Case 3, Countries are fighting:

Initial State

    Country 1 has full IaC with CI
    2 has no IaC but claims they do, no test coverage, manual deploys
    3 has to deploy in 2, lots of pain
    Once 3 is allowed to deploy in 1 the pain vanished

Conclusion

    You can fake automation until someone who has done automation shows up.

###### Case 4, Ops is not involved at all:

Initial State

    Large Transformation
    devops team tells people to use tools that they don't use
    devs complain about awful/broken tools
    tools enforce a manual process

2 Years later:

    average "devops" person lasts 2 months
    senior management has peaced out (2 versions of sm)
    only the analysts remain (not devs or ops)
    only contract devs left
    moving to a private cloud for some reason without fixing underlying issues, deployment via emailing reqs in word documents
    legacy container ecosystem (an old k8s stack)

Conclusion

    Involve skilled ops people

##### Why ops first?
You can't support/understand what you're making
Unblock delivery/provisioning by getting ops to make what you need before it's needed

##### On prem vs cloud
So many things you need to make (TF, VPC, Pipelines, Monitoring, Security)
In both cases ops has a major role

"it works in my container" <- lol

Micheal Ducy - containers in dev vs prod

Devoops -> forgetting to do the things ops has to do until you're done writing the thing

##### Waterfall & ITIL vs Agile
Lots of older ops people are still not doing Agile and need help to adapt

##### A CI Ecosystem
Things ops people might not know:

    vcs
    deployment
    build tooling
    arti repo
    code coverage tooling
    testing tools

# CI is a security requirement

# Get the mean time to repair as close to 0 as possible

its not about the tools
its about change
it's about the people
