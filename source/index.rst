Accessibility
=============

.. toctree::
   :maxdepth: 2
   :hidden:

   images
   reference


Motivations and Barriers
------------------------

Summary of Motivations and Barriers
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

-  Accessibility is about making technology accessible to the full range
   of human experience, which includes disabilities.
-  General reasons why open-source software should be more accessible:

   -  accessibility benefits everyone
   -  access to information and technology as human right
   -  enjoyment and creation for disabled people

-  Reasons very specific to open-source software:

   -  achieve the ethos of open-source
   -  solving root problems due to open-source’s scale
   -  better represent needs of disabled users

-  Open-source software is currently not very accessible due to:

   -  decentralized structure
   -  uncertainty in implementation
   -  different accessibility needs of open-source software
   -  under-representation of disabled users
   -  insufficient funding

Accessibility is about making the world accessible to the full range of
human experience, which includes disabilities. For example, the physical
world can be made more accessible for wheelchair users by having more
buildings with ramps. Not only should the physical world be accessible,
but the digital world as well.

More and more people are accessing the world digitally. Access to the
internet is a human right. [citation for UN]. With access to the
internet, people can access vital information, such as education
[citation for various country laws to access education] or their banking
information.

People with disabilities access the internet as well. Blind users can
access text on websites with assistive technology such as a
screen-reader, which verbally reads text out loud. Thus assistive
technology empower disabled people to live autonomous lives.

An accessible world allows people with disabilities to not only access
information, but also communicate and create. Helen Keller’s access to
Braille, another form of assistive technology, allowed her to read about
the world. She used Braille to communicate with others who were
Deaf-Blind. It also allowed her to publish her experiences [citation for
Story of My Life] and advocate for the Deaf-Blind community to the
general public.

Accessibility benefits everyone. For example, captions for videos
benefit not only Deaf viewers with complete hearing loss, but also
viewers with partial hearing loss due to age. Captions also benefit
viewers who cannot play audio out loud, such as in a quiet environment
or if they have broken speakers. [citation to range of disabilities and
situational disability]. Thus accessibility benefits not just “a few
disabled people”[a] but all people.

These are general reasons why open-source software should be more
accessible. However, there are reasons very specific to open-source
software as well.

Open-source software should be more accessible to better achieve the
aims and ethos of open-source. Open source prides itself as available to
all, due to its XYZ license [citation]. Money and licensing should not
be a barrier to creating art for self-expression [GIMP vs Photoshop] or
creating mathematical graphs for research [matplotlib vs MatLab].
However, available does not necessarily mean accessible.

A project’s community meetings available for all contributors to attend,
but inaccessible to some due to time-zone differences. For example, a
community meeting held at UTC XYZ. For a contributor in New York City,
this meeting would be easily accessible at their local time of 3pm. For
a contributor in New Delhi, India, this meeting would be inaccessible at
their local time of 1am. In turn, to make their meetings more
accessible, some projects alternate their meeting times [citation, NumPy
alternate IST-friendly meeting].

In a similar way, disabled developers may not be able to access
documentation or navigate the user interface of open-source software.
For a visually-disabled developer, an image can still be accessed via
screen-reader. The screen-reader reads out-loud the image’s ‘alt-text’,
which is a short description of the image. Images in documentation are
valuable sources of information. However, images without ‘alt-text’
cannot be accessed this way, and the developer loses valuable
information.

For open-source software that uses a graphical interface, a mouse can be
used to interact with the elements in the interface, such as clicking a
cell or hovering over a button. A developer with motor-disabilities may
interact via keyboard instead. The developer can navigate across
elements via the Tab key and select to interact with the Enter key. A
user interface that is not keyboard-navigable cannot be accessed at all
for the developer.

If a developer cannot access open-source software, they are much less
likely to join open-source spaces. Contribution and community engagement
is the lifeblood of open-source development. Inaccessible open-source
software is less diverse, and diverse contributions make open-source
stronger [citation].

Thus, to truly make open-source available to all, it needs to be
accessible as well.

Accessible open-source affects not only disabled developers, but
disabled users as well.

Open-source software should be more accessible due to a matter of scale.
Open-source is foundational to modern digital infrastructure [citation…
that xkcd comic?]. Problems at the foundational level are magnified at
scale, and thus inaccessible open-source projects affect millions of
users across the world [citation of chapter in book ‘The Making and
Maintenance of Open Source Software’].

For example, the open-source software CodeMirror is used as part of the
Firefox’s Developer Tools [citation]. CodeMirror provides a code editor
in the browser. However, Codemirror 5 and its previous versions were
inaccessible to keyboard and screen-reader users. It did not support the
use of the Tab key as a navigational input. Instead, the Tab key could
only be used for code indentation.

