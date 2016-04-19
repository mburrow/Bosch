

#Redis

Created by [mjb](mailto:mike.burrow@emc.com "send email") on 19 Apr 2016.
Last modified by [mjb](mailto:mike.burrow@emc.com  "send email") on 19 Apr 2016

> **Note:** Some of the information listed below will not be applicable for every service!

##Service Information

Item|Value
:----|-----
Service category|Data Management|
Service name|-|
Service short name|Cache-Redis|
Service version|1|
Service provider|CI/PJ-IoT|
Service owner|[Ottenwaelder Beate (CI/PJ-IoT-C)](https://inside-docupedia.bosch.com/confluence/display/%7EOTB8FE)
Technical team|-|
Consulting|-|
BICS contact person|[Ottenwaelder Beate (CI/PJ-IoT-C)](https://inside-docupedia.bosch.com/confluence/display/%7EOTB8FE) & [Enderes Philipp (CI/PJ-IoT-C)](https://inside-docupedia.bosch.com/confluence/display/%7EENP1FE).|
Release date|E07/2015|
State|-|
SLA|A=99,0%|

##Service Details
###Description
[Redis](http://www.redis.io) is an in-memory key-value store. The key Redis service features:
 
+ Based on Redis OSS 3.0
+ Data persistence
+ Shared development plan available 
+ Dedicated production plan available

Item     | Value
:-------- | -----
Service components|
Service eligibility|RB internal|
Service dependencies|None|
Service accessibility|-|
Recommended client components|-|
Protocols provided|-|
Language support provided|-|
EAM domain classification|-|
Not included in service scope|High-availability & Auto-scaling.|
Obligations of service recipient|TBD|

##Service Plans

Item | Bronze|Silver|
:-------- | :------|:----|
Description|**_Shared development plan:_** Provision a Redis process on a shared VM.|**_Dedicated production plan:_** Provision dedicated VM which is configured with a Redis process ready to be used.|
Capacity|Cache size: ~ 1 GB (Shared).|Cache size: ~ 2 GB.|
Pricing|-|-|
Availability|tbd|**_Current:_** 99%, excluding announced maintenance windows. **_Target:_** 07/2016: 99.5%, excluding announced maintenance windows.
Reliability|-|-|
Performance|-|-|
Security|-|-|
Elasticity|-|-|
Retention period|-|-|
Manageability|-|-|
Monitoring|The subscriber will be able to use the [MONITOR](http://redis.io/commands/monitor) command; a debugging command that streams back every command processed by the Redis process.|The subscriber will be able to use the [MONITOR](http://redis.io/commands/monitor) command; a debugging command that streams back every command processed by the Redis process.|
Logging|The subscriber will be able to use the [MONITOR](http://redis.io/commands/monitor) command; a debugging command that streams back every command processed by the Redis process.|The subscriber will be able to use the [MONITOR](http://redis.io/commands/monitor) command; a debugging command that streams back every command processed by the Redis process.|
Reporting|-|-|
Backup and disaster recovery|None|None|
Patch management|-|-|
Tenancy mode|Isolation at process level.|Isolation at VM level.|
High Availability|The service does not guarantee H/A; however, data availability is drastically increased by [persisting](http://redis.io/topics/persistence) cached data using RDB and AOF.|The service does not guarantee H/A; however, data availability is drastically increased by [persisting](http://redis.io/topics/persistence) cached data using RDB and AOF.|
Roles and authorisation|-|-|

##Service Support

Plan/Item | Bronze & Silver|
:--------- | :----------|
Incident management|1st Level support by BICS platform support [Incident management](https://inside-docupedia.bosch.com/confluence/display/BICI/Incident+management). See [BICS Support](https://inside-docupedia.bosch.com/confluence/x/nmFWF).
Incident response time|BICS Support - [Solution Time (KPIs)](https://inside-docupedia.bosch.com/confluence/display/BICI/BICS+Support#BICSSupport-SolutionTime%28KPIs%29).
Incident escalation stages|BICS Support - [Escalation Concept](https://inside-docupedia.bosch.com/confluence/display/BICI/BICS+Support#BICSSupport-EscalationConcept).
Service disaster recovery – single failure|-|
Service disaster recovery – full data restore|-|
Maintenance windows|-|

##Miscellaneous Information

Item     | Value
-------- | -----
General security compliance|
List of regulatory compliances|
Internal service ID|

##How To Order

##Service Provisioning

##Service Usage

###Introduction to the Service

The [Redis service](http://pivotal.io/platform/datasheet/redis-for-pivotal-cloud-foundry) allows stateless applications to maintain and share data (e.g. state) between several application instances. 

The Redis service is based on [Redis for Pivotal Cloud Foundry](http://docs.pivotal.io/redis/index.html). The package supports [two basic service plans](http://docs.pivotal.io/redis/overview.html): a shared developer plan and a dedicated production plan.  

+ On provisioning the shared service plan, the Redis service winds up a Redis process on the shared VM. 

+ On provisioning the dedicated service plan, the Redis service supplies a dedicated VM which is configured with a Redis process ready to be used.  


###API / Web Service Documentation

On binding, the service supplies relevant connection information. This connection information includes the dedicated VM's IP, the port on which the Redis process is listening, and a password to authenticate an application against the Redis process.

Procedures describing how to [bind](http://docs.pivotal.io/redis/using.html#bind) a Redis service instance

###User documentation

Redis can be used both via Pivotal Apps Manager and the CLI, both methods are outlined [here](http://docs.pivotal.io/redis/using.html)

Instructions on how to use Spring Data Redis, part of the larger Spring Data family which provides easy configuration and access to Redis from Spring applications can be found [here](http://projects.spring.io/spring-data-redis).

The official Redis Documentation can be found [here](http://redis.io/documentation).

####Example

An example application has also been created to help application developers get started with Redis for PCF, and can be downloaded [here](https://github.com/pivotal-cf/cf-redis-example-app/archive/master.zip)

###Class documentation

###Release Notes

Here are the [pivotal release notes](http://docs.pivotal.io/redis/release.html).

##Future Outlook

Here are [design drafts](http://redis.io/topics/rdd) of new Redis proposals.
A report of the Redis Dev Day London 2015 can be found [here](https://fnordig.de/2015/10/22/redis-dev-day-london-2015/).

##User Reviews and Feedback

> Written with [StackEdit](https://stackedit.io/).
