**Daniel Laird**
**Head of software, media processing and delivery**
**MediaKind**

Started as an embedded engineer at phillips (used to writing tiny things)

#####What's special about MediaKind's journey?

Can't start from scratch, people see it as wasteful
Support agreements mean that you can't test on customers easily
Had to work in place

Broadcasting thought it was special
Made bespoke hardware for their own DC's
Custom hardware/cabling standards
Specialised engineers to support this pyramid of specialness

What changed to make them more generic to the rest of us?
Software performance on FPGA's became good
The customer wants new features infrastructure
Using normal hardware lowers OPEX and allows competitive pricing

---

Moving from specialised hardware/software to containers
initially delivered "fat" containers (5-600MB*number of containers required)
Why?
*   R&D didn't have to change much
*   More agile than hardware
*    Changes had to be made

Challenges:
*   Adopting Kubernetes
*   Learning how to deliver containers

# He, as a Broadcasting org is calling 500MB images "gigantic". People are nodding.

####multi stage builds are good
####only ship exactly what's required
if devs _need_ to be able to get into a shell in a container then ship a dev and a prod image
##if you can use `scratch` _use `scratch`_!

In C they use LDD to find libs, is there something like this for Java?

Creating an RPM DB in the container means that you can submit CVE's that will be shipped with the app to customers who have the container delivered to them

Is something like a local RPM DB possible with `apk`?

##Running as root in containers is pretty much the 8th deadly sin

https://github.com/GoogleContainerTools/distroless

Key Lessons MediaKind Learnt:
1. You don't have to make a clean start
2. Optimise delivering the solution, not the containers
3. Keep up with the technology, it moves pretty quickly. Time was there were 10's of deployment methods for containers. Now it's pretty much just k8s or maybe openshit.
    3a.   embedded software practices are very applicable to containers

####Questions:

They've had customers who are more worried about knowing what risk they're exposed to over getting the risk removed right this second.
