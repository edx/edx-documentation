.. _Additional Video Options:

###################################
Specifying Additional Video Options
###################################

When you create a video component, you can customize additonal settings such as
specifying download options for the video and transcript, video license options,
a start and stop time for the video, and an audio description track for
accessibility.

.. contents::
  :local:
  :depth: 1

.. _Enable Video and Transcript Downloads:

********************************************
Enable Video and Transcript Downloads
********************************************

You can allow learners to download videos and transcript files that you have
provided so that they can view them offline.

To enable video and transcript downloads, follow these steps.

#. To allow learners to download the video, select **Allow video downloads**
   in the **Video Source** section.
#. To allow learners to download an .srt and .txt video transcript, select
   **Allow transcript downloads** in the **Transcript** section.
#. Select **Save**.

To test transcript downloads for the video, select **Download transcript** in
the video player’s control bar. You can download either the SubRip (.srt)
format or text (.txt) format.

.. _Video Settings:

**************************
Set Video Settings
**************************

.. contents::
  :local:
  :depth: 1

The following options appear on the **Edit** page of the video component.

.. list-table::
    :widths: 30 70

    * - **Component Display Name**
      - The name that you want your learners to see. To edit the display name,
        select the pencil icon inthe top left hand corner.

.. _Video Source:

===============
Video Source
===============

.. list-table::
    :widths: 30 70

    * - **Video ID**
      - The Video IDis the source for your video. Video IDs are the
        identifiers that the video process assigns to the video. Only courses on
        edx.org use Video IDs.

    * - **Video URL**
      - The Video URL is the source for your video. Video URLS are for externally
        hosted video.
  
    * - **Allow Video Downloads**
      - Specifies whether learners can download the video. If you select **Allow
        video downloads**, you must add at least one URL in the **Fallback
        Videos** field.

    * - **Fallback Videos**
      - The URL or URLs where you posted different versions of the video. If you
        added URLs by selecting **Add a video URL**, the URLs are listed in the
        fields below to **Fallback Videos**.

        Every URL must end in .mp4, .mpeg, .webm, or .ogg. Learners will view
        the first listed video that is compatible with their computer or mobile
        device.

        For the best experience for mobile users, make sure that the URL for
        the 360p version of the video is the first URL in the list.

        To help make sure all standard browsers can play your video, we
        **strongly** recommend that you use the .mp4 format.

.. _Thumbnail:

===============
Thumbnail
===============

.. note::
   **This feature is not available for Video components in Libraries.**

The thumbnail image is the image that learners see before the video begins to
play. For videos found on the **Video Uploads** page, the thumbnail image can be
specified. The thumbnail image should have an aspect ratio of 16:9.

To add a thumbnail to a video component, follow these steps:

#. Open the video component for the video.
#. Scroll down to the **Thumbnail** section, and then select **Upload
   Thumbnail**.
#. In the dialog box, browse to the image file, and then select **Open**.

To replace the current thumbnail, delete the thumbnail, and then follow the
steps above for adding a thumbnail

.. _Transcript:

============
Transcript
============

.. note::
   To test the transcript with the video, after you have saved the video, select
   **Show transcript** (”) icon in the video player's control bar. The transcript
   file scrolls while the file plays. You can also test the transcript by
   selecting the **CC** icon.

.. list-table::
    :widths: 30 70

    * - **Transcript Languages**
      - The transcript files for any additional languages. For more
        information, see :ref:`Transcripts in Additional Languages`.

    * - **Download Transcript Allowed**
      - Specifies whether you want to allow learners to download the .srt or
        .txt transcript. (By default, Studio creates a .txt transcript when you
        upload an .srt transcript.) If you select **Allow transcript
        downloads**, a link to download the file appears below the video.

        If you want to provide a downloadable transcript in a different format
        as well, such as .pdf, edX recommends that you upload a handout for learners by
        using the **Upload Handout** field. For more information, see
        :ref:`Additional Transcripts`.

    * - **Show Transcript by Default**
      - Specifies whether the transcript appears next to the video by default.
        If this is set to **unchecked**, learners can still view transcripts by
        selecting the **Show Transcript** (”) icon.

.. _Audio Description:

====================
Audio Description
====================

.. note::
   **This feature is not available for Video components in Libraries.** The
   Audio Description option only appears when your course administrator has
   enabled it for your course.

