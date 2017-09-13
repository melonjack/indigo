# Swift, Class Clusters, and the Objective-C Runtime

Recently, I've started working on a brand new project on the side, 

Going into the project, I knew I had three distinct "levels" of code 

In Apple's own terms, a class cluster is "an architecture that groups a number of private, concrete subclasses under a public, abstract superclass. " In other words, you initialize a public class, and depending on the provided inputs you give it, the framework will return you a private subclass best suited for the supplied inputs. I highly recommend reading [Apple's documentation of Class Clusters ](https://developer.apple.com/library/ios/documentation/General/Conceptual/DevPedia-CocoaCore/ClassCluster.html) for more information on the subject, but this should be enough information to understand the rest of this post.

Anyway, back to the issue at hand. 


