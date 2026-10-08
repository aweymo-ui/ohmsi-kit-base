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

__Oral History Multi-Speaker Interpretation-Kit__

This kit uses Whisper speech-to-text models and SpeechBrain _diarization_ (identifying _who is speaking when_) to turn oral history recordings into CSV transcripts of timestamped dialogue separated by speaker. Recordings are batch processed with a selection of scripts, tiered depending on the qualities of the original audio files. Each transcript can then be copy edited against its recording in a local workspace which is how the recording will appear on an [Oral History as Data](https://github.com/uidaholib/oral-history-collections-template) site. Keyboard shortcuts for playback, looping, speed and navigation streamline the copyediting process, while supplemental Python workflows batch correct repetitive and time consuming errors.

[GitHub Repository](https://github.com/Scholarly-Projects/ohmsi-kit)

<details class="section" markdown="1">
<summary><h2 id="purpose">Purpose</h2></summary>

**My intent in developing this audio to text toolkit continues to be:**

- Implementing free, open-source models for sustainability.
- Developing transparent, efficient digital interfaces to ensure cultural heritage workers can audit the audio to text model output for accuracy and preservation.
- Ensuring models don't require an API login or tokens, and run locally after their initial download for privacy.
- Making the toolkit freely available to other institutions facing similar challenges.

_Andrew Weymouth, Fall 2026._

</details>

<details class="section" markdown="1">
<summary><h2 id="Acknowledgements">Acknowledgements</h2></summary>

The transcript editing workspace is built from the [Oral History as Data collections template](https://github.com/uidaholib/oral-history-collections-template) by the CollectionBuilder contributors and University of Idaho Library Digital Initiatives, used under the MIT License with the contributors' permission; see [THIRD-PARTY-NOTICES.md](THIRD-PARTY-NOTICES.md). Transcription uses [Whisper](https://github.com/openai/whisper) and diarization uses [SpeechBrain](https://speechbrain.github.io/). The project logo is a collage adapted from _Tarjetas con Dibujos y Con Letras_ (Crane, 1975), a set of instructional ESL learning cards, used here under fair use for educational and non-commercial purposes. Special thanks to Digital Project Managers Maryelizabeth Koepele and Jack Kredell for their contributions to the project.

</details>

<details class="section" markdown="1">
<summary><h2 id="background">Background</h2></summary>

This kit was developed over time to facilitate the transcription of the [Latah County Oral History Collection](https://www.lib.uidaho.edu/digital/lcoh/), an initiative conducted in the 1970's by the Latah County Historical Society and later digitized by the University of Idaho's [Center for Digital Inquiry and Learning](https://cdil.lib.uidaho.edu/) (CDIL) in 2015. The author developed this kit to transcribe the over 550 hour collection over the spring and summer of 2026 to make the material more discoverable for researchers and to provide the Latah County community with more transparent access to their history.

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