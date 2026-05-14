# Pest Patrol

Pest Patrol is a static project website for a student-built automated pesticide car concept focused on controlled pesticide spraying, crop treatment support, and practical farm automation.

## Features

- Responsive landing page for desktop and mobile
- Project mission and automated pesticide car technology sections
- Toggleable team section
- Team portrait containers with initials fallback
- Robot prototype slideshow
- Contact/footer section with project details

## Project Structure

```text
pest-patrol-main/
  index.html
  README.md
  images/
    robot/
    team/
```

## Add Robot Photos

The top hero slideshow uses these files:

```text
images/robot/robot-1.jpg
images/robot/robot-2.jpg
images/robot/robot-3.jpg
```

## Add Team Photos

Place team photos in `images/team/` using these filenames:

```text
kiel-alcantara.jpg
curt-tataro.jpg
jared-vallangca.jpg
angelo-rivera.jpg
marinella-dela-cruz.jpg
shaine-vasquez.jpg
jewel-arce.jpg
john-paul-halili.jpg
jesriel-lapig.jpg
jovylem-siblag.jpg
allyssa-bajalla.jpg
```

If a photo is missing, the website shows the member's initials instead.

## Run Locally

This is a static site. You can open `index.html` directly, or serve it locally:

```bash
node dev-server.cjs
```

Then open:

```text
http://localhost:3000
```

In this workspace, the local server is intended to run at:

```text
http://127.0.0.1:3000
```

## Deploy

You can deploy this site to any static hosting service, including GitHub Pages, Netlify, Vercel, or Cloudflare Pages. Make sure `index.html` and the `images/team/` folder are included in the deployed files.
