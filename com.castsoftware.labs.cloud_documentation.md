# _com.castsoftware.labs.cloud_ Description
This extension provides computation of the following new assessment indicator(s)
* the *CloudReady index*
* supporting Technical Criteria

##  Problem Statement
With Cloud deployment adoption, Cloud deployment failure story also abounds.

The reason it becomes harder to ensure software quality is that the cloud creates an opportunity to deploy applications in a much simpler way. And although it’s not difficult to put an application in the cloud to try it out, it's difficult to put an application that is able to withstand the test of real production in the cloud. End-users don't understand the difference between a try-out application and a resilient application.

The difference lies inside the application architecture and is independent from the size of the deployment environment. So while IT departments would have asked for requirements in terms of capacity planning (for example: how many end-users? How many transactions per hour?), no such planning occurred with try-out applications that were deployed in the cloud by the marketing departments themselves.

They understand from the marketing buzz that it’s simple, fast, has capacity on-demand, etc. But they won’t understand the caution IT departments take before deploying an application, and they won’t understand why they ask for some time to make the application scalable. They think, “With the cloud, you can simply activate more horse power with a click of a button and some credit card info!”

They don’t realize that an application not designed to be scalable will not become scalable simply because it runs on ten more servers. With this in mind, you can understand that having the right architecture blueprint and -- more importantly -- sticking to it from the start, is a key factor of success.

## Research Labs proposal
To identify pieces of Software that could be optimized to withstand unexpected workload, increased "scrutiny" from hackers, "seamless" evolution of execution environment, the Research Labs offer a solution based on CAST AIP Assessment Model.
* The *CloudReady Index* is a Business Criterion that aggregates Quality Rules from existing high-impact Efficiency-, Security-, and portability relatedTechnical Criteria
* Grouped in new dedicated Technical Criteria
The Research Labs released this first version of the CloudReady Index to leverage the expertise and experience of customers in order to fine-tune its exact composition and collect feedback.

## Formula
The CloudReady Index is based on the following Technical Criteria
* CloudReady - focus on seamless portability
* CloudReady - focus on on-demand scalability
* CloudReady - focus on inter-component airtightness
* CloudReady - focus on inter-component and inter-service communication efficiency
* CloudReady - focus on security

The Technical Criteria have been populated with Quality Rules with aggregate weight greater or equal to 5 of the following existing Technical Criteria:
* Architecture - OS and Platform Independence
* Efficiency - Expensive Calls in Loops
* Efficiency - Memory, Network and Disk Space Management
* Efficiency - SQL and Data Handling Performance 
* Complexity - SQL Queries
* Secure Coding - API Abuse
* Secure Coding - Input Validation
* Secure Coding - Time and State

# In what situation should you install this extension?
If you are interested in getting a preview of what the CloudReady index would be and are willing to share the results to help the CAST Research Labs validate them.

# Release notes
## 1.1.0
Release 1.1.0 changes the composition of the index to integrating feedback from early try outs, and includes specific AAD-AED portal WAR to support full investigation in 8.1
## 2.0.0
Release 2.0.0 changes the organization and composition of the index, via dedicated Technical Criteria, to better map the type of issues at hand, and refine selection.

# _com.castsoftware.labs.cloud_ technology support
All technologies supported out-of-the-box by CAST AIP are supported.
In case of technologies supported by some AIP extensions, contact the Research Labs to build a compatible CloudReady index.

# Function Point, Quality and Sizing support
This extension is designed to bring new quality indicator aside existing ones.

# CAST AIP compatibility

This extension is compatible with:
* 8.1.x out-of-the-box (AIP release used for the tests)
* 8.0.x after changing the nuspec file (there is no reason the extension would not work but it was not tested)
* 7.x.x after changing the nuspec file (there is no reason the extension would not work but it was not tested)

# Supported DBMS servers
This extension is currently supported on CAST databases installed on any supported RDBMS.


# Prerequisites
* An installation of any compatible release of CAST AIP (see table above)


# Bug Fix List
N/A

# Download and installation instructions

Please see:  [Extension Link Installation](http://doc.castsoftware.com/display/DOCEXT/Extension+download+and+installation)

The installation steps are the following:
* download the extension through the CAST Extension Downloader
* open Server Manager 8.1+
* select the existing set of databases to update / install a new set of databases
* manage extensions of the existing set of database / follow the installation wizard up to the manage extension pane
* select _com.castsoftware.labs.cloud.2.0.0_
* run the update / the installation  
* open CAST Management Studio
* import the Assessment Model from the Dashboard Service processed in steps #3 to #6 above; this is a *Mandatory* step to start computing the new indicator, one MUST import and use the Assessment Model from the Dashboard that was updated with the extension
* deploy the WAR file from the WAR subdirectory
* configure the context.xml to target the Measurement Base you will use as well as the Dashboard Service processed in steps #3 to #6 above (to configure your own deployed WAR, contact the Labs for detailed procedure)

# Packaging, delivering and analyzing your source code
Packaging, delivering and analyzing your source code is performed the same way as usual.

To get results:
* run a new snapshot (if not possible, contact the Research Labs for alternative procedure)

To avoid computing the CloudReady index for applications that are not candidate to moving to the cloud:
* open CAST Management Studio
* edit the Dashboard Service(s) you are publishing the Snapshots of the N/A application(s)
* select the Assessment Model tab
* create an exclusion for the CloudReady index and the N/A application(s)

# What results can you expect?

## Objects
N/A

## Links
N/A

## Quality rules
N/A

## Technical Criteria
List of new Technical Criteria
* CloudReady - focus on seamless portability
* CloudReady - focus on on-demand scalability
* CloudReady - focus on inter-component airtightness
* CloudReady - focus on inter-component and inter-service communication efficiency
* CloudReady - focus on security

## Business Criteria
List of new Business Criteria
* CloudReady index

# Limitations
N/A
