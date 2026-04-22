.. _games_block:

.. This topic is used in both the edX and Open edX versions of the
   Building and Running a Course guide.

##############
Games Block
##############

The Games block allows course authors to create interactive learning activities
using either **Flashcards** or a **Matching** game. These activities support
retrieval practice and can be used to reinforce key concepts within a course.

.. contents::
  :local:
  :depth: 1

*************************************
Adding a Games Block to Your Course
*************************************

To add a Games block:

#. Open a **Unit page** in Studio.
#. Scroll to the bottom of the Unit page.
#. Select **Games**.

.. image:: ../../../shared/images/games_add_component.png
   :alt: The Add New Component area in Studio, showing the Games component
     button with a trophy icon and a Beta label.
   :width: 600

The Games block opens in the **Flashcards editor** by default.

*******************
Flashcards Editor
*******************

In the Flashcards editor, you can:

* Enter **terms** and **definitions**.
* Add **images** to terms or definitions.
* Drag cards to reorder them using the drag handle on the left.
* Expand or collapse individual cards.

.. image:: ../../../shared/images/flashcards_editor_expanded.png
   :alt: The Flashcards editor in Studio with a card expanded, showing fields
     for a term with an image and a definition. The Settings panel on the right
     shows Type set to Flashcards and Shuffle set to On.
   :width: 600

.. image:: ../../../shared/images/flashcards_editor_collapsed.png
   :alt: The Flashcards editor in Studio with multiple cards in collapsed view,
     showing numbered cards with term-definition pairs and image thumbnails.
   :width: 600

Using the Three-Dot Menu
========================

Use the **three-dot menu** (``...``) on each card to:

* Move the card up.
* Move the card down.
* Delete the card.

.. image:: ../../../shared/images/flashcards_three_dot_menu.png
   :alt: The three-dot menu on a flashcard, showing options to Move up, Move
     down, and Delete.
   :width: 600

Adding Alt Text for Images
===========================

To add alt text for images:

#. Expand the card.
#. Select the image.
#. Enter alt text in the **Alt Text** field.
#. Select **Save**.

.. image:: ../../../shared/images/flashcards_image_alt_text.png
   :alt: The Image Settings dialog in the Flashcards editor, showing a
     preview of the image, an Alt Text field, and a checkbox to mark the image
     as decorative.
   :width: 600

Flashcards Settings
====================

From the **Settings** panel on the right side of the editor, you can:

* Switch between **Flashcards** and **Matching** game types.
* Enable or disable **Shuffle**.

When Shuffle is enabled, the order of terms and definitions appears randomly
to learners.

.. image:: ../../../shared/images/flashcards_settings_panel.png
   :alt: The Settings panel showing a Type dropdown with Flashcards selected
     and a Shuffle toggle set to On.
   :width: 300

*************************
Flashcards Studio View
*************************

To preview Flashcards in Studio:

#. Select **Start**.

.. image:: ../../../shared/images/flashcards_studio_start.png
   :alt: The Flashcards component in Studio preview mode, showing the title
     Flashcards, the instruction text Click each card to reveal the definition,
     and a Start button.
   :width: 600

You will see:

* The term displayed on the card.
* The card number at the bottom of the screen.

Click anywhere on the card to reveal the definition. This interaction matches
the learner experience in the LMS.

.. image:: ../../../shared/images/flashcards_studio_definition.png
   :alt: A flashcard in preview mode showing the definition side of the card
     with the text panama city and navigation arrows with card counter 6 of 7
     at the bottom.
   :width: 600

.. image:: ../../../shared/images/flashcards_studio_term.png
   :alt: A flashcard in preview mode showing the term side of the card with
     an image and the text capital of panama, with navigation arrows and card
     counter 6 of 7 at the bottom.
   :width: 600

Use the arrows to move between cards.

***********************
Matching Game Editor
***********************

To create a Matching game:

#. Select **Settings**.
#. Select **Matching** from the **Type** dropdown.

Matching games use the same term-definition structure as Flashcards.

Matching games:

* Do **not** support images.
* Include an optional **timer**.

You can enable or disable the timer from the Settings panel.

.. image:: ../../../shared/images/matching_settings_panel.png
   :alt: The Settings panel for a Matching game, showing Type set to Matching,
     Shuffle set to On, and Timer set to On.
   :width: 300

*******************************
Studio View for Matching Game
*******************************

To preview the Matching game:

#. Select **Start**.

.. image:: ../../../shared/images/matching_studio_start.png
   :alt: The Matching game component in Studio preview mode, showing the title
     Matching, the instruction text Match each term with the correct definition,
     and a Start button.
   :width: 600

In the Matching game:

* Terms appear on the left.
* Definitions appear on the right.

.. image:: ../../../shared/images/matching_game_board.png
   :alt: The Matching game board showing terms on the left and definitions on
     the right, with a timer counting down at the bottom.
   :width: 600

When a correct match is made:

* The match is highlighted in **green**.
* The matched pair disappears.

.. image:: ../../../shared/images/matching_correct_selection.png
   :alt: The Matching game showing a correct match highlighted in green, with
     the selected term highlighted on the left.
   :width: 400

When an incorrect match is made:

* The selection is highlighted in **red**.
* The choices remain visible.

.. image:: ../../../shared/images/matching_incorrect_selection.png
   :alt: The Matching game showing an incorrect match highlighted in red, with
     both the term and definition selections shown.
   :width: 400

Additional interface elements include:

* A timer at the bottom of the screen (if enabled).
* Helper text available by hovering over the question mark icon that reads:
  "Match each term with the correct definition".

After completing the game, learners see a **congratulations screen** with their
completion time, their personal best time, and an option to play again.

.. image:: ../../../shared/images/matching_congratulations.png
   :alt: The Matching game congratulations screen showing confetti,
     the completion time, the personal best time, and a Play again button.
   :width: 600
