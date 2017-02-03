---
title: Syllabus
layout: main
---

## Lecture and section information
----------------------------------------------------------------------------------------

CS 2043, Spring 2017

Lecture time: MWF 11:15am - 12:05pm

Location location: Gates G01

## Staff and office hours
----------------------------------------------------------------------------------------

#### Lecturer: Stephen McDowell

- Thursday: 6:00pm - 7:00pm, Gates G11
- Friday: 2:00pm - 3:00pm, Gates G19

> #### Notice
> Do not, under any circumstances, e-mail any of the TAs directly.  All questions /
> queries for help should be done in person during office hours, or on the course
> Piazza.  If there is something urgent going on, you should e-mail me directly.

#### TA: Joe Caparelli

- Monday: 1:00pm - 2:00pm, Gates G15
- Thursday: 5:00pm - 6:00pm, Gates G19

#### TA: Trevor Edwards

- Monday: 3:00pm - 4:00pm, Gates G17
- Wednesday: 3:00pm - 4:00pm, Gates G19
- Friday: 3:00pm - 4:00pm, Gates G19

#### TA: Jakob Glueck

- Tuesday: 3:00pm - 4:00pm, Gates G17
- Friday: 1:00pm - 2:00pm, Gates G19

#### TA: Matt Lombana

- Monday: 2:00pm - 3:00pm, Gates G17
- Wednesday: 2:00pm - 3:00pm, Gates G19

#### TA: Joe Marino

- Tuesday: 11:30am - 12:30pm, Gates G19
- Thursday: 4:00pm - 5:00pm, Gates G19

<iframe src="https://calendar.google.com/calendar/embed?mode=WEEK&amp;height=600&amp;wkst=1&amp;bgcolor=%23cccccc&amp;src=cornell.edu_6lkr0dr01n7vhdju0f915aeeis%40group.calendar.google.com&amp;color=%237A367A&amp;ctz=America%2FNew_York" style="border-width:0" width="800" height="600" frameborder="0" scrolling="no"></iframe>

## Catalog description
----------------------------------------------------------------------------------------

2 credits.  S/U Only. UNIX and UNIX-like systems are increasingly being used
on personal computers, mobile phones, web servers, and many other systems.
They represent a wonderful family of programming environments useful both to
computer scientists and to people in many other fields, such as computational
biology and computational linguistics, in which data is naturally represented
by strings.  This course takes students from shell basics and piping, to
regular-expression processing tools, to shell scripting and Python.  Other
topics to be covered include handling concurrent and remote resources,
manipulating streams and files, and managing software installations.

## Prerequisites
----------------------------------------------------------------------------------------

One programming course or equivalent programming experience.  No previous
knowledge of UNIX or expertise in any particular language is assumed.

## Texts
----------------------------------------------------------------------------------------

None required, but I may add some external references on the
[Readings page]({{ site.baseurl }}{% link readings.md %}).

## Course technologies
----------------------------------------------------------------------------------------

- We will be working together on some selected programming / shell exercises
  in class, and you are *encouraged* to bring a laptop (or tablet) to fully
  participate.
- You will need a Unix development environment (native install, or Virtual Machine).
- Please refer to the [Getting Started]({{ site.baseurl }}{% link getting_started.md %})
  page for more information.

## Class material
----------------------------------------------------------------------------------------

Class material will be posted on GitHub, including the assignments, lecture slides,
and lecture demos.

