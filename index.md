---
title: WAI-ARIA Overview
permalink: /standards-guidelines/aria/
layout: default
github:
  repository: w3c/wai-intro-aria
feedbackmail: wai@w3.org
footer: |
  <p><strong>Date:</strong> Updated 19 May 2022. First published December 2006.</p>
  <p><strong>Editors:</strong> James Nurthen, <a href="https://www.w3.org/People/cooper/">Michael Cooper</a>, <a href="https://www.w3.org/People/shawn/">Shawn Lawton Henry</a>.</p>
  <p>Developed with input from the Accessible Rich Internet Applications Working Group (<a href="https://www.w3.org/WAI/ARIA/">ARIA WG</a>) and the Education and Outreach Working Group (<a href="https://www.w3.org/WAI/EO/">EOWG</a>).</p>
---

{::nomarkdown}
{% include box.html type="start" h="2" title="Summary" class="full" %}
{:/}

This page introduces the WAI-ARIA, the Accessible Rich Internet Applications suite of web standards.

Quick links to resources:
* [WAI-ARIA standard](/TR/wai-aria/)
* [WAI-ARIA Authoring Practices Guide (APG)](/WAI/ARIA/apg)
<!-- * [FAQ](/WAI/ARIA/faq) - including [What is the current status of WAI-ARIA development?](/WAI/ARIA/faq#update) -->

{::nomarkdown}
{% include box.html type="end" %}
{:/}

{::options toc_levels="2" /}

{::nomarkdown}
{% include_cached toc.html type="start" title="Page Contents" %}
{:/}

-   TOC is created automatically.
{:toc}

{::nomarkdown}
{% include_cached toc.html type="end" %}
{:/}

## Introduction

**WAI-ARIA, the Accessible Rich Internet Applications Suite, defines a
way to make Web content and Web applications more accessible to people
with disabilities. It especially helps with dynamic content and advanced
user interface controls developed with HTML, JavaScript, and
related technologies.** Without WAI-ARIA certain functionality used in Web
sites is not available to some users with disabilities, especially
people who rely on screen readers and people who cannot use a mouse.
WAI-ARIA addresses these accessibility challenges, for example, by
defining ways for functionality to be provided to assistive
technology. With WAI-ARIA, developers can make advanced Web applications
accessible and usable to people with disabilities.

This page describes the problems that WAI-ARIA addresses, and introduces
the WAI-ARIA suite of technical documents. Many of the terms used in
this page—including *Web content*, *user agent*s, and *assistive
technology*—are described in [Introduction to Web
Accessibility]({{ "/fundamentals/accessibility-intro/" | relative_url}}) and [Essential Components
of Web Accessibility]({{ "/fundamentals/components/" | relative_url }}).

### Technical Solutions

WAI-ARIA provides a framework for adding attributes
to identify features for user interaction, how they relate to each
other, and their current state. WAI-ARIA describes navigation
techniques to mark regions and common Web structures as menus, primary
content, secondary content, banner information, and other types of Web
structures. For example, with WAI-ARIA, developers can identify regions
of pages and enable keyboard users to easily move among regions, rather
than having to press Tab many times.

WAI-ARIA also includes technologies to map controls, live regions,
and events to accessibility application programming interfaces (APIs),
including custom controls used for rich Internet applications. WAI-ARIA
techniques apply to widgets such as buttons, drop-down lists, calendar
functions, tree controls (for example, expandable menus), and others.

WAI-ARIA provides Web authors with the following:

-   Roles to describe the type of widget presented, such as "menu",
    "treeitem", "slider", and "progressbar"
-   Roles to describe the structure of the Web page, such as headings,
    regions, and tables (grids)
-   Properties to describe the state widgets are in, such as "checked"
    for a check box, or "haspopup" for a menu.
-   Properties to define live regions of a page that are likely to get
    updates (such as stock quotes), as well as an interruption policy
    for those updates—for example, critical updates may be presented in
    an alert dialog box, and incidental updates occur within the page
-   A way to provide keyboard navigation for the Web objects and events,
    such as those mentioned above

## Authoring Practices Guide (APG)

**[ARIA Authoring Practices Guide (APG)](/WAI/ARIA/apg)**, recommends approaches to help web application developers make widgets, navigation, and behaviors accessible using WAI-ARIA roles, states, and properties.

It describes considerations that might not be evident to most authors from the WAI-ARIA specification, which is oriented primarily at user agent implementers.

## Versions {#versions}

* [WAI-ARIA 1.0](/TR/wai-aria/) was published as a completed W3C
Recommendation on 20 March 2014.

* [WAI-ARIA 1.1](/TR/wai-aria-1.1/) was published as a completed W3C
Recommendation on 14 December 2017.

* [WAI-ARIA 1.2](/TR/wai-aria-1.2/) is under development.

<!-- The latest status is updated in the [FAQ: What is the current status of
WAI-ARIA development?](/WAI/aria/faq#update) -->

### WAI-ARIA 1.2 {#wai-aria-1_2}

The 1.2 version will extend WAI-ARIA 1.1 to provide a small number of
features to complete the HTML + ARIA accessibility model. For 1.2, user 
agent implementation guidance is provided as a suite of accessibility 
API mapping specifications that describe how to expose semantics of 
WAI-ARIA and other web content languages to accessibility APIs.

Published WAI-ARIA 1.2 Working Drafts are as follows:

-   **[WAI-ARIA 1.2](/TR/wai-aria-1.2/) technical specification**,
    provides features to define accessible user interface elements and
    in order to improve the accessibility and interoperability of web
    content and applications. It is primarily for developers of Web
    browsers, assistive technologies, and other user agents; developers
    of Web technologies (technical specifications); and developers of
    accessibility evaluation tools.
-   **[Core Accessibility API Mappings 1.2](/TR/core-aam-1.2/)**,
    describes how user agents should expose semantics of web content
    languages to accessibility APIs. The core module defines support
    that applies across multiple content technologies, including general
    keyboard navigation support and mapping of general-purpose WAI-ARIA
    features; other specifications will extend this for specific
    technologies.
-   **[Accessible Name and Description: Computation and API Mappings
    1.2](/TR/accname-1.2/)**, describes how user agents determine
    names and descriptions of accessible objects from web content
    languages and expose them in accessibility APIs. This allows
    assistive technologies to associate and relay the name or
    description of objects to users.
-   **[HTML Accessibility API Mappings 1.0](/TR/html-aam-1.0/)**,
    extends Core Accessibility API Mappings 1.2 and Accessible Name and
    Description: Computation and API Mappings 1.2 to define how user
    agents map HTML markup to platform accessibility application
    programming interfaces (APIs). Provides HTML-specific guidance for
    how the HTML user agent must respond to keyboard focus, native HTML
    features, and role, state and property attributes provided via
    WAI-ARIA.
-   **[SVG Accessibility API Mappings 1.0](/TR/svg-aam-1.0/)**, extends
    Core Accessibility API Mappings 1.2 to define how user agents map
    SVG markup to platform accessibility application programming
    interfaces (APIs). When supported by user agents, its features allow
    SVG authors to create accessible rich internet applications,
    including charts, graphs, and other drawings. Provides SVG-specific
    guidance for how the SVG user agent must respond to keyboard focus,
    native SVG features, and role, state and property attributes
    provided via WAI-ARIA.

Additional documents are expected in this suite, including other
accessibility API mappings and updated authoring guidance. Editors'
drafts under development can be accessed in the [WAI-ARIA GitHub
Repository](https://github.com/w3c/aria/).

*W3C Recommendations* and *Working Group Notes* are briefly explained in
[How WAI Develops Accessibility Guidelines through the W3C
Process](/WAI/intro/w3c-process), which also describes milestones in the
W3C Process.

### Technical document format

The WAI-ARIA documents follow the W3C format for technical
specifications which includes several sections at the beginning: links
to different versions, editors, copyright, abstract, and status with the
link to errata and the email address for comments.

## Who develops WAI-ARIA

The WAI-ARIA technical documents are developed by the Accessible Rich
Internet Applications Working Group ([ARIA WG](/WAI/ARIA/)), which is
part of the World Wide Web Consortium ([W3C](/)) Web Accessibility
Initiative ([WAI](/WAI/)). For more information about the working group,
see the [ARIA WG public page](/WAI/ARIA/).

[How WAI Develops Accessibility Guidelines through the W3C Process:
Milestones and Opportunities to Contribute](/WAI/intro/w3c-process)
describes formal periods for public review. Opportunities for review and
comment of WAI documents are announced on the [WAI home page](/WAI/) and
[WAI Interest Group](/WAI/IG/) mailing list. An email address for
sending comments is included in the "Status of this Document" section.

Opportunities for contributing to WAI-ARIA and other WAI work are
introduced in [Participating in WAI](/WAI/participation).
