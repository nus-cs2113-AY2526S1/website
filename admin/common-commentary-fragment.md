{% from "common/topics.njk" import panopto, slugify, topic_followup, topic_preamble with context %}
{% from "common/macros.njk" import embed_topic with context %}
<!-- ==================================================================================================== -->
                                         Software Engineering
<!-- ==================================================================================================== -->
<div id="{{ slugify("SE: Intro") }}">

Given this is a first course in SE, tradition demands that we start by defining the subject. However, let's not spend a lot of time going through lengthy/formal definitions of SE. Instead, let's look at an extract from the very first chapter of a very famous SE book, with the aim of providing some inspiration, but also an appreciation of the challenges ahead.
</div>
<!-- ==================================================================================================== -->
                                             Requirements
<!-- ==================================================================================================== -->
<div id="{{ slugify("Specifying Requirements [quick peek ahead]") }}">

This week, you will be dealing with the _requirements_ aspect of the tP. While there isn't time in this week to learn that topic fully, let's learn a couple the techniques you'll be using to deal with requirements of your tP this week: _user stories_ and _feature lists_.
</div>
<!-- ------------------------------------------------------------------------------------------------------ -->
<div id="{{ slugify("Requirements: Intro") }}">
<div tags="m--cs2103 m--cs2113">

Last week, we had a quick peek at the _requirements_ aspect. Let's study the topic properly this week, starting with an introduction to the topic.
</div>
<div tags="m--tic2002">

Let's learn about the _requirements_ aspect of SE projects. Although you have already started your course project (which didn't require heavy work on the requirements aspect), it is good to learn more about this topic, so that you can use it in future projects.
</div>
</div>
<!-- ------------------------------------------------------------------------------------------------------ -->
<div id="{{ slugify("Requirements: Gathering") }}">

Next, a quick look at techniques used for _gathering_ requirements. They are mostly common-sense but let's go through them for completeness' sake anyway.
</div>
<!-- ------------------------------------------------------------------------------------------------------ -->
<div id="{{ slugify("Requirements: Specifying") }}">
<div id="{{ slugify("Requirements: Specifying [continued from last week]") }}">

As you may have noticed in the section about prototyping, some techniques can be used for both gathering and specifying requirements. The two things often go hand-in-hand any way. For example, you gather some requirements, specify them in some form, and show them to stakeholders to get feedback.

Now, let's look at other techniques used for specifying requirements.<span tags="m--cs2113">Of course, you've seen two of them already.</span>
</div>
</div>
<!-- ------------------------------------------------------------------------------------------------------ -->
<div id="{{ slugify("specifyingRequirements-useCases-introduction") }}">

The technique of _use cases_ (don't confuse with _user stories_) covered below is another widely used technique. However, we only cover it briefly (i.e., you'll learn _what_ it is but not _how_ to use it) to lower to course workload.
</div>
<!-- ------------------------------------------------------------------------------------------------------ -->
<div id="{{ slugify("Requirements: Use Cases") }}">

Previously, you learned a number of techniques for specifying requirements. There's one more left, which we'll cover this week.
</div>
<!-- ------------------------------------------------------------------------------------------------------ -->
<div id="{{ slugify("followup Requirements: Use Cases") }}">

Now that you know all the different ways of specifying requirements, **here is an example that shows how all techniques of specifying requirements can work together**:
{{ panopto("a8d7db29-d50c-4e8c-8742-ac4400ee8366", desc="Example: TeamFormer") }}
</div>
<!-- ==================================================================================================== -->
                                             OOP
<!-- ==================================================================================================== -->
<div id="{{ slugify("OOP: Intro") }}">
<div id="{{ slugify("OOP: Classes and Objects") }}">

As you know, OOP is a core part of this course. Let's start learning the OOP paradigm this week.
</div>
</div>
<!-- ------------------------------------------------------------------------------------------------------ -->
<div id="{{ slugify("oop-objects-abstraction") }}">

**OOP is built upon four core concepts.** The firs two are:
1. _abstraction_
1. _encapsulation_
1. ...
1. ...

They are explained in the sections below.
</div>
<!-- ------------------------------------------------------------------------------------------------------ -->
<div id="{{ slugify("OOP, Java: Class-Level Members") }}">

You learned that objects can have members (methods, attributes). Well, there is something called _class-level_ members too. Let's learn what they are, how they differ from the former, and how to implement them in Java.
</div>
<!-- ------------------------------------------------------------------------------------------------------ -->
<div id="{{ slugify("Java: Useful Classes") }}">

While you _can_ (and will be) defining your own classes, Java comes with a whole bunch of built-in classes that you can use right-away. Let's learn about some of the most useful such built-in classes next.
</div>
<!-- ------------------------------------------------------------------------------------------------------ -->
<div id="{{ slugify("OOP + Java: Inheritance") }}">

Now that you know the basics about classes and objects, let's move to the next level. The sections below explain the third core concept of OOP (called _inheritance_) and how to use that in Java.
1. abstraction  {{ icon_tick }}
1. encapsulation  {{ icon_tick }}
1. **_inheritance_**
1. ...
</div>
<!-- ------------------------------------------------------------------------------------------------------ -->
<div id="{{ slugify("OOP + Java: Polymorphism") }}">

Inheritance is even more powerful when combined with _polymorphism_ (which also happens to be the fourth core concept of OOP), explained in the sections below.
1. abstraction {{ icon_tick }}
1. encapsulation {{ icon_tick }}
1. inheritance {{ icon_tick }}
1. **_polymorphism_**
</div>
<!-- ------------------------------------------------------------------------------------------------------ -->
<div id="{{ slugify("OOP + Java: Enumerations") }}">