Audio description (AD) is a narrated audio track that describes the visual
content of a video — such as on-screen text, actions, scene changes, and
graphics — for learners who are blind or have low vision. Adding an audio
description track to your videos helps you meet
`WCAG 2.1 Success Criterion 1.2.5 (Audio Description) <https://www.w3.org/WAI/WCAG21/Understanding/audio-description-prerecorded.html>`_.

When a video has an audio description attached, learners see an **Audio
Description** toggle button in the video player controls. They can turn the
audio description on or off at any time during playback.

**Supported File Formats**

You can upload audio description files in the following formats:

* MP3 (.mp3)
* OGG (.ogg)
* M4A (.m4a)
* WAV (.wav)
* AAC (.aac)

The maximum file size is **200 MB**.

.. _Add an Audio Description:

Add an Audio Description
*************************

To add an audio description to a video component in Studio, follow these steps.

#. In Studio, navigate to the unit that contains the video component you want
   to update.

#. Select **Edit** on the video component to open the video editor.

#. In the video settings panel on the right, scroll down until you see the
   **Audio Description (AD)** collapsible section. If no audio description
   file has been uploaded yet, the section displays **None** below the title.

   .. image:: ../../../shared/images/AudioDescription_SectionCollapsedWithNone.png
      :alt: The Audio Description (AD) section in the video settings panel,
          shown in its collapsed state with the subtitle None, indicating that
          no audio description file has been uploaded.

   .. note::
      If you do not see the **Audio Description (AD)** section, the feature
      has not been enabled for your course. Contact your course administrator
      to enable it.

#. Select the **Audio Description (AD)** section header to expand it. The
   expanded section displays the message "Add an audio description track
   (MP3, OGG, M4A, WAV, or AAC) to provide narrated descriptions of visual
   content for learners who are blind or have low vision" and an
   **Upload Audio Description** button with an upload icon.

   .. image:: ../../../shared/images/AudioDescription_SectionExpand.png
      :alt: The expanded Audio Description (AD) section showing the heading
          Audio Description (AD), the help text describing supported audio
          formats, and the Upload Audio Description button with an upload
          icon at the bottom left.

#. Select the **Upload Audio Description** button. A file browser dialog
   opens.

#. In the file browser, locate and select the audio description file you have
   prepared for this video. The file must be one of the supported formats
   (MP3, OGG, M4A, WAV, or AAC) and must not exceed 200 MB.

   If you select a file with an unsupported format, Studio displays an error
   message indicating which formats are accepted.

   .. image:: ../../../shared/images/AudioDescription_FileTypeError.png
      :alt: The Audio Description (AD) section showing an error banner that
          reads Only MP3, OGG, M4A, WAV, and AAC files are supported for
          audio descriptions, with a Dismiss button.

   If you select a file that exceeds 200 MB, Studio displays an error message
   indicating that the file is too large.

   .. image:: ../../../shared/images/AudioDescription_FileSizeError.png
      :alt: The Audio Description (AD) section showing an error banner that
          reads Audio description files must be 200 MB or less, with a
          Dismiss button.

   You can select **Dismiss** to close either error message and try again
   with a valid file.

#. Select **Open** (or **Choose**, depending on your browser) to begin the
   upload.

   Studio shows a spinning progress indicator while the file uploads. When
   the upload completes, the file name appears in the **Audio Description
   (AD)** section alongside a **Delete** button, and a help message confirms
   that learners can toggle the audio description track using the player
   controls.

   .. image:: ../../../shared/images/AudioDescription_UploadComplete.png
      :alt: The Audio Description (AD) section after a successful upload,
          showing the uploaded file name file_example_MP3_5MG.mp3 in a
          bordered row with a Delete button on the right.

#. Select **Save** at the bottom of the video editor to save your changes.

After you save, the collapsed **Audio Description (AD)** section displays the
uploaded file name instead of **None**.

.. image:: ../../../shared/images/AudioDescription_SectionCollapsedWithFile.png
   :alt: The Audio Description (AD) section in its collapsed state showing
       the uploaded file name file_example_MP3_5MG.mp3 as the subtitle.

Learners who view this video will see an **Audio Description** toggle button
in the video player controls. When the audio description is active, the button
appears highlighted.

