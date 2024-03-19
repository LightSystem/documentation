Create surveys
==============

To create a survey in the Odoo *Surveys* application, navigate to :menuselection:`Surveys app -->
New` to reveal a blank survey form.

[image of blank survey form]
.. image:: create/TBD.png
   :align: center
   :alt: 

.. note::
   The :guilabel:`New` button is **not** present on the *Surveys* dashboard if in the *Activities*
   view.

At the top of the survey form are four radio buttons, each representing a survey style. The radio
button options are:

- :guilabel:`Survey`
- :guilabel:`Live Session`
- :guilabel:`Assessment`
- :guilabel:`Custom` (selected by default)

These options are here to streamline the survey-making process, by providing users with automated
settings and options that are ideally specific to those types of surveys. Each of those survey type
options comes equipped with its own specific selection of options.

The :guilabel:`Custom` option, selected by default, offers all the options from every potential
survey type. Those options are located in the :guilabel:`Options` tab of the survey form.

Beneath those radio survey type options is a blank field in which a name for the survey **must** be
entered.

Below the survey name field, is the :guilabel:`Responsible` field. Designate any user from this
drop-down menu to be in charge of the survey. The user who initially created the survey is chosen as
the default :guilabel:`Repsonsible`.

To the right of those fields, and above the tabs, is the option to add a background image,
represented by a :guilabel:`(camera and plus sign)` icon. When clicked, the option to upload an
image becomes available. This image would be used as the background image for the entire survey.
This is **not** a required option.

Below those fields and options are four tabs: :guilabel:`Questions`, :guilabel:`Options`,
:guilabel:`Description`, and :guilabel:`End Message`.

Questions tab
=============

Add questions and sections to the survey in the :guilabel:`Questions` tab. 

Create sections
---------------

A *section* divides the survey into organized parts, in order to visually group similar questions
together. To make a section, click :guilabel:`Add a section` at the bottom of the
:guilabel:`Questions` tab, proceed to type in a desired name for the section, then either press
'Enter' or click away. 

Then, drag-and-drop desired questions beneath that section, or drag-and-drop the section title on
top of (before) the desired question(s), in order to populate the section with specific questions
that fit the theme of the section. Sections create neatly divided, organized sections in a survey.

Create questions
----------------

To create questions for the survey, click :guilabel:`Add a question` in the :guilabel:`Questions`
tab.

Clicking :guilabel:`Add a question` opens the :guilabel:`Create Sections and Questions` pop-up
window, in which a survey question can be created.

Create sections and questions
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

[image of the 'Create sections and questions pop-up']
.. image:: create/TBD.png
   :align: center
   :alt: 

In the :guilabel:`Create Sections and Questions` pop-up window, start by typing the question in the
:guilabel:`Question` field. 

Then, choose the desired :guilabel:`Question Type`. A preview of the question type is shown in the
preview window to the right of the :guilabel:`Question Type` field.

Choose from the following :guilabel:`Question Types`:

- :guilabel:`Multiple Lines Text Box`
- :guilabel:`Single Line Text Box`
- :guilabel:`Numerical Value`
- :guilabel:`Date`
- :guilabel:`Datetime`
- :guilabel:`Multiple choice: only one answer`
- :guilabel:`Multiple choice: multiple answers allowed`
- :guilabel:`Matrix`

.. note::
   Different features appear in the :guilabel:`Answers` and :guilabel:`Options` tabs, depending on
   the chosen :guilabel:`Question Type`.
   
   However, the :guilabel:`Description` tab **always** remains the same, regardless of what question
   type is chosen.

Once a :guilabel:`Question Type` has been selected, there are three possible tabs where information
can be customized for the question. These include the :guilabel:`Answers` tab (if applicable),
the :guilabel:`Description` tab, and the :guilabel:`Options` tab.

Each tab offers a variety of different features, depending on what :guilabel:`Question Type` was
chosen.

Answers tab
***********

The :guilabel:`Answers` tab **only** appears if the selected :guilabel:`Question Type` provides
answer options to the participant.

But, if a custom response is required to answer the selected :guilabel:`Question Type`, like a
:guilabel:`Multiple Lines Text Box`, for example. Or, if the answer to the :guilabel:`Question Type`
is a number, date, or datetime, the :guilabel:`Answers` tab disappears completely.

However, if the :guilabel:`Single Line Text Box` is selected as the :guilabel:`Question Type`, the
:guilabel:`Answers` tab remains, although it only provides two checkbox options: :guilabel:`Input
must be an email` and :guilabel:`Save as user nickname`.

For all other applicable :guilabel:`Question Type` options that provide answer options to the
participant, the :guilabel:`Answers` tab appears the same, with a :guilabel:`Choices` section, from
which users can add answer options by clicking :guilabel:`Add a line`, and typing in the various
answer options for that question.

An exception that is if the :guilabel:`Matrix` option is selected as the :guilabel:`Question Type`.
If that's chosen, the :guilabel:`Answers` tab remains, but below the typical :guilabel:`Choices`
section, there is a :guilabel:`Rows` section. That's because the :guilabel:`Matrix` option provides
an answer table for participants to fill out.

Description tab
***************

In the :guilabel:`Description` tab of the :guilabel:`Create Sections and Questions` pop-up window is
used to provide any kind of guidelines, instructions, or any other type of supplemental material
deemed necessary to help participants answer/understand the question.

Entering a description is **not** required.

Options tab
***********
[[[[[[[PICK UP FROM HERE]]]]]]]




For example, in the :guilabel:`Options` tab, the following options may appear:

- :guilabel:`Mandatory Answer`: the question must be answered.
- :guilabel:`Matrix Type`: for matrix-type questions, select if one choice or multiple choices can
  be selected per row.
