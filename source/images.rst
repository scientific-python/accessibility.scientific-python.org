Images
======

Scope
-----

Summary of Scope
~~~~~~~~~~~~~~~~

-  This SPEC’s scope is on making visual media accessible to people with
   screen-readers.
-  This can be done with the implementation of ‘alt-text’ in images.

‘Accessible’ is a very broad term, so is ‘accessible open-source’.
Open-source projects can be more accessible to people with visual,
auditory, physical, speech, and neurological disorders. Disabilities can
be permanent, temporary or situational [citation to WCAG page on Diverse
Abilities and
Barriers)](https://www.w3.org/WAI/people-use-web/abilities-barriers/].

This SPEC’s scope is on making visual media accessible to people with
visual disabilities who use screen-readers. Visual media can be made
accessible through the implementation of ‘alternative-text’ (alt-text).

People with visual disabilities include not only people who are blind
with complete vision loss, but also people with partial vision loss,
blurry vision, low-contrast vision and color-blindness. Some specific
visual disabilities include myopia, cataracts and red-green
color-blindess.

Some people with visual disabilities use assistive technology such as
screen-readers to use the computer, navigate websites and use programs.
Screen-readers ‘read out’ text and are used with keyboard commands to do
a variety of actions. This is possible because how people with and
without visual disabilities navigate web-pages is fundamentally the
same. A web-page is built from elements such as headers, text, images
and links. A user can navigate between these elements with a mouse,
keyboard, screen-reader and more.

Screen-readers can preview and skip information by jumping between page
headers, which is similar to visually skimming text. Screen-readers can
also read out images with alt-text.

Alt-text is a short summary of an image. When screen-readers can read
out images with alt-text, the user can still experience the image and
access the valuable information images provide.

Images without alt-text are inaccessible to people using screen-readers.
Valuable information is lost. For example, an tourism website may
provide an image of a map showing the nearest exits in a museum. If no
alt-text is provided, a user with a screen-reader misses this
information. An alt-text of ‘A map of the museum. The nearest exits are
to the left of the dinosaur exhibit.’ makes this information accessible
and allows the user to navigate a physical space with independence.

Alt-text is rendered on web-pages as the HTML alt attribute [citation to
MDN]. When uploading images online, the creator can attach alt-text to
an image.

There are many excellent resources available for writing alt-text, such
as the Web Content Accessibility Guidelines (WCAG). However, there are
many concerns specific to scientific Python open-source projects that
WCAG does not adequately address. Therefore this SPEC aims to provide
guidelines for writing alt-text for scientific Python open-source
projects..

There are other worthwhile concerns about how open-source can be more
accessible, such as keyboard accessibility. However, the implementation
of that is beyond the scope of this SPEC. These are worthwhile topics
for future SPECs.

Description of deliverables
---------------------------

The desired outcomes from the adoption of this SPEC is: \* Accessible
images with alt-text within various contexts in open-source software: \*
Main website \* Documentation \* Blog posts \* Videos \* Community
Meeting Notes \* and more

On a broader level, this SPEC also aims to create a cultural shift where
people with disabilities feel welcome in open-source spaces. By removing
these barriers, people with disabilities can use open-source software
and disabled developers can contribute back. Thus open-source can better
serve the needs of its disables users and in turn disabled people can
shape open-source.

Implementation
--------------

Implementing alt-text for images used in open-source software can seem
like a big task. There are probably many existing images without
alt-text. In the same way projects can have technical debt, there may
also be ‘accessibility debt’ to cover. Accessibility may not be part of
the contribution review process, such as requesting alt-text in
submissions or in CI tests. There are many options for auditing: manual
and automated. This auditing can be done internally by contributors or
commissioned to an external auditing company.

However, implementing alt-text can be done: if done deliberately, in
stages and in coordination with others.

This section aims to highlight case studies where projects have
implemented this SPEC’s guidelines, their unique challenges, solutions
and outcomes.

The SPEC process is primarily aimed at ‘SPEC Core Projects’. The Core
Projects are a small subset of the Scientific Python ecosystem
consisting of mature, community developed projects that are (a) depended
upon by most of the other projects and (b) responsible for reviewing,
discussing, implementing, and endorsing SPEC documents. The full list of
Core Projects can be found at the `SPEC Core Projects
page <https://scientific-python.org/specs/core-projects/>`__.

The SPEC process is primarily aimed at ‘SPEC Core Projects’ due their
foundational nature. Rather than having projects built on top of
open-source software inherit problems or create their individual
patches, SPEC Core Projects have the power to solve accessibility
problems across the board.

However, projects that are not SPEC Core Projects are certainly welcome
to learn from and adopt this document. We invite discussion of any
project’s needs and questions in this `SPEC’s
forum <https://discuss.scientific-python.org/t/discussion-accessible-open-source-projects/63>`__.

Any project is invited to use the Reference section in writing alt-text.
The Reference section aims to be a centralized resource for writing
alt-text specific for open-source software’s needs.

Core Project Endorsement
~~~~~~~~~~~~~~~~~~~~~~~~

In the SPEC process, a SPEC document has three main stages: accept,
endorse and adopt.

The authors of this SPEC are contributors in the SPEC Core Projects.
They have also made several contributions specific to accessibility and
alt-text. In their discussions with other contributors, they have seen
several recurring questions worth documenting. They have also developed
guidelines specific for open-source processes that are not answered by
general alt-text guidelines. Therefore they have written this SPEC to
share this knowledge and open this discussion with others.

The accept decision of the SPEC process is made by the SPEC Steering
Committee. The Steering Committee represent the interests of the Core
Projects and is composed partially of individuals who are active Core
Project contributors. The full description and list of members can be
found in the `SPEC Steering Committee
page <https://scientific-python.org/specs/steering-committee/>`__

The endorse decision is made by the Core Projects. The Core Projects and
interested community members revise the accepted SPEC in a collaborative
and iterative process focused on ensuring the SPEC implementation plan
that is broadly applicable and likely to be widely adopted.

The following Core Projects endorse this SPEC. #### NumPy #### (Second
Core Project) #### JupyterLab

