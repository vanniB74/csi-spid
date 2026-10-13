# C.S.I. — Centro Servizi Integrati (SPID e PEC)

Website for C.S.I. — Centro Servizi Integrati at ACLI Ceglie del Campo (Bari). It covers the centre's SPID and PEC services, FAQ, contacts and privacy policy. Visitors can book an appointment there, and the site generates a printable client file (cover sheet, assistance mandate and GDPR consent).

## Technologies

- A single static HTML page (`public/index.html`) with inline CSS and vanilla JavaScript
- Appointments and client files are saved in the browser's `localStorage`; reminders are sent as an `.ics` download or via `mailto:`
- Hosted on Netlify as a static site, with no build step

## Run locally

```bash
netlify dev
# or any static server, e.g.
npx serve public
```

## Origin

The page was imported from a Z.AI shared space (`chat.z.ai/space/d1aj48756bs1-art`). Its images now live in `public/img/` and are no longer loaded from Z.AI's CDN.