- :guilabel:`Number of columns`: select how many columns are displayed.
- :guilabel:`Images on answers`: allow images on the answer options.
- :guilabel:`Conditional Display`: determine if the question is displayed based on the
  participant's answer to a previous question.
- :guilabel:`Show Comments Field`: allow the participant to type a comment in a text box.
- :guilabel:`Question Time Limit`: for live session surveys, set a time limit for the question.

Conditional Display
*******************

:guilabel:`Conditional Display` means the question is only displayed if the specified conditional
answer has been selected in a previous question.

When the box next to :guilabel:`Conditional Display` is selected, the :guilabel:`Triggering
Question` field appears. Select a question from the survey.

Then, a :guilabel:`Triggering Answer` field appears. Here, select which answer will trigger this
:guilabel:`Conditional Display` question.

Options tab
===========

Back on the main survey template form, under the :guilabel:`Options` tab, there are different
sections of settings that can be modified.

The sections include:

- :guilabel:`Questions`: focuses on the overall presentation of the survey
- :guilabel:`Scoring`: decides how the survey is scored
- :guilabel:`Candidates`: manages access to the survey
- :guilabel:`Live Session`: enables the survey into a real-time group activity.

Questions
---------

First, select the :guilabel:`Layout` of the survey. The following options can be chosen:

- :guilabel:`One page with all the questions`
- :guilabel:`One page per section`
- :guilabel:`One page per question`

If either the :guilabel:`One page per section` or :guilabel:`One page per question` options are
chosen, then the :guilabel:`Back Button` option appears. If selected, the :guilabel:`Back Button`
option allows the participant to go back to a question during the survey.

Under the :guilabel:`Layout` options is the :guilabel:`Progression Mode` setting, which indicates
how the participant's progress during the survey is displayed. It is shown as either a
:guilabel:`Percentage` or a :guilabel:`Number`.

Next, there is an option available to add a :guilabel:`Survey Time Limit`. To implement this
option, simply check the box, and enter the amount of time (in minutes) participants have to
complete the survey.

After the :guilabel:`Survey Time Limit` option is a section labeled :guilabel:`Selection`. Here,
questions can be :guilabel:`Randomized per section`, in other words, the number of random questions
can be configured by section. This mode is ignored in a live session.

.. seealso::
   :doc:`time_random`

Scoring
-------

The following options are available when deciding how a :guilabel:`Scoring` method:

- :guilabel:`No scoring`
- :guilabel:`Scoring with answers at the end`
- :guilabel:`Scoring without answers at the end`

If either the :guilabel:`Scoring with answers at the end` or :guilabel:`Scoring without answers at
the end` options are selected, a :guilabel:`Success %` field appears. Set the percentage of correct
answers needed to pass the survey.

Next, there is the option to make the survey a certification. To do so, check the box next to the
option labeled :guilabel:`Is a Certification`, and two additional fields appear. Select a color
theme in the :guilabel:`Certification Template` field and then choose an :guilabel:`Email
Template`. When a participant passes the certification with the required score, an email from Odoo
will automatically be sent to that person using the selected email template.

If the :guilabel:`Give Badge` feature is enabled and the :guilabel:`Certification Badge` is set,
the survey participant also receives a badge upon passing the certification.

.. seealso::
   :doc:`scoring`

Candidates
----------

To determine access to the survey, the :guilabel:`Access Mode` has two options to choose between:
:guilabel:`Anyone with the link` and :guilabel:`Invited people only`.

Below the :guilabel:`Appraisal Managers Only` checkbox is the :guilabel:`Login Required` option to
require a login to participate in the survey. If this option is activated, an :guilabel:`Attempts
Limit` field also populates, in which the number of survey attempts is defined for the participant.

Live Session
------------

The :guilabel:`Live Session` section is dedicated to users who are conducting surveys in real-time,
wherein they directly engage with and collect answers from a live audience.

Customize the :guilabel:`Session Code` here; this code is needed for participants to access the
live session survey. Reward participants for quick answers by selecting the checkbox labeled
:guilabel:`Reward quick answers`. By checking it, attendees will get more points if they answer
quickly.

Description tab
===============

Back on the main survey template page is the :guilabel:`Description` tab, where a custom
description of the survey can be added. This is displayed beneath the title on the survey's
homepage, which is on the front end of the website made through the Odoo :guilabel:`Website` app.

Test and share the survey
=========================

Once the survey is created and saved, run a test to check for possible errors before finally
sending it out to the participants by clicking :guilabel:`Test` in the upper left corner of the
survey template page.

When activated, Odoo redirects the page to a test version of the survey on the front end of the
website. This page displays how the survey will look to participants. Proceed to run through the
survey, like a normal participant, to check for errors.

To return to the survey template form in the backend, simply click the :guilabel:`This is a test
survey. Edit Survey` link in the blue banner along the top of the page. Once Odoo redirects the
page to the survey template in the backend, make any further changes, as needed, before officially
sending the survey out to participants.

When the survey is ready to be shared with the audience, click the :guilabel:`Start Survey` button
in the upper-left corner of the survey template form. Then, click :guilabel:`Share`.

In the pop-up window, add the survey recipients in the :guilabel:`Recipients` field (for existing
contacts in the Odoo database) or the :guilabel:`Additional emails` field (for contacts that do not
want to be listed in the Odoo database). Finally, click :guilabel:`Send`.

As answers are received, check them by clicking the :guilabel:`Answers` smart button on the survey
template form, or the :guilabel:`See Results` button in the upper left corner. To end the survey,
click the :guilabel:`Close` button on the survey template form.