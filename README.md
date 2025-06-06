# 🧄‍♂️ Beard Bros Vending – Fort Worth’s Most Reliable Vending Machine Provider



Live Site 👉 beardbrosvending.com

## 📌 Overview

Beard Bros Vending is a modern, SEO-optimized vending machine service website built for local businesses in the Fort Worth area. It highlights our mission to provide premium vending solutions — from healthy snacks and smart coolers to 24/7 service — while showcasing a scalable tech stack and professional branding.

This repository contains the full source code for the live production site, hosted on AWS S3 + CloudFront, with a CI/CD pipeline powered by GitHub Actions.

## 🚀 Tech Stack

Frontend: Vite + React + Tailwind CSS

Routing: React Router

Icons: Lucide React

SEO: react-helmet-async + Open Graph + Twitter Cards

Forms: FormSubmit.co (SMTP Email forwarding)

Hosting: S3 static site + CloudFront CDN + Route 53 domain

CI/CD: GitHub Actions → AWS CLI (aws s3 sync)

Asset Hosting: Public S3 bucket for Open Graph images & favicon

## 🧩 Features

✅ Responsive and mobile-first layout

✅ SEO-optimized with rich meta tags and structured data (JSON-LD)

✅ Contact form with form forwarding

✅ Open Graph support for clean previews via SMS, iMessage, Facebook, etc.

✅ Local business schema for Google indexing

✅ Branded color palette (red, white, black)

✅ Optimized page speed with Vite

✅ Dynamically rendered blog page (static content)

✅ Smart cooler + micro market services highlighted

✅ Easy asset management via S3 for marketing images

## 🗂️ File Structure

📁 /src
 ├️ 📁 components        # Reusable components like Navigation, Footer, SEO
 ├️ 📁 pages             # Page components like Home, About, Services, Contact, Blog
 ├️ 📁 assets            # Logo, favicon, and placeholder images (if not hosted on S3)
 ├️ 🗋 main.tsx          # Entry point
 ├️ 🗋 App.tsx           # App layout + Router setup
📁 /public
 ├️ 🗋 index.html        # Meta tags for social sharing
🗋 tailwind.config.js   # Custom Tailwind theme
🗋 package.json

## 🧠 What I Learned

Configuring and deploying a production-grade static website on AWS

Creating Open Graph and Twitter preview cards with dynamic meta content

Integrating structured data with react-helmet-async

Managing website assets with S3 for performance and CDN caching

Automating deployment with GitHub Actions and aws-cli

Building an SEO-optimized architecture with clean UX/UI

## 📷 Screenshot Preview

## ⚙️ Deployment Instructions

### Build the project
npm install
npm run build

### Deploy to S3
aws s3 sync dist/ s3://beardbrosvending.com --delete

### Invalidate CloudFront cache (if needed)
aws cloudfront create-invalidation --distribution-id YOUR_DISTRIBUTION_ID --paths "/*"

### ✨ Credits

Design + Branding: Cody Brookes

Development: Cody Brookes

Powered by: AWS, Vite, Tailwind, React

### 📬 Contact

Want to connect about vending, websites, or automation?

📧 info@beardbrosvending.com📍 Fort Worth, TX