Student work will also be posted on Cornell's Enterprise GitHub in private repositories
(don't worry, we will discuss how these work in class).  I will setup your repositories
for you.

## Course work
----------------------------------------------------------------------------------------

### In-class work

It is in your best interest to attend lecture so you can participate in the demos.
The purpose of the demos is to solidify what we have covered, in a "learning-by-doing"
scenario.  None of this will be graded or tracked in any way, and is strictly for
practice.

### Assignments

There will be around 5 assignments in all.  All assignments will be done individually.

On weeks when an assignment is due, it will be due at **5pm EST on Friday**.
These deadlines are be posted on the
[Schedule]({{ site.baseurl }}{% link schedule.md %}) page.  This time was chosen to
hopefully make your life easier; you are taking other classes and the majority should
have non-conflicting deadlines with this time.

#### Submissions

You will be submitting all of your work through GitHub.  This will be explained
in gory detail during lecture, but effectively all you need to do is make sure
that you have pushed your submission to your private repository **on the master
branch** by the deadline and it is submitted.  Don't worry if you are unfamiliar
with what this means, you will be shortly.

#### Feedback and Grade Postings

We will be providing you with feedback on the [Cornell University Course Management
System (CMS)][CMS].  We will grade your work as soon as reasonably possible, but
you are encouraged to setup notifications on CMS so that you get an e-mail with
when grades are released.  Inside the purple navbar on the left after you have
clicked on "CS 2043", click on the "Notifications" section.  Check the

- ...grades for an assignment are released.

box and click "Update" at the bottom to receive an e-mail when grades for an
assignment are released.

[CMS]: http://cms.csuglab.cornell.edu/

### Grading

Each assignment will be worth 10 points.  Your final grade will be determined by
a weighted average of all your scores.  I will not be releasing what this weighting
scheme is, so please do not ask for it.  The most I will say is that this is an
S/U class, so if you had to label it 6 and above are S and 5 and below are U.

Were I to release an official weighting policy, I would be required to follow it.
Ambiguity in this regard really does serve you best.

## Course policies
----------------------------------------------------------------------------------------

### Late work policy

As stated previously, assignments will be due by 5pm on Friday.  This is a hard
deadline.  However, life happens.  If you happen to need extra time, this is how it
will work:

<div class="table-responsive">
  <table class="table table-striped">
    <colgroup>
      <col class="col-xs-2">
      <col class="col-xs-2">
      <col class="col-xs-2">
    </colgroup>
    <thead>
      <tr>
        <th>Submission Day</th>
        <th>Submission Time</th>
        <th>Late Penalty</th>        
      </tr>
    </thead>
    <tr>
      <td>Friday</td>
      <td>5:01pm -- 11:59pm</td>
      <td><code>0.001</code> points</td>
    </tr>
    <tr>
      <td>Saturday</td>
      <td>12:01am -- 5:00pm</td>
      <td><code>1</code> point</td>
    </tr>
    <tr>
      <td>Sunday</td>
      <td>5:01pm -- 5:00pm</td>
      <td><code>2</code> points</td>
    </tr>
    <tr>
      <td>Monday</td>
      <td>5:01pm -- 5:00pm</td>
      <td><code>3</code> points</td>
    </tr>
  </table>
</div>

In words, you lose 1 point per 24hr period it is late with a quasi-grace period on
Friday evening.  No submissions will be accepted after 5pm on Monday.

### Collaboration

An assignment is an academic document, like a journal article.
When you turn it in, you are claiming everything in it is your
original work, *unless you cite a source for it*.

As part of the process of learning development skills, you should
attempt to develop and debug code for yourself.  You are welome to discuss the
assignments with other students *at a high level*, but you are forbidden -- under
any circumstances -- to be in the posession of another students' code.  This includes,
but is not limited to, looking at their code, copying their code, stealing their computer,
hacking the servers...

### Academic integrity

The assignments are there to teach you, and I assume you are interested in learning the
material by being enrolled in the course.  Cheating will teach you nothing, and can only
stand to hurt you.

We expect academic integrity from everyone.  School is stressful, and you may feel pressure
from your coursework or other factors, but that is no reason for dishonesty!  If you feel you
can't complete the work on the own, come talk to the professor, the TA, or your advisor, and
we can help you figure out what to do.

For more information, see Cornell's
[Code of Academic Integrity](http://cuinfo.cornell.edu/aic.cfm).

### Emergency procedures

In the event of a major campus emergency, course requirements, deadlines, and
grading percentages are subject to changes that may be necessitated by a
revised semester calendar or other circumstances.  Any such announcements will
be posted to [the course home page]({{ site.baseurl }}{% link index.md %}).

