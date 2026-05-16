---
title: 'Skills and Awards'
date: 2023-10-24
type: landing

design:
  spacing: '1rem'

# Note: `username` refers to the user's folder name in `content/authors/`

# Page sections
sections:
  - block: resume-experience
    content:
      username: me
      title: Leadership & Student Support
      show_education: false
    design:
      # Hugo date format
      date_format: 'January 2006'
      # Education or Experience section first?
      is_education_first: false
  - block: resume-skills
    content:
      title: Skills & Hobbies
      username: me
  - block: resume-awards
    content:
      title: Awards
      username: me
  - block: resume-languages
    content:
      title: Languages
      username: me
---

<!-- Page-specific script: rename Experience heading and remove Education section on this page only -->
<script>
document.addEventListener('DOMContentLoaded', function () {
  try {
    // Rename top 'Experience' heading if present
    var headings = document.querySelectorAll('h1, h2, h3');
    for (var i = 0; i < headings.length; i++) {
      var t = headings[i].textContent && headings[i].textContent.trim();
      if (!t) continue;
      if (t.toLowerCase() === 'experience') {
        headings[i].textContent = 'Leadership & Student Support';
        break;
      }
    }

    // Find and remove the Education section by locating its heading
    var allHeadings = document.querySelectorAll('h1, h2, h3, h4');
    for (var j = 0; j < allHeadings.length; j++) {
      var txt = (allHeadings[j].textContent || '').trim();
      if (txt.toLowerCase() === 'education') {
        var sec = allHeadings[j].closest('section') || allHeadings[j].parentElement;
        if (sec) sec.remove();
        break;
      }
    }
  } catch (e) {
    console.warn('Page script error:', e);
  }
});
</script>