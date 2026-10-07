---
title: Home
layout: page
---

<div class="hero-logo-wrap">
  <img src="{{ '/images/ohmsi_logo.png' | relative_url }}" class="hero-logo"
       alt="Opticolumn logo of a lighthouse on top of a book with the sea in the distance.">
</div>

<details class="section" markdown="1" open>
<summary><h2 id="overview">Overview</h2></summary>

The Opticolumn Toolkit is a series of scripts developed to embed more accurate, consistent and efficient Optical Character Recognition (OCR) into a wide variety of archival documents.

<details class="section" markdown="1">
<summary><h2 id="purpose">Purpose</h2></summary>

**My intent in developing this OCR toolkit continues to be:**

- Implementing free, open-source models for sustainability.
- Bypassing large language models for text recognition to avoid vulnerability to hallucination and favor consistent, reproducible output for preservation.
- Ensuring models don't require an API login or tokens, and run locally after their initial download for privacy.
- Achieving a significant improvement in the accuracy of both typed and handwritten text materials.
- Keeping file size growth relatively minimal (5–15 percent), with the addition of the OCR layer.
- Ensuring that processed files meet the WCAG 2.1 and PDF/A standards for nested archival materials.
- Making the toolkit freely available to other institutions facing similar challenges.

_Andrew Weymouth, Fall 2026._

</details>

<details class="section" markdown="1">
<summary><h2 id="tools">Tools</h2></summary>

The Opticolumn Toolkit includes the following resources and applications:

- [Opticolumn](https://github.com/Scholarly-Projects/opticolumn)
    - Intended for archival scans and designed for type, handwritten text, cursive or a combination of all three. The tool can handle unorthodox arrangements of text, such as annotations and marginalia, but its reading order identification is not as developed as the following script.
- [Opticolumns](https://github.com/Scholarly-Projects/opticolumns)
    - Intended for archival scans of large-scale, multi-columned materials, such as newspapers.
- [Opticolumn_Editor](https://github.com/Scholarly-Projects/opticolumn_editor) (repository private until the completion of 2026 grant project)
    - Creates OCR using Opticolumn and produces a CSV of the OCR text that can be edited and processed again to incorporate copy edits into the final embedded layer. This method is recommended if you need OCR that surpasses Opticolumn benchmarks detailed in the [OSF Repository for Post-Processing OCR Accuracy Survey](https://osf.io/9f483/overview){:target="_blank" rel="noopener"}.
- _Forthcoming_:
    - An Optical Music Recognition tool, to make the library's International Jazz Collection and digitized sheet music fully accessible.

_Step-by-step instructions for installing and running these scripts are included in each tool's setup.md file._

</details>

<details class="section" markdown="1">
<summary><h2 id="about">About</h2></summary>

- [Transparent Practices: OCR and AI in the Archives, published in _Collections: A Journal for Museum and Archives Professionals_, June 2026](https://journals.sagepub.com/doi/full/10.1177/15501906261439241){:target="_blank" rel="noopener"}
- [OSF Repository for Post-Processing OCR Accuracy Survey](https://osf.io/9f483/overview){:target="_blank" rel="noopener"}
- [Presentation Site for the Fall 2026 Renfrew Colloquium on the Project](https://aweymo-ui.github.io/practices-rc/){:target="_blank" rel="noopener"}
- [Slide Deck for the Presentation](https://indd.adobe.com/view/a5ed9089-f1ec-4962-905a-75fb99c9f259){:target="_blank" rel="noopener"}
- [Presentation Recording](https://www.youtube.com/watch?v=8a54gpxjTPE){:target="_blank" rel="noopener"}

</details>

<details class="section" markdown="1">
<summary><h2 id="background">Background</h2></summary>

The Opticolumn Toolkit was developed while overhauling the [University of Idaho Library's](https://www.lib.uidaho.edu/) [digital collections](https://www.lib.uidaho.edu/digital/) to make the collection more discoverable and accessible. The development of the original [Opticolumn](https://github.com/Scholarly-Projects/opticolumn) tool is written about in greater detail in [_Transparent Practices: OCR and AI in the Archives_](https://journals.sagepub.com/doi/full/10.1177/15501906261439241) by Rebecca Hastings and Andrew Weymouth, _Collections: A Journal for Museum and Archives Professionals_, June 2026.

</details>

<details class="section" markdown="1">
<summary><h2 id="author">Author</h2></summary>

[Andrew Weymouth](https://aweymo.github.io/base/) is an Assistant Professor with the University of Idaho and the digital initiatives librarian for the Digital Scholarship and Open Strategies department. He focuses on using static web hosting to curate the institution’s special collections and develops digital tools and workflows to enhance transcription, tagging, and image processing to make the university’s media, text, and visual resources more discoverable for researchers. He is completing an MA in history at U of I under the supervision of Dr. Rebecca Scofield, focusing on pageantry and speculation in the Inland Empire.

</details>

------

{% include template/credits.html %}

<script>
  // Open a collapsed section when its nav link (or a #hash URL) targets it
  function openTargetSection() {
    var el = document.getElementById(decodeURIComponent(location.hash.slice(1)));
    if (el) {
      var d = el.closest('details');
      if (d) d.open = true;
    }
  }
  window.addEventListener('hashchange', openTargetSection);
  openTargetSection();
</script>