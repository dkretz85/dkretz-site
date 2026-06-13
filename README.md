# dkretz.com — your site

A seven-page static site in the "index" direction. Self-contained: each page has
its CSS inlined, so any file renders correctly opened on its own — no separate
stylesheet to keep alongside it. No build step, no dependencies, nothing to maintain.

## Pages

- index.html — homepage (numbered index)
- about.html — about & research, with bio and languages (complete)
- publications.html — books, articles, reviews, translations (populated from your CV)
- talks.html — selected recent talks (full list points to the CV)
- teaching.html — courses as instructor of record and as TA (populated from your CV)
- contact.html — email is set to david.kretz@yale.edu; ORCID is optional
- 404.html — shown for bad URLs
- CNAME — tells GitHub Pages your custom domain is dkretz.com

## Before you publish — short list

1. Add your CV. Save it as a PDF named exactly cv.pdf and drop it in this folder.
   (The "Curriculum vitae" link and the "see the CV" notes point to it.)
2. ORCID on the contact page is the only optional placeholder left. Add it or
   delete the line.
3. Everything else is real content from your CV — read through and adjust voice
   or selection as you like. Talks and teaching are deliberately a selection;
   the CV carries the complete record.

## A note on what I included

I transcribed publications, talks, and teaching directly from
CV_DKretz_April_2026.pdf. I did not invent anything. Where I made an editorial
call — showing selected talks rather than all ~35, folding service/public-writing
into the CV rather than separate pages — you can change it.

## Editing

Each page is plain HTML with a <style> block at the top. To change wording, edit
the text between the tags. To restyle, edit the <style> block — note it's now
duplicated across pages (the trade-off for standalone files). If you'd rather go
back to one shared style.css, I can give you that version too.

## Publishing (GitHub Pages — free)

1. Buy dkretz.com from any registrar (Namecheap, Porkbun, Cloudflare ~€10–12/yr).
2. Create a GitHub account, then a new public repo named davidkretz.github.io.
3. Upload every file in this folder to that repo (drag-and-drop works).
4. Repo → Settings → Pages → Source: main branch, /root. Save.
5. Under "Custom domain", enter dkretz.com.
6. At your registrar's DNS, add:
   - Four A records for the apex (@): 185.199.108.153, 185.199.109.153,
     185.199.110.153, 185.199.111.153
   - One CNAME record: www → davidkretz.github.io
7. Wait for DNS to propagate, then tick "Enforce HTTPS" in Settings → Pages.

Netlify or Cloudflare Pages work equally well via drag-and-drop; set the domain
in their dashboard instead of using the CNAME file.
