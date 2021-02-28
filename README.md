# Python-Job-Scheduler


**Introduction**

•	A company, XYZ financial services, has a list of daily operation processing jobs (background jobs) which run their business operations.

•	Jobs that load prices, transactions, validate incoming transactions, end of day reports etc.

•	They require a job scheduling program which maintains the scheduling of these daily jobs. They also need the program to be dynamic, new jobs can be scheduled and scheduled jobs can be removed from the schedule during the day.

**Specification**

•	There are a basic number of jobs that are input to the program when it starts, these jobs are added to a 'load file' the night before. The program needs to be able to load these jobs and create a starter schedule from this load file when it starts.

•	The program needs to be dynamic - jobs can be scheduled or removed during the day. The program needs to have an interface through which new jobs can be added to the schedule and existing jobs can be removed, without changing the order of the remaining jobs already scheduled.

•	Jobs can only run one at a time. There cannot be any overlap during the duration of a job. The scheduling program needs to be able to test for this while jobs are being scheduled, both dynamically and from the load file.

•	The load file needs to be dynamically updated as jobs are being added or removed in the scheduling program. This is necessary to ensure that the modified daily schedule (due to add/remove transactions) are not lost when the user exits the program.

**Proposed solution**

•	Based on the specs, the Binary search Tree structure fits these specifications perfectly.

•	The key for our nodes will be time. Since time is continuous and we can only have one job run at a given time, the BST will not allow for duplicate jobs and be easy to determine the scheduling.

•	Scheduling can happen at any time for later times in the day, so the order in which jobs are scheduled (insertions) will be random, but based on the BST structure we'll always be able to get a sorted view of our data based on the ordering of nodes that a BST allows to maintain.

•	We can traverse the BST easy using in-order traversal to get a sorted view of our daily scheduled jobs.

•	We can easily add restrictions on the insertion of jobs to the schedule to account for no overlap.

•	Insertion, removal and other operations like number of jobs, finding a specific job (not a requirement at this time) are very fast in a BST.
