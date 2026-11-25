# Creative Portfolio — GitHub Pages starter

This is a one-page creative portfolio inspired by the sample site you shared: dark background, lime accent, Manrope + DM Mono typography, sticky navigation, and responsive layout. It is designed around **vertical 9:16 videos** for Acnhoes, Acnhoes IRL, and Chibinvasion.

## 1. Before publishing

Open `index.html` and replace:

- `[YOUR NAME]` with the name you want to display.
- `your.email@example.com` with your public contact email.
- Social links if your profile URLs change.

The résumé/CV links are currently left inside HTML comments, so they do not appear on the page. When you have a PDF ready, you can remove the comments around any CV link and add the PDF file.

The project descriptions are draft wording based on the information you provided. Review them before publishing.

## 2. Add your vertical videos

Copy your compressed MP4 files into `assets/videos/` using these exact names:

- `acnhoes.mp4`
- `acnhoes-irl.mp4`
- `chibinvasion-wip.mp4`

The video frames are designed for portrait **9:16** footage. On desktop, the video appears beside its description; on mobile, it is centered above the description and scales to the screen width. The HTML video players use `controls`, `playsinline`, and `preload="none"` so clips are not intentionally downloaded when the page first opens.

Recommended export settings:

- MP4 / H.264
- 1080 × 1920 (or 720 × 1280)
- 24–30 fps
- AAC audio
- Use a web-friendly bitrate and keep each clip as small as practical. A short portfolio excerpt is usually better than uploading a full-length source video.

The SVG files in `assets/posters/` are portrait placeholder covers. Replace them with a still frame from each real video when ready. A JPG or WebP poster is also fine; update the `poster` path in `index.html` if you change the filename.

## 3. Preview on your computer

From this folder, run:

```bash
python -m http.server 8000
```

Then visit `http://localhost:8000` on your computer. To check the mobile layout, resize the browser window or open the same local-network address on your phone while both devices are on the same Wi-Fi network. `localhost` on a phone refers to the phone itself, not your computer.

## 4. Publish with GitHub Pages

1. Create a GitHub repository. For the cleanest address, name it `<your-github-username>.github.io` if that user-site repository is available. Otherwise, name it `creative-portfolio`; the resulting address will include `/creative-portfolio/`.
2. For GitHub Free, make the repository public to use GitHub Pages.
3. Upload the **contents** of this folder to the repository root. Important: `index.html` must be at the root, not inside an extra `creative-portfolio-starter` folder.
4. Open the repository's **Settings → Pages**.
5. Under **Build and deployment**, choose **Deploy from a branch**.
6. Select branch **main** and folder **/(root)**, then click **Save**.
7. After GitHub finishes publishing, the site address will appear in the Pages settings.

Official guide: https://docs.github.com/en/pages/quickstart

## 5. Important GitHub Pages video limits

GitHub Pages is static hosting, not a dedicated video-streaming service. Published sites may be up to 1 GB and have a soft bandwidth limit of 100 GB per month. Git LFS cannot be used with GitHub Pages. GitHub's browser upload currently allows up to 25 MiB per file; command-line uploads allow up to 100 MiB per file. Avoid putting original camera footage or high-bitrate masters in this repository.

Official references:
- https://docs.github.com/en/pages/getting-started-with-github-pages/github-pages-limits
- https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site
- https://docs.github.com/en/repositories/working-with-files/managing-files/adding-a-file-to-a-repository
- https://docs.github.com/en/repositories/working-with-files/managing-large-files/about-git-large-file-storage

## Project notes

- `Acnhoes`: social media comedy videos featuring Animal Crossing characters.
- `Acnhoes IRL`: character integration/compositing experiment in pre-recorded footage.
- `Chibinvasion`: original character project marked WIP. The Butter clip is a temporary test; Butter is not an original Chibinvasion character.

The site does not include the actual videos or résumé PDF yet. Add your own MP4 files before sharing the portfolio publicly.
