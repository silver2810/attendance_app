# attendance_app
Tracking Sabbath School Attendance

## Deploy on Render for online access

This project is configured as a static site for Render via `/home/runner/work/attendance_app/attendance_app/render.yaml`.

1. Push this repository to GitHub.
2. In Render, click **New +** → **Blueprint**.
3. Select this repository and create the service.
4. Render will deploy using `public/` as the published folder.

After deployment, your app URL will look like:

`https://<your-render-service>.onrender.com`

## QR code that opens the form

- Open your deployed app URL.
- The home page (`/`) shows a QR code that points to:
  - `https://<your-render-service>.onrender.com/form.html`
- Share or print that QR code so people can scan it and fill out the attendance form online.

## Local development

To preview locally:

```bash
cd /home/runner/work/attendance_app/attendance_app
python -m http.server 8000 --directory public
```

Then open `http://localhost:8000`.
