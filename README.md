

<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">



<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<meta name="theme-color" content="#102b24">
<meta name="description" content="Discover Hilltop Haven in Kotagala, Sri Lanka — delicious food, warm hospitality and a refreshing hill-country atmosphere.">
<title>Hilltop Haven | Mountain Dining in Kotagala</title>

<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=DM+Sans:wght@400;500;600;700&family=Playfair+Display:wght@500;600;700&display=swap" rel="stylesheet">

<style>
:root {
    --green: #123c30;
    --green2: #28634c;
    --gold: #d9b978;
    --cream: #f5f3ec;
    --paper: #fff;
    --ink: #1d3028;
    --muted: #6d7c73;
    --line: rgba(25,60,45,.13);
    --shadow: 0 18px 55px rgba(15,45,32,.12);
}

* {
    box-sizing: border-box;
    margin: 0;
    padding: 0;
}

html {
    scroll-behavior: smooth;
    scroll-padding-top: 88px;
}

body {
    font-family: "DM Sans", sans-serif;
    background: var(--cream);
    color: var(--ink);
    transition: background .3s, color .3s;
}

body.dark {
    --cream: #101e19;
    --paper: #1a2d24;
    --ink: #eef3ed;
    --muted: #b2c1b7;
    --line: rgba(230,240,230,.13);
    --shadow: 0 18px 55px rgba(0,0,0,.22);
}

a {
    color: inherit;
    text-decoration: none;
}

button, input, select, textarea {
    font: inherit;
}

button {
    cursor: pointer;
}

img {
    display: block;
    max-width: 100%;
}

.container {
    width: min(1160px, 90%);
    margin: auto;
}

.section {
    padding: 100px 0;
}

.eyebrow {
    font-size: .75rem;
    font-weight: 700;
    letter-spacing: 4px;
    text-transform: uppercase;
    color: var(--green2);
}

body.dark .eyebrow {
    color: var(--gold);
}

.section-head {
    text-align: center;
    max-width: 690px;
    margin: 0 auto 46px;
}

.section-head h2,
.story h2,
.reserve-copy h2 {
    font: 600 clamp(2.3rem,5vw,3.8rem)/1.12 "Playfair Display", serif;
    margin: 15px 0;
}

.section-head p,
.muted {
    color: var(--muted);
    line-height: 1.85;
}

/* Navigation */

header {
    position: fixed;
    z-index: 1000;
    inset: 0 0 auto;
    background: rgba(245,243,236,.88);
    backdrop-filter: blur(18px);
    border-bottom: 1px solid var(--line);
}

body.dark header {
    background: rgba(16,30,25,.9);
}

.nav {
    min-height: 78px;
    display: flex;
    align-items: center;
    justify-content: space-between;
    gap: 22px;
}

.brand {
    font: 700 1.5rem "Playfair Display", serif;
    color: var(--green);
    white-space: nowrap;
}

body.dark .brand {
    color: var(--gold);
}

.brand span {
    color: var(--gold);
}

.navlinks {
    display: flex;
    align-items: center;
    gap: 25px;
    list-style: none;
}

.navlinks a {
    font-size: .87rem;
    font-weight: 600;
    transition: color .2s;
}

.navlinks a:hover {
    color: #b48a43;
}

.navtools {
    display: flex;
    align-items: center;
    gap: 10px;
}

.icon-btn,
.menu-toggle {
    height: 41px;
    width: 41px;
    border: 1px solid var(--line);
    border-radius: 50%;
    background: transparent;
    color: var(--ink);
}

.menu-toggle {
    display: none;
    border-radius: 9px;
    font-size: 1.2rem;
}

/* Buttons */

.btn {
    display: inline-flex;
    align-items: center;
    justify-content: center;
    gap: 9px;
    padding: 14px 23px;
    border-radius: 5px;
    border: 1px solid var(--green);
    background: var(--green);
    color: white;
    font-weight: 700;
    transition: .25s;
}

.btn:hover {
    transform: translateY(-3px);
    background: var(--green2);
}

.btn.gold {
    background: var(--gold);
    border-color: var(--gold);
    color: #1d3428;
}

.btn.outline {
    background: transparent;
    border-color: rgba(255,255,255,.7);
    color: white;
}

/* Hero section */

.hero {
    min-height: 100svh;
    display: flex;
    align-items: center;
    color: white;
    position: relative;
    background:
        linear-gradient(90deg,rgba(5,24,18,.86),rgba(5,24,18,.45),rgba(5,24,18,.08)),
        url("https://images.unsplash.com/photo-1448375240586-882707db888b?auto=format&fit=crop&w=2200&q=85") center/cover no-repeat;
}

.hero:after {
    content: "";
    position: absolute;
    inset: auto 0 0;
    height: 130px;
    background: linear-gradient(transparent,rgba(5,24,18,.35));
    pointer-events: none;
}

