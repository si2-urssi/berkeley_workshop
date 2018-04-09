# Usability and Software Sustainability

[Dan Gunter](dkgunter@lbl.gov)<br/>
Lawrence Berkeley National Laboratory

## Introduction

Our experience shows us that the best practices for usability
and user experience can have a strong positive effect on
software sustainability.  User research methods have been shown to result in gains
in productivity, improve performance of underlying systems, produce
cost-savings and reduce the cost of fixing software failures [1].

In the past 30 years, a significant body of practice and knowledge has
been developed on how to improve the quality of the user
experience. A body of theory and practice is also being disseminated
through academic courses and degree programs targeted at Human-Computer
Interaction (HCI). However, much of this knowledge and theory is non-required
coursework for computer science majors, and considered esoteric by researchers
coming from scientific backgrounds. In addition, much of the content
leans towards commercial large-scale software or cutting-edge HCI
research. The dynamic nature of scientific
collaborations and data analyses projects introduces different challenges
in applying basic, classical user-centered design methodology to
development of research software.

In the last several years, we have used user research methods in
our research and software development projects. We have developed
and modified practices to be suitable for the scientific community. We
have used a variety of techniques -- including participant observation,
interviews, heuristic evaluation, and usability studies -- to
understand, collect, and refine user requirements and improve
usability of software products. We have used these techniques in our
projects to improve user interfaces for data exploration and analyses,
workflow APIs, and building data management tools.
Our collaborations have included various
scientific domains, including bioinformatics, materials, environmental,
and climate sciences. These methods influence not only the user
experience but also the design of the overall system and the software
development life cycle.  It enables teams to focus on user needs early
and often and remove biases and preferences of the designers. Software
based on user needs has a streamlined implementation path and has a
greater chance of adoption.

## Best Practices for Usability

Much has been written
on methods, applications, and tools for usability engineering in HCI
textbooks, journals, and conference papers. An entire volume of
Springer's Human-Computer Interaction series [2] is
dedicated to the interplay between usability, HCI, and software
engineering. Briefly, the major methods are:

* Participant observation: Passively observe the target users performing their
work (or, if developer is part of the target audience, reflect on your own
  work practices)  _before_ any new software is introduced.
