# Architecture – AWS-01 S3 + CloudFront Portfolio

## Overview

This project hosts a static website in an S3 bucket and uses CloudFront as a CDN in front of it, with a custom domain managed in Route 53 and HTTPS provided by ACM.

## Components

- **Amazon S3**
  - Hosts static HTML, CSS, and image files
  - Static website hosting enabled with `index.html` as root

- **Amazon CloudFront**
  - Uses the S3 **website endpoint** as origin
  - Redirects HTTP to HTTPS
  - Caches content at edge locations

- **AWS Certificate Manager (ACM)**
  - Issues TLS certificate for `yourdomain.com` and `www.yourdomain.com`
  - DNS validation via Route 53 CNAME records

- **Route 53**
  - Public hosted zone for `yourdomain.com`
  - A Alias record pointing to CloudFront distribution

## Diagram

See `architecture-diagram.png` for a visual representation.
