# nginx-for-s3-and-lambda
Example of configuration for nginx as reversed proxy with cache for Amazon Cloud Front and API Gateway.
As single web page application with javascript is normally badly received by google bot - I have used prerendered website served from external server (prerenderer.io) only from bot.
The static files are served via Amazon CloudFront to Amazon S3. The dynamic AJAX requests are served via api.example.com via reversed nginx proxy. The api gateway for amazon lambda needs to be provided as well like cloud front endpoint and prerenderer token.