.hero-content {
    position: relative;
    z-index: 1;
    max-width: 760px;
    padding-top: 90px;
    animation: rise .9s both;
}

.pill {
    display: inline-block;
    border: 1px solid rgba(255,255,255,.5);
    border-radius: 30px;
    padding: 10px 15px;
    letter-spacing: 2px;
    font-size: .75rem;
    background: rgba(255,255,255,.08);
    backdrop-filter: blur(8px);
}

.hero h1 {
    font: 600 clamp(3.4rem,8vw,7rem)/.98 "Playfair Display", serif;
    margin: 27px 0;
}

.hero h1 em {
    color: var(--gold);
}

.hero p {
    max-width: 570px;
    color: #e9eee9;
    line-height: 1.9;
    font-size: 1.06rem;
    margin-bottom: 30px;
}

.actions {
    display: flex;
    gap: 13px;
    flex-wrap: wrap;
}

.hero-meta {
    margin-top: 55px;
    color: #e1e9e2;
    letter-spacing: 2px;
    font-size: .76rem;
}

/* Highlights */

.highlights {
    background: var(--green);
    color: white;
    padding: 26px 0;
}

.highlight-grid {
    display: grid;
    grid-template-columns: repeat(4,1fr);
    gap: 20px;
}

.highlight {
    display: flex;
    align-items: center;
    justify-content: center;
    gap: 12px;
}

.highlight .emoji {
    font-size: 1.7rem;
}

.highlight strong {
    display: block;
    font-size: .95rem;
}

.highlight small {
    color: #c6d7cb;
}

/* About section */

.story-grid {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 70px;
    align-items: center;
}

.story-photo {
    position: relative;
}

.story-photo img {
    width: 100%;
    height: 540px;
    object-fit: cover;
    border-radius: 8px;
}

.photo-tag {
    position: absolute;
    right: -18px;
    bottom: 28px;
    background: var(--gold);
    color: #1d3428;
    padding: 20px 25px;
    text-align: center;
    border-radius: 5px;
}

.photo-tag strong {
    display: block;
    font: 700 1.5rem "Playfair Display", serif;
}

.story h2 {
    margin: 15px 0 20px;
}

.story p {
    color: var(--muted);
    line-height: 1.9;
    margin-bottom: 17px;
}

.story-points {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 13px;
    margin: 25px 0;
}

.story-points div {
    background: var(--paper);
    padding: 17px;
    border-radius: 7px;
    box-shadow: var(--shadow);
}

.story-points strong {
    display: block;
    margin-bottom: 6px;
}

/* Menu section */

.menu-section {
    background: var(--paper);
}

.filters {
    display: flex;
    justify-content: center;
    gap: 10px;
    flex-wrap: wrap;
    margin-bottom: 35px;
}

.filter {
    border: 1px solid var(--line);
    background: transparent;
    color: var(--ink);
    padding: 10px 18px;
    border-radius: 30px;
}

.filter.active,
.filter:hover {
    background: var(--green);
    color: white;
    border-color: var(--green);
}

.menu-grid {
    display: grid;
    grid-template-columns: repeat(3,1fr);
    gap: 24px;
}

.dish {
    background: var(--cream);
    border-radius: 9px;
    overflow: hidden;
    box-shadow: var(--shadow);
    transition: .3s;
}

.dish:hover {
    transform: translateY(-7px);
}

.dish.hide {
    display: none;
}

.dish img {
    height: 225px;
    width: 100%;
    object-fit: cover;
}

.dish-info {
    padding: 21px;
}

.dish h3 {
    font: 600 1.35rem "Playfair Display", serif;
    margin-bottom: 9px;
}

.dish p {
    font-size: .9rem;
    color: var(--muted);
    line-height: 1.7;
    min-height: 48px;
}

.dish-bottom {
    display: flex;
    justify-content: space-between;
    margin-top: 17px;
    font-weight: 700;
}

.price {
    color: #b48a43;
}

/* Experience */

.experience {
    color: white;
    background:
        linear-gradient(rgba(12,43,31,.88),rgba(12,43,31,.88)),
        url("https://images.unsplash.com/photo-1500530855697-b586d89ba3ee?auto=format&fit=crop&w=1800&q=85") center/cover fixed;
}

.experience .section-head p {
    color: #d7e2d9;
}

.experience .eyebrow {
    color: var(--gold);
}

.experience-grid {
    display: grid;
    grid-template-columns: repeat(3,1fr);
    gap: 22px;
}

.experience-card {
    padding: 32px 27px;
    border: 1px solid rgba(255,255,255,.22);
    background: rgba(255,255,255,.07);
    backdrop-filter: blur(9px);
    border-radius: 9px;
    transition: .3s;
}

.experience-card:hover {
    transform: translateY(-6px);
    background: rgba
