# Job Scheduler

Job Scheduler is a Python-based console application that uses a Binary Search Tree (BST) data structure to manage and schedule tasks or jobs.

## Overview

This project contains a Job Scheduler system that ensures no overlapping jobs are scheduled. It allows users to add, remove, or view scheduled jobs via a user-friendly command-line interface. Jobs are persistently stored in a "data.txt" file.

The two primary components of this project are:

1. `bst_demo.py`: This file defines a Node class for individual tasks and a BSTDemo class for the job schedule tree. Each node contains the job's scheduled start time, duration, end time, and name.

2. `job_scheduler.py`: This file provides a user interface for the Job Scheduler system. It reads from and writes to the "data.txt" file, storing jobs persistently.

## Features

- Efficiently manages the jobs using a Binary Search Tree (BST).
- Allows the user to view the current schedule of jobs.
- Facilitates the addition of new jobs, checking for possible overlap with existing ones.
- Provides functionality to remove jobs from the schedule.
- Persists the job data in a .txt file.

## Getting Started

To start using this project, perform the following tasks:

1. Clone the repository: `git clone https://github.com/Rahul2K20/Python-Job-Scheduler.git`.
2. Navigate to the project directory: `cd Python-Job-Scheduler`.
3. Run the `job_scheduler.py` script to start the application: `python job_scheduler.py`.

## Usage

Upon running `job_scheduler.py`, you will be presented with a menu of four options:

1. View Today's Scheduled Jobs: This will display the list of jobs scheduled for the day.
2. Add a Job to Today's Schedule: You can add a job by providing the start time, duration, and job name.
3. Remove a Job from the Schedule: You can remove a job by providing the start time, duration, and job name.
4. Quit: This will exit the application.

## License

This project is licensed under the MIT License.
