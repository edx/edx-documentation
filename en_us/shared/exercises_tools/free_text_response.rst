.. _Free Text Response:

.. This topic is used in both the edX and Open edX versions of the
   Building and Running a Course guide.

##################
Free-text Response
##################

The **Free-text Response** component allows learners to respond to an
open-ended question or prompt directly within a course.

Course teams can use Free-text Response for reflection, short-form peer
engagement, and other activities where learners are asked to express an idea
in their own words. Course teams can also allow learners to view responses
submitted by other learners after submitting their own response.

For example, you might ask learners to reflect on a concept from a video,
share an example from their own experience, or respond to a question before
seeing how other learners responded.

.. contents::
  :local:
  :depth: 1

************************************************
The Learner View of a Free-text Response
************************************************

Learners see the question or prompt configured by the course team and enter
their response in a text field.

Depending on how the component is configured, learners can:

* Enter and submit a written response.
* Save a draft response.
* Submit a response within a specified minimum or maximum word count.
* View responses submitted by other learners after submitting their own
  response.

When **Display Other Student Responses** is enabled, Free-text Response can be
used as a lightweight peer-engagement activity. Learners first formulate and
submit their own response and can then see how other learners responded to the
same prompt.

This can be useful for reflection and peer learning activities that do not
require a full discussion.

************************************************
Create a Free-text Response
************************************************

To add a Free-text Response component to a course:

#. From the **Course Outline** page, locate the unit where you want to add the
   activity.
#. Under the unit, select **+ Add component**.

   .. image:: ../../../shared/images/free_text_response_add_component.png
      :alt: The bottom of a unit page in Studio, showing existing components
        and the Add component button.
      :width: 600

#. Select **Free-text Response**.
#. In the new component that appears, select **Edit**.

   .. image:: ../../../shared/images/free_text_response_component.png
      :alt: A Free-text Response component on a unit page in Studio, with the
        Edit button.
      :width: 600

The Free-text Response editor opens.

************************************************
Configure the Question
************************************************

Use the following fields to configure the question that learners see.

============
Display Name
============

The **Display Name** is the name of the component displayed in Studio.

The default display name is **Free-text Response**. It is recommended that you
change the display name to describe the activity or question more
specifically.

======
Prompt
======

The **Prompt** is the question or instruction presented to learners.

Use this field to explain what you want learners to respond to.

For example:

  Think about the concept introduced in the previous video. How might you
  apply this concept in your own work?

When you have finished configuring the fields, select **Save** to save your
changes.

.. image:: ../../../shared/images/free_text_response_editor_question.png
   :alt: The Free-text Response editor in Studio showing the Display Name and
     Prompt fields.
   :width: 600

************************************************
Configure Attempts and Correctness
************************************************

The Free-text Response editor includes additional settings that determine how
the activity behaves.

======
Weight
======

**Weight** assigns an integer value representing the weight of the problem.

For an activity that is being used for reflection or peer engagement rather
than assessment, you can use a weight of ``0``.

==========================
Maximum Number of Attempts
==========================

**Maximum Number of Attempts** determines the maximum number of times a learner
is allowed to attempt the activity.

===================
Display Correctness
===================

**Display Correctness** determines whether a correctness indicator is
displayed after a learner submits a response.

You can set **Display Correctness** to either:

* **True** -- Displays the correctness indicator. This is the default setting.
* **False** -- Does not display the correctness indicator.

For reflection or peer-engagement activities where there is no correct or
incorrect response, set **Display Correctness** to **False**.

.. image:: ../../../shared/images/free_text_response_editor_attempts.png
   :alt: The Free-text Response editor in Studio showing the Weight, Maximum
     Number of Attempts, and Display Correctness fields.
   :width: 600

************************************************
Configure Response Length and Key Phrases
************************************************

You can configure requirements for the length and content of learner
responses.

==================
Minimum Word Count
==================

**Minimum Word Count** specifies the minimum number of words required in a
learner's response.

==================
Maximum Word Count
==================

**Maximum Word Count** specifies the maximum number of words allowed in a
learner's response.

========================
Full-Credit Key Phrases
========================

**Full-Credit Key Phrases** specifies a list of words or phrases, one of which
must be present for the learner's response to receive full credit.

For an open-ended reflection or peer-engagement activity that is not assessed,
this field can be left empty.

.. image:: ../../../shared/images/free_text_response_editor_word_count.png
   :alt: The Free-text Response editor in Studio showing the Minimum Word
     Count, Maximum Word Count, and Full-Credit Key Phrases fields.
   :width: 600

========================
Half-Credit Key Phrases
========================

**Half-Credit Key Phrases** specifies a list of words or phrases, one of which
must be present for the learner's response to receive half credit.

For an open-ended reflection or peer-engagement activity that is not assessed,
this field can be left empty.

************************************************
Configure Submission Messages and Peer Responses
************************************************

You can configure what learners see when they save or submit their responses
and whether they can view responses from other learners.

===========================
Submission Received Message
===========================

**Submission Received Message** is the message learners see after submitting
their response.

The default message is:

  Your submission has been received

You can customize this message to provide additional instructions or context
after submission.

.. image:: ../../../shared/images/free_text_response_editor_submission_message.png
   :alt: The Free-text Response editor in Studio showing the Half-Credit Key
     Phrases and Submission Received Message fields.
   :width: 600

================================
Display Other Student Responses
================================

**Display Other Student Responses** determines whether learners can view
responses submitted by other learners after submitting their own response.

Enable this setting when you want to use Free-text Response as a
peer-engagement activity where learners benefit from seeing how other learners
responded to the same question.

======================
Draft Received Message
======================

**Draft Received Message** is the message learners see when they save a draft
response.

You can customize this message to clarify that the learner's response has been
saved but has not yet been submitted.

.. image:: ../../../shared/images/free_text_response_editor_peer_responses.png
   :alt: The Free-text Response editor in Studio showing the Submission
     Received Message, Display Other Student Responses, and Draft Received
     Message fields.
   :width: 600

************************************************
Create a Peer-Engagement Activity
************************************************

Free-text Response can be used to create a short-form peer-engagement activity
that does not need to be assessed or graded.

For example:

  What is one idea from this section that changed how you think about the
  topic? Explain why.

For this type of activity:

#. Enter the question in **Prompt**.
#. Set **Weight** to ``0``.
#. Set **Display Correctness** to **False**.
#. Leave **Full-Credit Key Phrases** and **Half-Credit Key Phrases** empty.
#. Set an appropriate **Minimum Word Count** and **Maximum Word Count**.
#. Enable **Display Other Student Responses** if you want learners to see their
   peers' responses after submitting their own response.
#. Select **Save**.

This configuration creates a lightweight reflection and peer-engagement
activity in which learners formulate their own response and can then compare
it with the perspectives of other learners.
