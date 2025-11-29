AWS-01 – S3 + CloudFront Portfolio Website

# Project: Portfolio Website on AWS S3 + Cloudfront + Route 53 + ACM

## Goal: Host a personal portfolio site using AWS serverless services with global HTTPS delivery.

**High-level flow:**

User → DNS (Route 53) → CloudFront (HTTPS) → S3 Static Website Endpoint → index.html

**Architecture:**
  Amazon S3 (Static website hosting)
  Cloudfront (CDN + HTTPS)
  Route 53 + ACM for custom domain

**What I built:**
  Created an S3 bucket with static website hosting enabled.
  Uploaded static assets (HTML/CSS/images) to S3.
  Configured a public-read bucket policy for website content.
  Set up a CloudFront distribution With S3 website endpoint as origin.
  Enabled Redirect HTTP to HTTPS and set index.html as the default root object.
  Configured custom domain + SSL via ACM & Route 53.

**Tech Skills Demonstrated: **
  S3 bucket configuration, static web hosting, bucket policies.
  CloudFront distribution creation and cache behavior configuration.
  Basic DNS management and ACM TLS certificate setup.

**Links:**
  CloudFront URL: https://d3jijzkbd3efvw.cloudfront.net
  
  Custom Domain: www.awsdjm.com
  
  GitHub repo: https://github.com/Satcomonline/AWS-Examples
  
