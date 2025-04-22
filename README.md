# My DevOps Portfolio - AWS S3 Static Website Project

I built a personal portfolio website to showcase my DevOps skills and hosted it on AWS S3. This project let me practice both front-end design and AWS cloud configuration.

## Site Customisation
I wasn't a fan of the original template's look, so I made several changes to create something that better represents me:

- Switched to a more subtle blue-grey gradient background that looks more professional
- Used Montserrat and Roboto fonts from Google Fonts instead of the basic ones
- Made the skills and certifications display in a nice grid layout
- Added hover effects to make the site feel more interactive
- Fixed the spacing and padding to give everything room to breathe


- Updated everything with my name (Chibuzo Nmecha)
- Added some specific achievements, like how I reduced deployment times by 40%
- Added AWS Cloud Practitioner cert
- Updated my contact info with my real email and GitHub

## AWS Configuration

1. Created a unique S3 bucket
2. Turned on static website hosting and set index.html as the main page
3. Uploaded all my website files

For security, I used a bucket policy instead of just making everything public:
```json
{
  "Version": "2012-10-17",
  "Statement": [
    {
      "Sid": "PublicReadGetObject",
      "Effect": "Allow",
      "Principal": "*",
      "Action": "s3:GetObject",
      "Resource": "arn:aws:s3:::my-portfolio-bucket/*"
    }
  ]
}
```
This lets people view my site but doesn't let them mess with my files.

I also set up a lifecycle rule to save on storage costs:
- Move files to GLACIER after 30 days (cheaper storage)
- Delete them after 180 days (so I remember to keep content fresh)

For the bonus part, I did not configure a custom subdomain using Route 53.

## What I Learned
This project helped me practice:
- Working with S3 buckets and permissions
- Writing IAM policies
- Building and customising websites
- Managing storage lifecycles
