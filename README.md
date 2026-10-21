# LEMBEM LAB

Official static research website for the Laboratory for Emerging Media, Bio-informatics and Engineering Models (LEMBEM), built with the visual design language of the [AgriSense project](https://github.com/yanghoxom/agrisense-ai).

**Site:** https://lab.lembem.com  
**Repository:** `yanghoxom/lembem`  
**Technology:** static HTML, Tailwind CSS via CDN, Lexend and Material Symbols.

## Institutional information

The legal and team details below were provided by the repository owner for publication.

- **English name:** Laboratory for Emerging Media, Bio-informatics and Engineering Models (LEMBEM)
- **Vietnamese name:** Viện Nghiên cứu Mô hình Kỹ thuật, Tin sinh học và Truyền thông Mới
- **Status:** Registered Non-Profit Scientific and Technological Organization (Tổ chức Khoa học và Công nghệ ngoài công lập / Phi lợi nhuận)
- **Registration:** A-2836 / ĐK-KHCN
- **Tax ID:** 2301284126
- **Founded:** 2025-05-15
- **Headquarters:** Chi Lang Commune, Bac Ninh Province, Vietnam
- **Legal representative:** Dao Van Hung (Hung Dao), Director of Research & Legal Representative
- **Email:** contact@lembem.com

## Research team

- Hung Dao — Director of Research & Principal Investigator (Engineering Models & Open AI)
- Phung Ha — Secretary General & Head of Bio-informatics Research
- Minh Nguyen — Lead Researcher (Emerging Media & Scientific Archiving)

## Projects

- **AgriSense Open Initiative:** Active Community Deployment; https://agrisense.lembem.com
- **VietBioNet Dataset:** Open Access Dataset (CC BY-NC 4.0); https://lab.lembem.com/datasets/vietbionet
- **EcoModel-VN:** In Development · Private. No publicly accessible source code or repository link.

The VietBioNet page has a **research access request form** and a conditional acknowledgement modal. It does not contain the actual dataset files. The EcoModel-VN repository remains intentionally private during development.

## Repo structure

- `index.html` — landing page with mission, pillars, initiatives, governance, publications, dataset anchor, support and contact
- `governance.html` — registration details, roles and public-benefit commitments
- `datasets/vietbionet/index.html` — dataset overview, access request form, delivery confirmation modal and CC BY-NC 4.0 notice
- `privacy.html` — privacy notice
- `terms.html` — website terms
- `CONTENT-LICENSE.md` — original website content licence
- `favicon.svg` — LEMBEM icon
- `CNAME` — GitHub Pages custom domain `lab.lembem.com`
- `.nojekyll` — GitHub Pages static-content support

## Hosting

The site is already configured for GitHub Pages from `main` and uses the custom domain in `CNAME`. Static updates committed to `main` should trigger Pages deployment. No build command is required.

## Licensing and third-party assets

Original website text is designated CC BY-NC 4.0 unless otherwise noted. VietBioNet is designated CC BY-NC 4.0. EcoModel-VN remains private; its licence will be announced on release. These terms do **not** automatically extend to third-party images, fonts, logos, or source code that may be governed by different rights. The hero background and logo have been retained from the site's current design.

## VietBioNet access request form

The request form sends submitted name, email, optional institution and research purpose to `https://formsubmit.co/ajax/contact@lembem.com`, using JSON POST and a same-page confirmation modal. The modal opens **only** if the provider returns `success: true` or `success: "true"`; FormSubmit can respond with `success: "false"` even on HTTP 200. Failed/activation-pending submissions show an error instead of claiming successful delivery.

**Important one-time setup:** FormSubmit requires the owner of `contact@lembem.com` to activate the destination email by clicking the verification link sent by FormSubmit when the first request is submitted. Until activation, delivery is not confirmed and the UI offers direct email contact. This has not been activated or test-submitted by the site editor. See [FormSubmit's documentation](https://formsubmit.co/documentation).

The form's collected personal information is described in `privacy.html`. FormSubmit is an external processor; website visitors must tick a consent checkbox. The form has a honeypot field for spam prevention. To replace FormSubmit with an in-house API or an existing organization endpoint, update the `action` URL in `datasets/vietbionet/index.html`.