As Firefox is used by millions of users every month [citation on usage],
millions of people have inherited this inaccessibility. Thus at scale,
many users could not access Firefox’s Developer Tools. It was only years
later with the release of Codemirror 6 that an option was provided to
use the Tab key as navigational input as well. Rather than having
projects built on top of open-source software inherit problems or create
their individual patches, open-source projects have the power to solve
accessibility problems across the board.

Barriers
~~~~~~~~

The current state of open-source software is not very accessible, for a
variety of reasons.

Open-source software is currently not very accessible due to its
decentralized nature. Being decentralized is both open-source software’s
greatest strength and weakness. It allows anyone to contribute, and
different contributors contribute different things. However, this can
also make it difficult to create a cohesive alternative experience for a
screen-reader user, keyboard user and more. If an accessibility is not
evenly applied, a user journey can be disrupted, such as with a keyboard
trap [citation]. Thus to make open-source software more accessible, it
must be done deliberately, in stages and in coordination with others[b].

Open-source software is currently not very accessible due to uncertainty
in implementing accessibility. The vast majority of contributors in
open-source software are software developers [citation on percentage].
While developers may feel comfortable contributing code, they may feel
less comfortable contributing outside of the usual wheelhouse, such as
accessibility. While there is growing awareness about accessibility in
open-source [citation], contributors may still hold back due to a fear
of ‘doing it wrong’. By providing guidelines in this document, we hope
that this uncertainty can be overcome.

Open-source software is currently not very accessible due to the
different accessibility needs of open-source software. Current
accessibility guidelines are for general use and focused primarily on
web-pages [citation, WCAG]. There are guidelines specific for certain
sectors, such as education and the creation of accessible tests for
disabled students [citation, Diagram Center and USA education]. However,
these guidelines are not suited for open-source’s technical demands and
processes. There are much less resources on how to make a command-line
interface accessible, best practices in writing accessible documentation
or community meeting notes. This document aims to provide guidelines
specific for open-source software.

Open-source software is currently not very accessible due to the
under-representation of disabled people in open-source spaces. While
disabled people make up X [citation of disabled people in general
population], in open source the number is Y [citation]. The above cited
barriers prevent disabled people from using open-source software and
reporting problems with their experiences, such as with Github Issues.
These barriers also prevent disabled developers from contributing back.
If disabled people are kept out of a space, then disabled people’s
voices are not heard within that same space. It creates a
chicken-and-egg problem where open-source software is not made with
disabled users in mind and in turn disabled users cannot help shape
open-source.

Open-source software is currently not very accessible due to
insufficient funding for accessibility. Open-source software relies not
only on volunteer labor of contributors, but also paid labor through
grants [citation]. Grants allow proposed features to be prioritized and
created in a sustainable way. However, out of X dollars spent on funding
open-source software, only Y percent, Z dollars is spent on
accessibility [citation]. This is related to the above mentioned problem
of under-representation. In a grant proposal,it can be difficult to
justify funds for making open-source accessible without proof of demand
such as with a high number of Github issues about accessibility
[citation of grant-proposal process[c]]. Thus this lack of funding
perpetuates another cycle where accessibility is not financially
supported.

Overcoming Barriers Together
~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Open-source software can begin to be more accessible by coordinating
with each other. Within the scientific Python ecosystem, there is one
such effort: the Scientific Python Ecosystem Coordination (SPEC).

The SPEC process is designed to identify areas of shared concern between
projects in the scientific Python ecosystem and to produce
collaboratively written, community adopted guidelines for addressing
these areas. Such guidelines are known as ‘SPEC documents’ or a ‘SPEC’.

Projects in the ecosystem have an existing, diverse set of proposal
processes and development constraints. SPECs complement these: they are
a mechanism to encourage shared practices and improve uniformity of
experience across projects. This SPEC captures established practices so
that new projects can learn from them. As SPECs are living documents,
authors may propose a new practice that they believe will benefit the
ecosystem as a whole.

Projects decide for themselves whether to adopt any given SPEC—often,
this would be through team consensus. A SPEC may not be a good fit for
every single project, and thus there is no expectation that all SPECs
must be adopted by all projects. That said, SPECs serve their purpose
through being adopted by several projects—and their authority stems from
the extent to which they are. [citation, SPEC Processes page]

The purpose of this SPEC document is to: - Make the ecosystem more
accessible - Clarify the broad term accessibility and its various
possible implementations - Provide specific assessment tools and steps -
Direct to existing accessibility standards and modifications for open
source specifically - Provide case studies of how different core
projects became more accessible - Start discussion and develop shared
solutions
