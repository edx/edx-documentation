.. _course_optimizer:

#################
Course Optimizer
#################

The **Course Optimizer** page is available in edX Studio from the **Tools**
dropdown menu, alongside **Import**, **Export**, and **Checklists**.

Use the Course Optimizer to scan your course for issues such as broken links,
broken images, and links that point to content from a previous course run.

****************************************
Scan for Broken Links and Images
****************************************

To scan your course:

#. Select **Tools**, then select **Course Optimizer**.

   From the **Course Outline** page, open the **Tools** menu and select **Course
   Optimizer**.

   .. image:: ../../../shared/images/course_optimizer_tools_menu.png
    :width: 600
    :alt: The Tools menu in Studio with Course Optimizer highlighted.

#. Select **Scan course**.

On the **Course Optimizer** page, select **Scan course** to start scanning
your course content for broken links and images.

.. image:: ../../../shared/images/course_optimizer_scan_page.png
 :width: 600
 :alt: The Course Optimizer page with the Scan course button.

The scan progresses through three stages:

* **Preparing**
* **Scanning**
* **Success**

Scan time depends on the size of your course.

.. image:: ../../../shared/images/course_optimizer_scan_progress.png
 :width: 600
 :alt: The Course Optimizer scan progress showing Preparing, Scanning, and
  Success stages.

After the scan completes, the results page displays any broken links, broken
images, and links that could not be verified.

Three icons indicate different types of link results:

* **Broken links**

  Links to external websites or images that no longer exist or cannot be
  reached. These links may prevent learners from accessing course content.

* **Unverified links**

  Links that cannot be automatically validated. Review these links manually.

* **Locked course file links**

  Links to course files that are inaccessible to non-enrolled users. These
  links cannot be verified automatically.

.. image:: ../../../shared/images/course_optimizer_scan_results.png
 :width: 600
 :alt: Scan results showing broken link counts for course content.

Use the available filters to refine the results list.

.. image:: ../../../shared/images/course_optimizer_filters.png
 :width: 600
 :alt: The Filters menu on the scan results page.

Expand any result to:

* open the block where the issue appears
* view the affected link directly

.. image:: ../../../shared/images/course_optimizer_expanded_result.png
 :width: 600
 :alt: An expanded scan result showing affected links in a course block.

********************************************
Update Links from a Previous Course Run
********************************************

The Course Optimizer also identifies links that still point to pages from a
previous course run.

If no issues are found, the page displays:

**No results found**

.. image:: ../../../shared/images/course_optimizer_no_previous_run_links.png
 :width: 600
 :alt: The Links to previous course run section showing No results found.

If outdated links are detected, you can:

* select **Update all** to update all links automatically
* update individual links manually as needed

.. image:: ../../../shared/images/course_optimizer_update_previous_run_links.png
 :width: 600
 :alt: Outdated links from a previous course run with Update all and individual
  Update buttons.

Updating these links ensures learners are directed to the correct content in
the current course run.