Ecosystem Adoption
~~~~~~~~~~~~~~~~~~

The final stage in the SPEC process is adoption.

The adopt decision is made by individual projects according to their own
decision-making processes. Any project in the ecosystem is welcome to
adopt a SPEC at any point. However, it may make sense to wait until a
SPEC is endorsed by several Core Projects

Core Projects interested in formally adopting this SPEC can follow the
`SPEC Purpose and Process
page <https://scientific-python.org/specs/purpose-and-process/>`__.

Formally adopting this SPEC has several advantages. It provides a space
to ask questions, provide shared solutions and prevent ‘re-inventing the
wheel’. It signals a project’s recognition and investment of
accessibility as a core tenant of open-source software. It prepares
Scientific Python for the next decade of scientific discovery and user
growth.

The following Core Projects have adopted this SPEC. Each section
highlights how a project has implemented this SPEC’s guidelines, their
unique challenges, solutions and outcomes. #### NumPy #### (Second Core
Project) #### JupyterLab

Closing
-------

Accessibility comes in various forms beyond alt-text. The authors of
this SPEC hope this document answers questions, coordinates across
projects, inspires action and the development of future SPECs focused on
accessibility.

This is the end of the high-level overview. The next section is the
reference section.

The `reference section <https://accessibility.scientific-python.org/>`__
is similar to an API reference. Look at the Table of Contents to see if
any section pertains to your project or current needs.

| The reference sections of this document is divided into: \* Best
  practices, main principles and style guide \* Guidelines for writing
  alt-text by image type (graphs, logos, gifs, etc) \* Guidelines by
  context (main website, documentation, blog posts, etc) \*
  Project-specific needs
| \* Frequently-Asked-Questions

Notes
-----
