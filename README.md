# Creative Portfolio — GitHub Pages starter

This is a one-page portfolio adapted from the visual direction of the sample portfolio you shared: dark background, lime accent, Manrope + DM Mono typography, sticky navigation, and responsive layout. The multi-page programmer case studies have been replaced with three video projects displayed on the same page.

## 1. Before publishing

Open `index.html` and replace:

- `[YOUR NAME]` with the name you want to display.
- `your.email@example.com` with your public contact email.
- The CV link target by adding your PDF as `assets/your-cv.pdf` (or remove the CV links if you do not want to publish one).
- Social links if your profile URLs change.

The project descriptions are draft wording based on the information you provided. Review them before publishing.

## 2. Add your videos

Copy your compressed MP4 files into `assets/videos/` using these exact names:

- `acnhoes.mp4`
- `acnhoes-irl.mp4`
- `chibinvasion-wip.mp4`

The page uses local HTML video players (`<video controls>`) with `preload="none"`, so the clips are not intentionally preloaded when someone first opens the page. The temporary SVG posters are only visual placeholders; replace them with screenshots/thumbnails from your own videos when ready.

Recommended: MP4 / H.264, 720p or 1080p, short clips, compressed for web playback. Keep each video as small as practical. GitHub's browser upload currently allows up to 25 MiB per file; command-line uploads allow up to 100 MiB per file. GitHub blocks files larger than 100 MiB in normal Git, and Git LFS cannot be used with GitHub Pages. Avoid putting original camera footage or high-bitrate masters in this repository.

## 3. Preview on your computer

You can open `index.html` directly in a browser for a quick visual check. To test video paths more reliably, use a local server:

```bash
python -m http.server 8000
```

Then visit `http://localhost:8000`.

## 4. Publish with GitHub Pages

1. Create a GitHub repository. For the cleanest address, name it `<your-github-username>.github.io` if that user-site repository is available. Otherwise, name it `creative-portfolio`; the resulting address will include `/creative-portfolio/`.
2. For GitHub Free, make the repository public to use GitHub Pages.
3. Upload the contents of this folder to the repository root. Important: `index.html` must be at the root, not inside an extra `creative-portfolio` folder.
4. Open the repository's **Settings → Pages**.
5. Under **Build and deployment**, choose **Deploy from a branch**.
6. Select branch **main** and folder **/(root)**, then click **Save**.
7. After GitHub finishes publishing, the site address will appear in the Pages settings.

GitHub Pages sites are public on the internet. Do not put private information in this repository. The site uses relative file paths, so it can work as either a user site or a project site.

## 5. Important GitHub Pages video limits

GitHub Pages is static hosting, not a dedicated video-streaming service. Published sites may be up to 1 GB and have a soft bandwidth limit of 100 GB per month. Keep the site and clips lightweight. If a clip is larger than 25 MiB, use GitHub Desktop or Git from the command line to upload it; if it is larger than 100 MiB, it will not work as a normal Git file on Pages.

Official references:
- https://docs.github.com/en/pages/getting-started-with-github-pages/github-pages-limits
- https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site
- https://docs.github.com/en/repositories/working-with-files/managing-files/adding-a-file-to-a-repository
- https://docs.github.com/en/repositories/working-with-files/managing-large-files/about-git-large-file-storage

## Project notes

- `Acnhoes`: social media comedy videos featuring Animal Crossing characters.
- `Acnhoes IRL`: character integration/compositing experiment in pre-recorded footage.
- `Chibinvasion`: original character project marked WIP. The Butter clip is explicitly identified as a temporary test using a character that is not part of the original IP.

The site does not include the actual videos or résumé PDF yet. Add those files before sharing the portfolio publicly.
