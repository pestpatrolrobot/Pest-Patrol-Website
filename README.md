# Pest Patrol

Pest Patrol is a static project website for a student-built automated pesticide car concept focused on controlled pesticide spraying, crop treatment support, and practical farm automation.

## Features

- Responsive landing page for desktop and mobile
- Project mission and automated pesticide car technology sections
- Dedicated project parts section with categories and component descriptions
- QR code section that links to the deployed website
- Hosted visitor counter badge below the QR code
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
    parts/
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

## Project Parts Section

The Parts navigation item links to the `#parts` section in `index.html`. Parts are grouped by function:

- Control and Electronics
- Sensors and Movement
- Spraying System
- Power Supply
- Wiring and Assembly

Each part card includes:

- Component image
- Category badge
- Component name
- Short explanation of how it is used in the Pest Patrol prototype

Part images are stored in:

```text
images/parts/
```

Current part image files:

```text
4dof arm.jpg
4wd chassis kit.jpg
Arduino_Uno_-_R3.jpg
awg wire.jpg
barb connector.jpg
battery holder.jpg
buck converter1.png
buck converter2.png
esp32.jpg
hcr sensor.jpg
jumper wires.jpg
line tracking.jpg
m3 bolts and nuts.jpg
m3 standoffs.jpg
ncr batterry.jpg
nozzle.jpg
pump.jpg
relay module.jpg
rocker switch.jpg
servo channel.jpg
tbb612 module.jpg
tube.jpg
```

The website uses fixed image frames and `object-fit: contain` so low-resolution or uneven photos display consistently without stretching.

## QR Code and Visitor Counter

The QR section points to the live GitHub Pages website:

```text
https://pestpatrolrobot.github.io/Pest-Patrol-Website/
```

The QR image is loaded from a QR image endpoint, and the visitor total is shown with a hosted counter badge. Because GitHub Pages is static, the site cannot store a global visit count without an external service.

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

This site deploys to GitHub Pages through `.github/workflows/pages.yml` whenever changes are pushed to `main`.

Live site:

```text
https://pestpatrolrobot.github.io/Pest-Patrol-Website/
```

You can also deploy this site to any static hosting service, including GitHub Pages, Netlify, Vercel, or Cloudflare Pages. Make sure `index.html`, `images/robot/`, `images/team/`, and `images/parts/` are included in the deployed files.
