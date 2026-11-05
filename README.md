# Brunch Club site: setup

1. Images go in /images (compress each to under 300 KB at squoosh.app):
   hero.jpg (still frame for the video), hero.mp4 (5s, under 3 MB), studio.jpg, linda.jpg,
   italy.jpg, guatemala.jpg, europe.jpg, latam.jpg, portfolio-1.jpg to portfolio-6.jpg
2. Convert the video: ffmpeg -i clip.mov -vf scale=1920:-2 -an -c:v libx264 -crf 28 -preset slow -movflags +faststart hero.mp4
3. Form: create a free key at web3forms.com with the studio email, paste it in inquire.html (PASTE_WEB3FORMS_KEY).
4. Copy: edit all text in i18n.js (en, es, it). Brand colors: the :root block at the top of style.css.
5. GitHub: new repo, upload these files, Settings > Pages > deploy from main. The CNAME file holds the custom domain.
