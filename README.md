# eladbash.com

## Deployment
Auto CD when pushing to master - by aws code pipeline (an AWS app is installed on this repo to listen to changes on master)
The deploy takes all the changes and push it to S3 bucket that serves eladbash.com

## Troubleshooting
If after the push you don't see any changes - check cloudfront and invalidate it's cache.
