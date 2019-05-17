**Mike Bursell**
**Red Hat**
**Chief Security Architect**

##### Intro
got intro'd

##### How containers are like vms
self-contained/images/scheduled workloads/host based security
containers are more lightweight but have less relation to hardware
vm's have security provided in part by hardware

so are vm's more secure than containers?
it's the wrong question apprently

##### What is a container?
it's a linux process with isolation:
*   namespaces
*   cgroups for resource management
*   selinux (sometimes)
*   seccomp

this is what's seen by an ops person apparently
securty whingebags

containers are launched from images:
*   pre-prepared packages
*   aimed at specific use cases
*   live in repos

this is what's seen by a developer
bunch of cowboys

##### What's Security?
good security is built around the container lifecycle

How containers aren't like vms
containers are:
*   lightweight
*   short lived (not around for as long to be compromised)(if running containers, recycle them regularly so that if they're compromised they're no longer compromised)
*   redhat container repo plug
*   well suited to CI/CD (anchore compliance checks)
*   easier to decompose
*   trusted repos for images


security and controls


?