.. image:: ../../../shared/images/AudioDescription_PlayerToggleActive.png
   :alt: The learner video player controls showing the Audio Description
       toggle button in its active state, highlighted in yellow.

When the audio description is inactive, learners can select the button to turn
it on.

.. image:: ../../../shared/images/AudioDescription_PlayerToggleInactive.png
   :alt: The learner video player controls showing the Audio Description
       toggle button in its inactive state.

If no audio description file has been uploaded for the video, the toggle button
appears disabled and a tooltip displays **Audio description not available**
when learners hover over it.

.. image:: ../../../shared/images/AudioDescription_PlayerToggleDisabled.png
   :alt: The learner video player controls showing the Audio Description
       toggle button in a disabled state with a tooltip that reads Audio
       description not available.

.. tip::
   For the best learner experience, the audio description track should be
   approximately the same length as the video. Consider re-recording the
   description to match the video length if needed.

.. _Replace an Audio Description:

Replace an Audio Description
*****************************

To replace an existing audio description file with a new one, you must first
delete the current file and then upload the replacement.

#. In Studio, navigate to the unit that contains the video component.

#. Select **Edit** on the video component to open the video editor.

#. In the video settings panel, expand the **Audio Description (AD)** section.
   You will see the current audio description file name with a **Delete**
   button next to it.

   .. image:: ../../../shared/images/AudioDescription_UploadComplete.png
      :alt: The Audio Description (AD) section showing the current file name
          and the Delete button next to it.

#. Select **Delete** to remove the current audio description file.

#. Select **Upload Audio Description** and choose the new audio description
   file from your computer.

#. After the upload completes and the new file name appears, select **Save**.

.. _Delete an Audio Description:

Delete an Audio Description
****************************

To remove the audio description from a video component, follow these steps.

#. In Studio, navigate to the unit that contains the video component.

#. Select **Edit** on the video component to open the video editor.

#. In the video settings panel, expand the **Audio Description (AD)** section.

#. Select **Delete** next to the audio description file name.

   The file name disappears, and the **Upload Audio Description** button
   reappears.

   .. image:: ../../../shared/images/AudioDescription_SectionExpand.png
      :alt: The Audio Description (AD) section after deletion, showing the
          Upload Audio Description button with no file attached.

#. Select **Save** to save your changes.

After you save, the **Audio Description** toggle button will no longer appear
in the learner's video player for that video.

.. _Duration:

===============
Duration
===============

.. note::
   To keep the full length of the video, both the start and stop time should be
   set to 00:00:00.

.. list-table::
    :widths: 30 70

    * - **Video Start Time**
      - The time you want the video to start if you do not want the entire
        video to play. Use HH:MM:SS format. The maximum value is 23:59:59.

        .. note::
           Learners who play video in the mobile app see the entire video file.
           Only videos that play in a browser start playing at the specified
           start time.

    * - **Video Stop Time**
      - The time you want the video to stop if you do not want the entire video
        to play. Use HH:MM:SS format. The default value is 00:00:00 if you do
        not specify an end time. 00:00:00 is equal to the end of the video. The
        maximum value is 23:59:59.

        .. note::
           Learners who play video in the mobile app see the entire video file.
           Only videos that play in a browser stop playing at the specified
           stop time.

.. _Handout:

==============
Handout
==============

.. note::
   **This feature is not available for Video components in Libraries.**

.. list-table::
    :widths: 30 70

    * - **Upload Handout**
      - Allows you to upload a handout to accompany the video, such as a PDF
        transcript or other handout. Learners can download the handout by
        selecting **Download Handout** under the video. The procedure for
        adding handouts is the same as the procedure for adding a supplemental
        transcript. For more information, see :ref:`Additional Transcripts`.

.. _License:

===============
License
===============

.. note::
   The license defaults to the license set at the course level

.. list-table::
    :widths: 30 70

    * - **License**
      - Optionally, you can set the license for the video, if you want to
        release the video with a license different from the overall course
        license.

        * Select **All Rights Reserved** to indicate to learners that you own
          the copyright for the video.

        * Select **Creative Commons** to grant others the right to share and
          use the video. You must then select the Creative Commons license
          options that you want.

          The license options that you select control the copyright notice that
          learners see for the video. For more information, see :ref:`Licensing
          a Course`.
