# S3-Web-Hosting

DevOps S3 Web Hosting Assignment

1. Static Portfolio Website Development
Build a simple DevOps portfolio website using HTML (and optional CSS). Your site must
include:
 Your name and role (e.g., DevOps Engineer)
 Skills list
 Certifications
 Project descriptions
 Contact information or LinkedIn link

Customize the design by changing colors, layout, sections, and text to reflect your personal
brand.

2. S3 Static Website Hosting
Create a new S3 bucket and:
 Enable static website hosting
 Set index.html as the default page
 Upload your customized portfolio files
 Make the site public using a bucket policy only (do not enable public access manually)
 Share the S3 static website URL

3. Bucket Policy Configuration
Apply a bucket policy that grants public read access only to the objects in the bucket.
Paste the bucket policy used and explain what each part of it does.

4. Lifecycle Rule Setup
Create a lifecycle rule on your S3 bucket to:

 Transition objects to GLACIER storage after 30 days
 Delete objects after 180 days

Take a screenshot of your lifecycle rule configuration and explain the rule briefly.

5. DNS Customization (Bonus)
(Optional, extra credit)
Use a domain or subdomain from Route 53 (or any free DNS provider) to point to your S3
website by:
 Creating a CNAME or Alias record to map your domain to the S3 website endpoint
Provide a screenshot of your DNS record configuration and the custom domain in use.

6. Submission Requirements
Include the following in your submission:
 Screenshots showing:
o S3 bucket with static hosting enabled
o Bucket policy applied
o Lifecycle rule created
o Website working in browser
o (Optional) DNS alias/custom domain working
 A short text or README file explaining what you changed in your site and setup
 URL link to your portfolio

&lt;!DOCTYPE html&gt;
&lt;html lang=&quot;en&quot;&gt;
&lt;head&gt;