An _enumeration_ is something in between a primitive (e.g., `int`) and a class (e.g., `Person`). Let's learn about enumerations next.
</div>
<!-- ------------------------------------------------------------------------------------------------------ -->
<div id="{{ slugify("OOP + Java: Abstract Classes") }}">

It is time to move on to some intermediate level OOP concepts. Next, let's learn about _abstract classes_ and how they are implemented in Java.
</div>
<!-- ------------------------------------------------------------------------------------------------------ -->
<div id="{{ slugify("OOP + Java: Interfaces") }}">

From abstract classes, we move to another related OOP concept _interfaces_, and how they are implemented in Java.
</div>
<!-- ==================================================================================================== -->
                                             C++ to Java
<!-- ==================================================================================================== -->
<div id="{{ slugify("Java: Intro") }}">

Next, let's get started learning Java. First, a bit about the language itself.
</div>
<!-- ------------------------------------------------------------------------------------------------------ -->
<div id="{{ slugify("cppToJava-javaWorld-how") }}">

Note that this topic (and many other topics) come with a pre-recorded lecture video.

{{ embed_topic("textbooks.md#tip-about-lecture-videos", "Admin " + icon_embedding + " Lectures → Extract", "3", status="expanded") }}
<p/>

</div>

<!-- ------------------------------------------------------------------------------------------------------ -->
<div id="{{ slugify("Java: HelloWorld") }}">

As with any language, the first step is to install the language on your computer. After that, you write a simple HelloWorld program, and get it running.