* Interviews: Actively discuss requirements with target users. There are
some specific approaches needed to avoid common pitfalls of "requirements
analysis".
* Heuristic evaluation: Evaluate the usability against known principles.
These are also called "expert reviews", but there are standard checklists
that allow this to be performed by virtually anyone.
* Usability studies: Also called [usability testing](https://en.wikipedia.org/wiki/Usability_testing).
This refers to testing the software with the end users in a controlled setting.

The application of these methods introduces a significant up-front "planning"
component to software development. It encourages incremental development
based on non-functional or semi-functional prototypes, which are "tested"
with users and heuristics before the full implementation. This introduces
an interesting dynamic with the so-called "agile" methods of software development,
as well as the naturally dynamic and exploratory nature of research software.

## Challenges and Opportunities for Software Sustainability

Incorporating usability into the core practices for research software
has a number of challenges. But, in the context
of a coordinated effort to improve software sustainability,
we see opportunities for usability to help frame and extend
classical software engineering and community engagement approaches.

### Challenges

There are challenges to incorporating usability and user experience practices
into research software development and we call out several major ones below: training, evaluation and credit, implementation, and communication.
These challenges partially overlap with the challenges facing classical
software engineering approaches (continuous integration, release management, etc.), and we discuss this overlap further in the Opportunities section.

**Training.** Additional knowledge and skills are required to address usability issues
efficiently and thoroughly. The required training materials for introducing
these skills to the non-specialist (i.e., scientist/programmer or computer
scientist without HCI background) are not as readily available as courses on
agile development, testing, using version control, etc. Formal methods taught
in university courses may not apply directly to research or scientific
software, where one programmer may wear many hats and the software development
cycle may be punctuated by many exploratory detours (see [3] for more discussion of this point).

**Evaluation and credit.** The quality of "usability" _can_ be evaluated, but
this is not well-recognized or widely practiced. Measurement of usability is
rarely given the prominence of other metrics such as software performance, and
does not appear as a factor in the inclusion of software in research publications.
The effort  put into usability is usually not recognized explicitly, leave alone
credited to specific individuals. It is also true that the measurements of
usability are more subjective than software timings or numerical accuracy, and
therefore require more explanation and/or statistical rigor.

**Implementation.** The research software and scientific software environments
are quite challenging places to introduce "new" techniques. Individual researchers often perform variations of the
 same analysis over and over, developing workarounds for software
 quirks. Different researchers may use different software tools for
 the same tasks. This creates an environment that is both dynamic (many tools and
 systems) and resistant to change (repeatability and deadlines).  
 The boundaries of the software development life cycle -- requirements gathering, design, and implementation -- are
 not strongly differentiated. This creates an environment that is resistant
 to the structures introduced of observation, interviews, heuristics, and testing to improve usability.

**Communication.** The language of usability research and best practices
is unfamiliar to many reviewers of, particularly, grant proposals. This makes
it more difficult to insert the various time and effort requirements into
proposed deliverables. Explanations of what, why, how, etc. distract from
the content of the proposal. This is compounded by the lack of easily
communicated measurements for achievement of "usability", as described
previously.

### Opportunities

The opportunities for expanding the use of usability research and practices to
create more sustainable software stem primarily from the fundamental alignment
of the goals of usability -- allowing other people to understand and use
your software -- with the goals of sustainable software, which could be
described as allowing software to continue to exist and thrive beyond its
initial demonstration of utility. The categories of opportunities mirror
the challenges discussed above.

**Training.** More and new training is required for classical software engineering techniques. While this is being developed, there is an opportunity
to incorporate training on usability best practices. For programmers coming
from scientific backgrounds, we have found that the value of user research is more immediately obvious, and thus usability training may actually serve as a less painful first step towards the full toolbox of usability and software
engineering practices.

**Evaluation and credit.** Because, as noted above, there are techniques
for evaluating usability, there is an opportunity to formalize and
socialize those techniques within the community so that people who have
developed highly usable software get the credit they deserve, and
research software that is not very usable can be targeted for improvement.
This is also an opportunity to discuss frankly how much the sustainability
of the software is important, since software that is not usable is not
going to be sustainable. In other words, if software is really a prototype with
no expected user community, putting "n/a" for the usability evaluation is
a much clearer signal of this intent than the word "prototype" (which could simply mean "I need more time").

**Implementation.** Usability research and practices encourage a holistic
approach to software, i.e. rather than focusing solely on the algorithms or performance goals, the developer starts with questions about who will use the software and how they will use it. These are exactly the kinds of questions
that must be asked in order to foster a community around any research software.
Even when the target community is a student and a professor, answering
these questions thoroughly can save time and effort.
When it comes to expanding software to more and other users, user research techniques are a necessary tool, and will pay dividends in community
engagement.

**Communication.** We have had some success talking about usability
in Department of Energy grants, so there is an opportunity in a coordinated
effort to develop more standard language, along the lines of language
added for data management. The ultimate goal, however, is to move an
understanding of usability into "common knowledge", where it can simply
be referenced by shorthand in grants and other writing. This will not
happen overnight. In the meantime, another application of usability is to leverage the understanding (observation and interviews) and evaluation (heuristics and user testing) practices as natural "bookends" for research software milestones. Some standard language and training on how to do this could be a useful way to start introducing usability in project deliverables.

## Conclusion

An active and structured approach to software usability has been shown to
pay dividends in both quality and uptake of the result. Based on our experience
with scientific software, we can confidently say that this general statement
is just as true for research software. We have described some challenges and
concomitant opportunities for introducing usability research and practices
into the effort to improve software sustainability. We look forward to
further discussions of concrete steps that can be taken to make these
ideas a reality.

## References

[1]: https://isbnsearch.org/isbn/0201192462 Gilb, Tom, "Principles of Software
Engineering Management", Addison-Wesley Longman Publishing Co., Inc.,
Boston, MA, USA, 1988. ISBN: 0-20-119246-2

[2]: https://books.google.com/books?id=NkMp0\_spR5QC Seffah, A., Gulliksen, J.,
and Desmarais, M.C., "Human-Centered Software Engineering - Integrating Usability in the Software Development Lifecycle",
Human-Computer Interaction Series, Springer Netherlands, 2006. ISBN: 9781402041136

[3]: https://ieeexplore.ieee.org/document/8109139/ Ramakrishnan, L. and Gunter, D., "Ten Principles for Creating Usable Software for Science", eScience 2017.
