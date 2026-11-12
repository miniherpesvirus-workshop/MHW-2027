# Miniherpesvirus Workshop 2027

A responsive announcement page for the MHW's European chapter in Rotterdam.
Plain HTML and CSS: no build, installation, JavaScript, external fonts or dependencies.

## What is included

- `index.html`: the complete page, including all styling.
- `assets/rotterdam.png`: the organiser-supplied Rotterdam image.
- `.nojekyll`: tells GitHub Pages to serve these static files directly.
- `assets/README.md`: image details and replacement instructions.

## Event details

The workshop is in **Rotterdam on 23–24 September 2027**.
The organisers are **Georges Verjans, Werner Ouwendijk and Michiel van Gent**.
The dates, names and image were supplied by the organiser.

The working name is **Miniherpesvirus Workshop 2027**, with the announcement
line **The MHW goes European**. Venue, registration, abstract submissions
and programme remain explicitly unannounced. Fees, speakers and sponsors
have not been carried forward from 2026.

This is the MHW announcement. The International Herpesvirus Workshop is a
separate meeting; its homepage lists Rotterdam for 2028.

## Rotterdam image

The uploaded `Rotterdam.png` is already included as `assets/rotterdam.png`.
Its original 2048 × 819 pixels are preserved. The full collage remains visible
on mobile, with the date and location caption beneath it on narrow screens.
No photo replacement is needed before uploading this package.

If replacing the image later, update the `src`, `alt`, `width` and `height`
attributes in `index.html`. Keep the path relative, without a leading `/`, and
adjust the `.city-figure` CSS aspect ratio to match. Add any required photo
credit at the `PHOTO CREDIT` comment.

## Publish from GitHub's website (recommended)

1. Open the intended **2027 repository** in your GitHub account or organisation.
   The instructions below use `miniherpesvirus-workshop/MHW-2027` as an example;
   the existence and exact name of that repository have not been verified.
   If needed, create a public repository named `MHW-2027` under the organisation
   you intend to use. A public repository works with GitHub Free.
2. Extract the ZIP. Upload **the contents of the extracted `MHW-2027` folder**
   into the repository's root using **Add file → Upload files**. Ensure that
   `index.html` is at the repository root, not in another `MHW-2027` subfolder.
   Preserve the `assets` folder and include `.nojekyll`.
3. Commit the upload to `main` (or the repository's actual default branch).
4. Open **Settings → Pages**. Under **Build and deployment**, select
   **Deploy from a branch**, then choose **main** and **/(root)**. Click **Save**.
5. GitHub shows the published address on the Pages settings screen. With the
   example organisation and repository above, the expected address is:
   `https://miniherpesvirus-workshop.github.io/MHW-2027/`.
   If your organisation or repository name differs, the address differs too.
   Initial publication can take up to 10 minutes.

Keep the 2026 repository as the archive. Later commits to the selected publishing
branch update the 2027 website automatically. No custom workflow is needed.
If the repository already publishes through a custom GitHub Actions workflow,
review that configuration before changing its publishing source.

## Publish from an existing local Git clone

Clone the intended 2027 repository, copy this package's contents into its root,
and confirm the announcement text. The photo is already included. Run these commands from
the clone:

```bash
git status
git add index.html assets .nojekyll README.md
git commit -m "Add MHW 2027 announcement page"
git push
```

Configure **Settings → Pages → Deploy from a branch → main → /(root)** once as
described above. Do not run `git init` over an existing repository.

## Editing the page later

Search `index.html` for the `EDIT`, `PHOTO` and `PHOTO CREDIT` comments.

| Change | Where to edit |
| --- | --- |
| Formal title / event name | `<title>`, description and Open Graph metadata, header, main heading and footer |
| Date | Introduction, location label over the image, about paragraph, “When” row, footer and metadata |
| Venue | “Location” row in the information table |
| Registration | Replace its information row with the confirmed details and a real link |
| Abstract submission | Replace its information row with the confirmed details and a real link |
| Organisers | “Organisers” row in the information table and description metadata |
| Contact | Add confirmed contact details below the about section |
| Photo and credit | Image `src`, `alt` text and the caption paragraph |
| Colours | Variables at the top of the `<style>` block |

All links and assets use relative paths where appropriate so the site also
works under a GitHub project URL such as `/MHW-2027/`. To preview locally,
open `index.html` in a browser; no server is required.

## References checked on 12 November 2026

- MHW 2026: https://miniherpesvirus-workshop.github.io/MHW-2026/
- MHW 2026 event listing: https://g-f-v.org/events/19th-mini-herpesvirus-workshop/
- IHW homepage and visual reference: https://www.herpesvirusworkshop.com/
- IHW 2026: https://www.herpesvirusworkshop.com/2026/
- GitHub Pages publishing instructions:
  https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site

The design takes inspiration from IHW's teal palette and city photographs with
year and location labels. Its HTML, CSS, geometric mark and text were created
for this draft. The Rotterdam image was supplied by the organiser; IHW logos
and photographs are not included.