Java 17 can be downloaded from [here](https://www.oracle.com/java/technologies/downloads/#java17).

</div>
<!-- ------------------------------------------------------------------------------------------------------ -->
<div id="{{ slugify("Java: Data Types") }}">

Now that you know how to write the simplest of Java programs, you can move onto learning about basic language concepts, starting with data types.

At the end of the next section, there is an exercise (_[Key Exercise] ByeWorld_) that you need to submit on Coursemology. From this point onwards, programming exercises marked as <span class="bg-dark text-white p-1">[Key Exercise]</span> need to be submitted on Coursemology.

{{ embed_topic("index-tic2002-fragment.md#coursemology-info", "Admin " + icon_embedding + " Tools → Coursemology", "3") }}
<p/>
</div>
<!-- ------------------------------------------------------------------------------------------------------ -->
<div id="{{ slugify("Java: Control Flow") }}">

Next up is learning how to control the flow of a Java program.
</div>
<!-- ------------------------------------------------------------------------------------------------------ -->
<div id="{{ slugify("Java: Objects") }}">

Now that you know what _objects_ are, let's see how they are used in Java, which happens to be an OOP language.
</div>
<!-- ------------------------------------------------------------------------------------------------------ -->
<div id="{{ slugify("Java: Classes") }}">

Having seen how to use objects in Java, the next step is learn how to define new _kinds_ of objects (aka _classes_) in Java.
</div>
<!-- ------------------------------------------------------------------------------------------------------ -->
<div id="{{ slugify("OOP: Class-level members") }}">

Now that we know about classes, let's learn what _class-level members_ are and how to use them in Java.
</div>
<!-- ------------------------------------------------------------------------------------------------------ -->
<div id="{{ slugify("Java: Constants") }}">

You already know how to define variables in Java code; do you know how to define constants?
</div>
<!-- ------------------------------------------------------------------------------------------------------ -->
<div id="{{ slugify("Java: Casting") }}">

As you have learned the Java basic topics already, it is time to move to intermediate level topics. This week, we cover several such topics, starting with the one given below.
</div>
<!-- ------------------------------------------------------------------------------------------------------ -->
<div id="{{ slugify("Java: Packages") }}">

As you add more and more Java classes to your project, keeping all those classes in the same directory becomes untenable. The solution is covered in the next topic.
</div>
<!-- ------------------------------------------------------------------------------------------------------ -->
<div id="{{ slugify("Java: JavaDocs") }}">

As you know, adding comments to the code is a good practice. Let's learn about a specific type of comments that you can use in Java code that can do even more than just explain the code.
</div>
<!-- ------------------------------------------------------------------------------------------------------ -->
<div id="{{ slugify("Java: Access Modifiers") }}">

As the size of your Java codebase grows, every class being able to access every member of every other class can be problematic. Hence, there should be a way to control the access to our Java classes and their members. The solution is given in the topic below.
</div>
<!-- ------------------------------------------------------------------------------------------------------ -->
<div id="{{ slugify("Java: Generics") }}">

As usual, we cover a few more Java topics that are relevant to the iP this week. We start with topics related to data structures that you can use to work with collections of objects, as you'll need to be able to manage a collection of task objects in your iP.

But first, let's learn a programming technique called _generics_ (similar to C++ _templates_) often used in such data structures.
</div>
<!-- ------------------------------------------------------------------------------------------------------ -->
<div id="{{ slugify("Java: Collections") }}">

Next, we learn about some built-in data structures that can be used to manage a collection of objects.
</div>
<!-- ------------------------------------------------------------------------------------------------------ -->
<div id="{{ slugify("Java: File Access") }}">

Another thing you need to do in your project soon is reading from and writing to files. Let's learn how to do that next.
</div>
<!-- ------------------------------------------------------------------------------------------------------ -->
<div id="{{ slugify("Java: JAR files") }}">

At some point, you want to package your code as a single executable file. The next topic covers how to do that.
</div>
<!-- ------------------------------------------------------------------------------------------------------ -->
<div id="{{ slugify("Java: Varargs") }}">

While the next few topics are optional, we recommend that you ==have a quick look anyway==, just so that you know their existence at least.
</div>
<!-- ------------------------------------------------------------------------------------------------------ -->
<div id="{{ slugify("Java: JavaFX") }}">

**JavaFX is not required for this course**<span tags="m--cs2113"> as we strongly discourage you from creating a GUI app</span>. If you are still interest to learn JavaFX, given below is a link to some tutorials.
</div>
<!-- ------------------------------------------------------------------------------------------------------ -->
<div id="{{ slugify("Java: Streams") }}">

**Streams is an advanced Java feature** not required for this course. If you are still interest to learn it, some resources are given below.
</div>
<!-- ------------------------------------------------------------------------------------------------------ -->
<div id="{{ slugify("cppToJava-junit-basic") }}">

**Now, let us learn about JUnit, a tool used for automated testing.** JUnit is a third-party tool (not included in the JDK). <span tags="m--cs2103 m--cs2113">but your tP project is already configured to use JUnit, with the help of Gradle. That means the video tutorial given at the end of the section is mostly not applicable to you, unless you are interested to learn how to set up a non-Gradle project for JUnit.</span>
</div>
<!-- ------------------------------------------------------------------------------------------------------ -->
<div id="{{ slugify("cppToJava-junit-intermediate") }}">

While the JUnit concepts mentioned in the topic below are not strictly needed for the course projects, it is good to be aware of them so that you try some of them when applicable.
</div>
<!-- ==================================================================================================== -->
                                           Revision Control
<!-- ==================================================================================================== -->
<div id="rcs-intro">
<div tags="m--cs2103">

This week, you are starting your individual project (iP). As you are adding code to the iP in rapid succession, you'll need a way to keep track of all the changes you do. The tool we are going to use for that is called Git, and we need to learn Git basics pretty quickly.

Let's jump in and learn how to get started using Git in your own computer.
</div>
<div tags="m--cs2113">

:thinking: In case you are puzzled by the sudden change of topic, it's because we take an iterative approach to covering topics, as explained in the panel below:

{{ embed_topic("courseOverview.md#meaning-of-iterative-topics", "Admin " + icon_embedding + " Course Overview → Extract", "3") }}
<p/></div>
<div tags="m--tic2002">

You are going to start your project pretty soon. As you are adding feature increments to your project, you'll need a way to keep track of all those changes too. The tool we are going to use for that is called Git.

Let's jump in and learn how to get started using Git in your own computer.

<p/></div>
</div>
<!-- ------------------------------------------------------------------------------------------------------ -->
<div id="{{ slugify("gitAndGithub-init") }}">

Now that we know what RCS is in general, we can try to practice it ourselves using a specific tool i.e., Git.

The following section gives a specific scenario that includes the steps of initializing a Git repository.

**If you are new to Git**, you are highly recommended to ==follow those steps in your own computer== to get some hands-on practice as you learn Git usage.

<div tags="m--cs2103">

Note that this topic (and many other topics) come with a pre-recorded video.

{{ embed_topic("textbooks.md#tip-about-lecture-videos", "Admin " + icon_embedding + " Textbooks → Extract", "3", status="expanded") }}
<p/>

</div>
</div>
<!-- ------------------------------------------------------------------------------------------------------ -->
<div id="rcs-remote-repos">

Having learned how to use Git in your own computer, let's also learn a bit about working with remote repositories too. <span tags="m--cs2103 m--cs2113">While it seems like a bit 'too much' to take in one week, but we want you to start using Git in your iP (individual project) from the very beginning.</span>
</div>
<!-- ------------------------------------------------------------------------------------------------------ -->
<div id="{{ slugify("RCS: Using History") }}">

Previously, you learned how to _save_ revision history in your local repository, in the form of _commits_. Next, let us use how to make use of that history.
</div>
<!-- ------------------------------------------------------------------------------------------------------ -->
<div id="{{ slugify("RCS: Pull, Push") }}">

Last week, you learned how to fork and clone a remote repository. Let's now learn how to transfer revision history date to and from a remote repository.
</div>
<!-- ------------------------------------------------------------------------------------------------------ -->
<div id="{{ slugify("RCS: Creating Pull Requests") }}">

Let's learn how to create a pull request (PRs) on GitHub; you need to create one for your project this week.

<div tags="m--cs2113">

Follow that with learning how to review PRs as you'll be doing that too later in this week.
</div>
</div>
<!-- ------------------------------------------------------------------------------------------------------ -->
<div id="{{ slugify("RCS: Merging PRs") }}">

Let's learn how to merge a PR on GitHub; you need to do that in the tP later, and you'll be practicing PR merging in the iP this week.

</div>
<!-- ------------------------------------------------------------------------------------------------------ -->
<div id="{{ slugify("RCS: Branching") }}">

Let's learn about a few more Git techniques, starting with branching. Although these techniques are not really needed for the iP, we require you to use them in the iP so that you have more time to practice them before they are really needed in the tP.
</div>
<!-- ------------------------------------------------------------------------------------------------------ -->
<div id="{{ slugify("RCS: Merge Conflicts") }}">

When working with Git, sooner or later you will face a problem called _merge conflict_. Let's learn how to deal with them.
</div>
<!-- ------------------------------------------------------------------------------------------------------ -->
<div id="{{ slugify("RCS: Workflows") }}">

**Next, you will learn a workflow called the 'Forking Flow'**, which combines the various Git and GitHub techniques you have been learning over the past few weeks. It is also the workflow you will use in the tP.
</div>
<!-- ------------------------------------------------------------------------------------------------------ -->
<div id="{{ slugify("gitAndGithub-forkingWorkflow") }}">

==The activity in the section below can be skipped== as you will be doing a similar activity in a coming tutorial.
</div>
<!-- ------------------------------------------------------------------------------------------------------ -->
<div id="{{ slugify("gitAndGithub-drcsVsCrcs") }}">

**Git is considered a DRCS**. Read the topic below to learn what that means and how it differs from the alternative.
</div>
<!-- ------------------------------------------------------------------------------------------------------ -->
<div id="{{ slugify("gitAndGithub-featureBranchFlow") }}">

**These are two workflows that are riskier (but simpler) than the forking flow**. After following the forking flow for a while, you may switch to one of these, but at your own risk.
</div>
<!-- ==================================================================================================== -->
                                     Implementation
<!-- ==================================================================================================== -->
<div id="{{ slugify("Reuse") }}">

Do you know the difference between a _library_ and a _framework_?

Programmers often reuse code in various ways. The next few topics aim to clarify the difference between several forms reusable software comes in.
</div>
<!-- ------------------------------------------------------------------------------------------------------ -->
<div id="{{ slugify("Cloud Computing") }}">

While not examinable, the next few sections explain some basic cloud computing concepts that are relevant to software engineers.
</div>
<!-- ==================================================================================================== -->
                                     IDEs
<!-- ==================================================================================================== -->
<div id="{{ slugify("IDEs: Basic Features") }}">

As you are likely to be using an IDE for the {{ ip_name }}, let's learn at least enough about IDEs to get you started using one.

<div tags="m--cs2103">

:thinking: In case you are puzzled by the sudden change of topic, it's because we take an iterative approach to covering topics, as explained in the panel below:

{{ embed_topic("courseOverview.md#meaning-of-iterative-topics", "Admin " + icon_embedding + " Course Overview → Extract", "3") }}
<p/>
</div>
</div>
<!-- ------------------------------------------------------------------------------------------------------ -->
<div id="{{ slugify("IDEs: Intermediate Features") }}">

Now that you know how to use IDE basic features, it's worth looking at even more ways of leveraging their power. In particular, ==the _debugging_ feature can be indispensable== at times.
<p/>
</div>
<!-- ------------------------------------------------------------------------------------------------------ -->
<div id="{{ slugify("IDEs: Advanced Features") }}">

In case you are the type who want to become a 'power user' of IDEs (it's not a bad idea, given the IDE is like the primary tool of a software engineer), given below are some more things you can do with IDEs.
</div>
<!-- ==================================================================================================== -->
                                     Code Quality
<!-- ==================================================================================================== -->
<div id="{{ slugify("Code Quality: Guidelines") }}">

Next, let's learn about some guidelines that can apply to improve the quality of your code.
</div>
<!-- ------------------------------------------------------------------------------------------------------ -->
<div id="{{ slugify("Code Quality: Coding Standards") }}">

As you know, one of the objectives of the iP is to raise the quality of your code. We'll be learning about various ways to improve the code quality in the next few weeks, starting with coding standards.
</div>
<!-- ------------------------------------------------------------------------------------------------------ -->
<div id="{{ slugify("codeQuality-introduction-basic") }}">
<div tags="m--cs2103">

<box type="info" header="In-video quizzes" seamless>

The <span style="font-size: large;" class="badge rounded-pill bg-warning text-dark">Q+</span> icon indicates that the video has an in-video quiz. Submitting the in-video quiz can earn you bonus [participation marks]({{ baseUrl }}/admin/participation.html).<br>

In-video quizzes are in only a small number of pre-recorded videos that are more important than the rest. They are a very light way to engage you with the video a bit more than just passively watching.
</box>

==Please watch the video given below as it has some extra points not given in the text version.==
</div>
</div>
<!-- ------------------------------------------------------------------------------------------------------ -->
<div id="{{ slugify("Code Quality: Naming") }}">

Previously, you learned about coding standards as a way to improve code quality. The next topic along that theme covers guidelines for naming things in code.
</div>
<!-- ------------------------------------------------------------------------------------------------------ -->
<div id="{{ slugify("Code Quality: Readability") }}">

Continuing our theme on _code quality_, given below is another aspect of it: _readability_
</div>
<!-- ------------------------------------------------------------------------------------------------------ -->
<div id="{{ slugify("Code Quality: Refactoring") }}">

Knowing code-quality guidelines is useful for sure, but how do we improve the code quality of existing code in a systematic and safe way? That's where the next topic comes in.
</div>
<!-- ------------------------------------------------------------------------------------------------------ -->
<div id="{{ slugify("Code Quality: Refactoring (Revisited)") }}">

The topic of _refactoring_ was covered in an ealier week. We ==repeat the topic below for your convenience== as you'll need to refactor your code when applying the code quality guidelines given above.
</div>
<!-- ------------------------------------------------------------------------------------------------------ -->
<div id="{{ slugify("Code Quality: Unsafe Practices") }}">

Another step in our journey to improve code quality: Let's learn some legit but _unsafe_ practices we should avoid.
</div>
<!-- ------------------------------------------------------------------------------------------------------ -->
<div id="{{ slugify("Code Quality: Code Comments") }}">

**This is the final installment of the _code quality_ topics.** As you are learning about JavaDoc comments this week, you can also learn these guidelines to write better code comments.
</div>
<!-- ==================================================================================================== -->
                                    Error Handling
<!-- ==================================================================================================== -->
<div id="{{ slugify("Error Handling: Exceptions") }}">

So far, your iP may have assumed a 'perfect world' e.g., user input is always in the expected format. To make the product ready for the not-so-perfect real world, the code should be able to handle error conditions. Let's learn how to do that.
</div>
<!-- ------------------------------------------------------------------------------------------------------ -->
<div id="{{ slugify("Error Handling: Logging and Assertions") }}">

Previously, you learned how to use exceptions to handle errors. Here are two more techniques that can help with the error handling aspect of programming.
</div>
<!-- ------------------------------------------------------------------------------------------------------ -->
<div id="{{ slugify("Logging") }}">

Given next are **two techniques that help you locate problems in the code**: _logging_, and _assertions_
</div>
<!-- ------------------------------------------------------------------------------------------------------ -->
<div id="{{ slugify("Defensive Programming") }}">

You already know some techniques (e.g., exceptions, assertions) to make the code more resilient to errors. Given next is an overarching approach to coding that aims to push further in that direction.
</div>
<!-- ==================================================================================================== -->
                                    Documentation
<!-- ==================================================================================================== -->
<div id="{{ slugify("Writing Developer Documents") }}">

As you will be updating documentation of your project soon, here are some guidelines to help you with that.
</div>
<!-- ==================================================================================================== -->
                                    Testing
<!-- ==================================================================================================== -->
<div id="{{ slugify("Automated Testing of Text UIs") }}">

As you start adding features to your project iteratively, you'll need **a way to detect if the new code breaks the existing code**. Next, let's learn a rather simple way to do that using a certain type of testing (we'll be learning more sophisticated methods in later weeks).

<span tags="m--cs2103">This also means we are now switching focus from the _implementation_ aspect to the _testing_ aspect of SE.</span>
</div>
<!-- ------------------------------------------------------------------------------------------------------ -->
<div id="{{ slugify("Developer Testing") }}">

**Soon, you will start writing automated Java tests for your project**.

First, let us learn such testing fits into an aspect called _developer testing_ of the testing landscape.
</div>
<!-- ------------------------------------------------------------------------------------------------------ -->
<div id="{{ slugify("Unit Testing") }}">

_Unit testing_ is the type of _developer testing_ that is used the most. Let's learn about it next.
</div>
<!-- ------------------------------------------------------------------------------------------------------ -->
<div id="{{ slugify("testing-testAutomation-usingTestDrivers") }}">

**The sections below gives an overview of _test automation_**, something used heavily in developer testing.
</div>
<!-- ------------------------------------------------------------------------------------------------------ -->
<div id="{{ slugify("Testing: Intermediate Techniques") }}">

We started writing JUnit testing in the last week. The topics below helps you push a bit further in the same direction.
</div>
<!-- ------------------------------------------------------------------------------------------------------ -->
<div id="{{ slugify("Testing: Intermediate Concepts") }}">

One of the primary goals of a software engineer is to avoid bugs. You certainly don't want to be the person responsible for causing a major bug that caused heavy damages to some party. That's why we need to focus heavily on testing -- one of the main defences against bugs.

The next few sections cover some intermediate level testing topics that you are very likely to encounter in software engineering.
</div>
<!-- ------------------------------------------------------------------------------------------------------ -->
<div id="{{ slugify("Testing: Test Coverage") }}">

Previously, you learned how to write JUnit tests. **How do you know which parts of the code is being tested by your tests? That's where _test coverage_ comes in.**
</div>
<!-- ------------------------------------------------------------------------------------------------------ -->
<div id="{{ slugify("testing-testCoverage-how") }}">

Learn how to measure test coverage in your tP. You will be asked to demo that in the coming tutorial.
</div>
<!-- ------------------------------------------------------------------------------------------------------ -->
<div id="{{ slugify("followup-testing-tdd-how") }}">

You are welcome to, but not required to, follow the TDD approach in your project.
</div>
<!-- ---------------------------------------------------------------------------- -->
<div id="{{ slugify("Types of Testing") }}" >

As we approach the last part of the tP, we'll be spending more time learning about software testing. This week, we start off with an overview of different _types_ of software testing.
</div>
<!-- ---------------------------------------------------------------------------- -->
<div id="{{ slugify("Testing: Types") }}" >

You've already been doing some testing in your project work. It turns out there are many ways to categorize testing. Let's learn some of the more common categorizations of testing.
</div>
<!-- ---------------------------------------------------------------------------- -->
<div id="{{ slugify("testing-dependencyInjection-what") }}" >

_Dependency Injection_ is a technique closely related to stubs. It is not in the syllabus but is given below in case some of you would like to know more about it.
</div>
<!-- ---------------------------------------------------------------------------- -->
<div id="{{ slugify("Test Case Design") }}" >
<div id="{{ slugify("Test Cases: Intro") }}" >

Previously, we learned how to measure test _coverage_. This week, we look into how to increase coverage with the least number of test cases.

First, we take a look at test case design in general, different approaches to test case design, and few different categorization of test cases.
</div>
</div>
<!-- ---------------------------------------------------------------------------- -->
<div id="{{ slugify("testCaseDesign-introduction-what") }}" >

**What is _test case design_, and why should we care?**
</div>
<!-- ---------------------------------------------------------------------------- -->
<div id="{{ slugify("testCaseDesign-introduction-blackVsGlass") }}" >

**How much information about the code is being used when designing test cases?**
</div>
<!-- ---------------------------------------------------------------------------- -->
<div id="{{ slugify("Equivalence Partitioning") }}" >
<div id="{{ slugify("Test Cases: Equivalence Partitioning") }}" >

Next, a heuristic used for improving the quality of test cases.
</div>
</div>
<!-- ------------------------------------------------------------------------------------------------------ -->
<div id="{{ slugify("Boundary Value Analysis") }}" >
<div id="{{ slugify("Test Cases: Boundary Value Analysis") }}" >

Previously, you learned about _equivalence partitions_, a heuristic for dividing the possible test cases into partitions. But which test cases should we pick from each partition? Next, let us learn another heuristic which can help us answer that question.
</div>
</div>
<!-- ---------------------------------------------------------------------------- -->
<div id="{{ slugify("Test Cases: Combining Multiple Inputs") }}" >
<div id="{{ slugify("Combining Multiple Test Inputs") }}" >

Earlier, you learned <tooltip content="Equivalence Partitioning, Boundary Value Analysis">two heuristics</tooltip> that can improve the test case quality. Even when applying them, the number of test cases can increase when the SUT takes multiple inputs. Let's see how we can deal with such situations.
</div>
</div>
<!-- ---------------------------------------------------------------------------- -->
<div id="{{ slugify("Quality Assurance") }}" >
<div id="{{ slugify("Other QA Techniques") }}" >

Testing is the first thing that comes to mind when you hear 'Quality Assurance' but there are other QA techniques that can complement testing. Let's first take a step back and take a look at QA in general, followed by a look at some other QA techniques.
</div>
</div>
<!-- ---------------------------------------------------------------------------- -->
<div id="qualityassurance-formalverification-what" >

Previously, you already learned about two 'other' QA methods. This week, we add a third:

- [x] %%Code reviews%%
- [x] %%Static Analysis%%
- [ ] **Formal methods**

</div>
<!-- ==================================================================================================== -->
                                    Project Mgt
<!-- ==================================================================================================== -->
<div id="{{ slugify("SDLC Process Models: Basics") }}">

Now, let's switch our focus to the _project management_ aspect of SE.

Broadly speaking, there are two approaches to doing a software project. Those two approaches are also highly relevant to the way this course is run, and how it is different from most SE courses elsewhere.

Let's learn about those two approaches early so that we can better understand how this course works.
</div>
<!-- ------------------------------------------------------------------------------------------------------ -->
<div id="{{ slugify("SDLC Process Models: XP/Scrum") }}" >

In [a previous week](../schedule/week2/topics.html), you learned about _sequential_ and _iterative_ ways of doing a software.
Now, let us take a quick look at a couple of well-known processes used in the industry, both of which fall into a category called _agile processes_.
</div>
<!-- ------------------------------------------------------------------------------------------------------ -->
<div id="{{ slugify("Project Mgt: Scheduling and Tracking") }}">

<span tags="m--cs2103 m--cs2113">Coordinating a team project is not easy.</span> Given below are some very basic tools and techniques that are often used in planning, scheduling, and tracking projects.
</div>
<!-- ------------------------------------------------------------------------------------------------------ -->
<div id="{{ slugify("projectPlanning-ganttCharts") }}">

GANTT Charts and PERT charts are popular tools in the project management domain but they are rarely useful in small software projects. Hence, they are not included in {{ course }} syllabus but it is **useful to know at least their names and how they look like**.
</div>
<!-- ------------------------------------------------------------------------------------------------------ -->
<div id="{{ slugify("teamwork-teamStructures") }}">

This topic is included in the syllabus just **to let you know that teams can be structured in different ways**.

Which of them is closest to the structure of your team?
</div>
<!-- ------------------------------------------------------------------------------------------------------ -->
<div id="{{ slugify("Project Mgt: Workflows") }}">

Continuing on the same theme, given below are more practices used in managing projects, particularly related to the revision control aspect.
</div>
<!-- ==================================================================================================== -->
                                    Documentation
<!-- ==================================================================================================== -->
<div id="{{ slugify("documentation-tools-javaDoc-what") }}">

**You'll need to add JavaDoc comments to the iP code this week.** Let's learn how to do that.
</div>
<!-- ------------------------------------------------------------------------------------------------------ -->
<div id="{{ slugify("Writing Developer Documents") }}">

**You will be writing some developer documentation as well in the tP**, unlike the iP in which you only wrote some user documentation. To prepare you for that, given below is a brief introduction to developer documentation.
</div>
<!-- ==================================================================================================== -->
                                    Integration
<!-- ==================================================================================================== -->
<div id="{{ slugify("Integration Approaches") }}">

As you start adding new code to the tP, let's also become aware of various approaches in integrating new code to a product.
</div>
<!-- ------------------------------------------------------------------------------------------------------ -->
<div id="{{ slugify("Continuous Integration/Deployment") }}">

**Modern software projects, and your tP, make heavy use of build/CI/CD tools** The topics below give you an overview of those tools, to prepare you to start using them yourself.
</div>
<!-- ------------------------------------------------------------------------------------------------------ -->
<div id="{{ slugify("Automating the Build Process") }}">

As your project gets bigger and changes become more frequent, it's natural to look for ways to automate the many steps involved in going from the code you write in the editor to an executable product. This is a good time to start learning about that aspect too.
</div>
<!-- ==================================================================================================== -->
                                    Models/UML
<!-- ==================================================================================================== -->
<div id="{{ slugify("Design: Models") }}">

Software engineers often have to write _developer documentation_ to explain their work to others. One important objective of developer documentation is to explain the design and the implementation of the software, which usually uses diagrams as _models_ of the design being described.

**Let's learn what models are, and how they are useful even beyond mere documentation.**
</div>
<!-- ------------------------------------------------------------------------------------------------------ -->
<div id="{{ slugify("Class/Object Diagrams: Basics") }}">
<div tags="m--tic2002">

This course covers only two types of diagrams: class/object diagrams (CD/OD) -- which model a _structural_ aspect of an OOP design, and sequence diagrams (SD) -- which model a _behavioral_ aspect. This week, let's learn the basic CD/OD notation.

We recommend you ==try the relevant post-lecture quizzes as you read each sections== below. In these quizzes, you will  be able to see the answers immediately after completing the quiz.
</div>
</div>
<!-- ------------------------------------------------------------------------------------------------------ -->
<div id="{{ slugify("Followup Class/Object Diagrams: Basics") }}">

</div>
<!-- ------------------------------------------------------------------------------------------------------ -->
<div id="{{ slugify("Class/Object Diagrams: Intermediate") }}">

Having learned class/object diagrams basics, we can now move on to some intermediate CD/OD notations.

<div tags="m--tic2002">

But first, **try this CD/OD drawing example/exercise (solution provided)**.

{{ panopto("88a6d3bc-7bbb-4566-a035-ac4100ce1085", desc="[Example] Box, Item, Lid") }}
</div>
</div>
<!-- ------------------------------------------------------------------------------------------------------ -->
<div id="{{ slugify("Followup Class/Object Diagrams: Intermediate") }}">

Now, you can try these worked examples:
{{ panopto("052aa055-c89f-4dbf-af24-ac4000f175e0", desc="Drawing class/object diagrams (intermediate) - `Action`, `Task`, `History`") }}
{{ panopto("f4f7e1f2-60a4-4d18-b70a-ac4000f17608", desc="Drawing class/object diagrams (intermediate) - `Person`, `Inbox`, `Message`") }}
{{ panopto("e05845ed-8c70-47d9-a4d0-ac6800d58224", desc="Drawing class/object diagrams (intermediate) - `Person`, `Project`, `Task`") }}
</div>
<!-- ------------------------------------------------------------------------------------------------------ -->
<div id="{{ slugify("modeling-modelingStructures-objectDiagrams") }}">

**Object diagrams complement class diagrams**, and therefore, they are covered together with class diagrams.
</div>
<!-- ------------------------------------------------------------------------------------------------------ -->
<div id="{{ slugify("Class Diagrams: Intermediate-Level") }}">

**This week, let us learn the remaining class diagram notations**.
</div>
<!-- ------------------------------------------------------------------------------------------------------ -->
<div id="{{ slugify("Sequence Diagrams: Basics") }}">
<div tags="m--cs2113">

Good news: this will be the last installment of UML notations.<br>
Bad news: we are going to cover an entire new diagram type in one go (reason: to give you more time to use them in project documentation).
</div>
<div tags="m--cs2103 m--tic2002">

**Let us learn a UML diagram type that can be used to model a _behavioral_ aspect of software entities**; in contrast, class/object diagrams that you learned earlier model _structural_ aspects.
</div>
</div>
<!-- ------------------------------------------------------------------------------------------------------ -->
<div id="{{ slugify("Followup Sequence Diagrams: Basics") }}">
<div tags="m--tic2002">

Now that you know the basic notations for the sequence diagrams, here is a worked example of drawing sequence diagrams (basic notation) to match a code snippet.

{{ panopto("fe9d362e-4e3d-4c30-81ec-ac5a00cf8d95", desc="Sequence diagrams (basic) - `Item` creation") }}
</div>
</div>
<!-- ------------------------------------------------------------------------------------------------------ -->
<div id="{{ slugify("Sequence Diagrams: Intermediate") }}">

Earlier, you learned the basic notation used in sequence diagrams. Now, let's learn some intermediate notation.
</div>
<!-- ------------------------------------------------------------------------------------------------------ -->
<div id="{{ slugify("Followup Sequence Diagrams: Intermediate") }}">

Here is a worked example of drawing sequence diagrams (intermediate notation) to match a code snippet.

{{ panopto("3e47c3c3-60db-4e2f-a15f-ac4100ce10c4", desc="Drawing sequence diagrams (intermediate) - `TaskList#generateTask()`") }}
{{ panopto("c4856a68-4c30-4f9c-8efa-ac6800d581f2", desc="Drawing sequence diagrams (intermediate) - create `Quote`") }}
</div>
<!-- ------------------------------------------------------------------------------------------------------ -->
<div id="{{ slugify("OO Domain Models") }}">

Previously, you learned about class and object diagrams. Let's touch on another variant of class diagrams that complements the first two. The good news is that it is simply a subset of the notation that you already know.
</div>
<!-- ------------------------------------------------------------------------------------------------------ -->
<div id="{{ slugify("Followup OO Domain Models") }}">

Here is an example that shows the steps of drawing an OODM to match a given problem domain.

{{ panopto("8ee3d654-c865-45fb-ae08-ac4e003584af", desc="OODM for the tasks domain") }}
</div>
<!-- ------------------------------------------------------------------------------------------------------ -->
<div id="{{ slugify("Activity Diagrams") }}">

Activity diagrams is the {{ "first" if tee3201 else "last" }} UML diagram type you'll be learning in this course, and probably the easiest and most intuitive of the lot. You've heard about 'flow charts', right? Well, this is the UML equivalent of that.
</div>
<!-- ------------------------------------------------------------------------------------------------------ -->
<div id="{{ slugify("Followup Activity Diagrams") }}">

Here are some examples showing the steps of drawing an activity diagram to match a given workflow.
<include src="common-schedule-fragment.md#uml-worked-examples-ad" />

</div>
<!-- ------------------------------------------------------------------------------------------------------ -->
<div id="{{ slugify("Other UML Models") }}">

To complete the picture about UML, given below are a peek into the other types of UML diagrams.
</div>
<!-- ==================================================================================================== -->
                                   Design
<!-- ==================================================================================================== -->
<div id="{{ slugify("followup-design-introduction-what") }}">

Now that you know there are two kinds of 'design', also note that this course focuses more on the internal design rather than the external design.
</div>
<!-- ------------------------------------------------------------------------------------------------------ -->
<div id="{{ slugify("Design: Basics") }}">

While you are learning Python basics, let's also take a look at some other SE topics that we need to cover. In the early weeks, we try to cover SE topics somewhat independent from the programming topics being covered so that if you are slow on the programming side, you can still make progress on the SE side.

**To start, let's look at the _design_ aspect, and _abstraction_** which is a concept most fundamental to the design aspect (and to many other aspects of SE).
</div>
<!-- ------------------------------------------------------------------------------------------------------ -->
<div id="{{ slugify("Design: Fundamentals") }}">

As you do projects, you'll have to make design decisions e.g., decide between multiple design alternatives. Let us learn three fundamental design concepts that you can use in those decisions.

It is extremely important for you to know these three because **they are like the DNA of every higher-level design concept**.
</div>
<!-- ------------------------------------------------------------------------------------------------------ -->
<div id="{{ slugify("Design Principles") }}">
<div tags="m--cs2113">

As you are still in the early stage of the project, **this is a good time to learn some design principles that you can try to apply in the internal design of your product**.
</div>
<div tags="m--tic2002">

This week, we learn a few **design principles that you can try to apply in your project**.
</div>

These principles build on top of the design fundamentals you learned earlier (i.e., abstraction, coupling, cohesion).
</div>
<!-- ------------------------------------------------------------------------------------------------------ -->
<div id="{{ slugify("Design Principles: SoC, SRP") }}">

As you are still in the early stage of the project, **this is a good time to learn some design principles that you can try to apply in the internal design of your product**.

These principles build on top of the design fundamentals you learned earlier (i.e., abstraction, coupling, cohesion).
</div>
<!-- ------------------------------------------------------------------------------------------------------ -->
<div id="{{ slugify("Design Principles") }}">

Remember you learned about <tooltip content="Abstraction, Coupling, Cohesion">the three things</tooltip> that are 'like the DNA' of design concepts. It's time to move to the next level and learn some design _principles_ that build upon those three. Given below are two new principles and three that you should have at least touched on in previous courses.
</div>
<!-- ------------------------------------------------------------------------------------------------------ -->
<div id="{{ slugify("designFundamentals-abstraction-what") }}">

Let's start by learning **the three most fundamental design qualities** upon which all other design principles are built.
</div>
<!-- ------------------------------------------------------------------------------------------------------ -->
<div id="{{ slugify("Some Principles") }}">

Given next are **two design principles that we can apply when designing OOP systems**. These aim to improve <tooltip content="abstraction, coupling, cohesion">the three design qualities you learned earlier</tooltip>.
</div>
<!-- ------------------------------------------------------------------------------------------------------ -->
<div id="{{ slugify("principles-interfaceSegregationPrinciple") }}">

If you liked the principles covered above, given below are a few more widely used principles most of which are optional in this course (they were moved to the optional topics in order to reduce the course workload).

The only examinable thing is ==the term== _SOLID principles_.
</div>
<!-- ------------------------------------------------------------------------------------------------------ -->
<div id="{{ slugify("Design Patterns") }}">

Previously, you learned:
* Three basic design quality aspects: abstraction, coupling, cohesion
* Some design principles (e.g., _Single Responsibility Principle_) that aim to improve those aspects. <span tags="m--cs2113">There are many more principles but we covered only two (to reduce workload) just to give you a taste only.</span>

**This week, we cover _design patterns_, a concept that builds upon the above**. <span tags="m--cs2113">Again, we limit to only two of them, for similar reasons.</span>
</div>
<!-- ------------------------------------------------------------------------------------------------------ -->
<div id="{{ slugify("designPatterns-introduction-what") }}">

First, let's learn what _design patterns_ are, in general.
</div>
<!-- ------------------------------------------------------------------------------------------------------ -->
<div id="{{ slugify("Singleton pattern") }}">

Now that you know what _design pattern_ is, let's learn a few example design patterns.
</div>
<!-- ------------------------------------------------------------------------------------------------------ -->
<div id="{{ slugify("More Design Patterns") }}">

Previously, you learned about design patterns, and some example design patterns. Let's continue that journey this week.
</div>
<!-- ------------------------------------------------------------------------------------------------------ -->
<div id="{{ slugify("designPatterns-modelViewController-what") }}">

First, let's learn two more widely-cited design patterns.
</div>
<!-- ------------------------------------------------------------------------------------------------------ -->
<div id="{{ slugify("designPatterns-more-otherDesignPatterns") }}">

Given below are a few more topics that continue the theme of design patterns, but have been made optional to reduce the course workload.</div>
<!-- ------------------------------------------------------------------------------------------------------ -->
<div id="{{ slugify("Architecture") }}" >

**While _architecture_ is not of high importance to a small project such as the tP, it is good to know a little bit about it** in case you are thrown into a larger project in future.
</div>
<!-- ------------------------------------------------------------------------------------------------------ -->
<div id="{{ slugify("Architectural Styles") }}" >

The next topic is like 'design patterns at architecture level'. In fact, the MVC pattern you saw earlier comes close to this category too.
</div>
<!-- ------------------------------------------------------------------------------------------------------ -->
<div id="{{ slugify("followup Architectural Styles") }}" >

As with design patterns, we covered only a few architecture styles. Although you didn't have to design an architecture in the tP, knowing the existence of these styles might come in handy in your future projects.
</div>
<!-- ---------------------------------------------------------------------------- -->
<div id="{{ slugify("designApproaches-multilevelDesign-what") }}" >

**First, let us learn about multi-level design**, a pre-cursor to learning about architecture.
</div>
<!-- ---------------------------------------------------------------------------- -->
<div id="{{ slugify("architecture-introduction-what") }}" >

Now that we know about multi-level design, let us learn about architecture, which is a special case of multi-level design. We also cover _architecture diagrams_ here.
</div>
<!-- ---------------------------------------------------------------------------- -->
<div id="{{ slugify("Architecture Diagrams: Drawing") }}" >

You've already encountered architecture diagrams in your tP. Pretty soon, you might have to update that diagram to match your new product. Given below are just a brief note about drawing architecture diagrams.
</div>
<!-- ---------------------------------------------------------------------------- -->
<div id="{{ slugify("Architectural Styles") }}" >

Remember _design patterns_? The _architectural styles_ covered below are like 'design patterns' at architecture level. As before, we only cover two of them just to give you a taste of the topic while keeping the workload low.
</div>

<!-- ---------------------------------------------------------------------------- -->
<div id="{{ slugify("Conceptualizing a Design") }}" >

A few weeks ago, you learned how to interpret UML diagrams. More recently, you learned how to draw diagrams to match code. There's a third use of models: as an aid for coming up with a design _before_ the code is written.

While this course doesn't ask you to come up with detailed designs before writing code (i.e., our approach leans closer to the _agile_ design rather than the _full design upfront_ approach), this third use of models come in handy at times. Let's learn a bit about that too.
</div>
