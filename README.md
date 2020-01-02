# Aaron Crawfis Personal Website

This repo contains the HTML for the single page application I use for my personal website, [crawfis.me](https://crawfis.me).

For a full guide on how I made my website check out my [guide on creating a website in Azure](Guide.md).

## Template

To get my website started I went over to [envato themeforest](https://themeforest.net) and grabbed the [Arlo - Personal / Portfolio / Resume Template](https://themeforest.net/item/arlo-personal-portfolio-template/23175475). This template got me started on my website. From here I replaced all of the example data with my own content.

I am using the [regular paid license](https://themeforest.net/licenses/terms/regular/2.2%20(Copy)) from envato for this website.

## Hosting

My website is hosted in an [Azure Blob Store with Static Hosting](https://docs.microsoft.com/en-us/azure/storage/blobs/storage-blob-static-website).

## CI/CD

Continuous deployment of my webapp is configured using [Azure Pipelines](https://azure.microsoft.com/en-us/services/devops/pipelines/). Upon every push/PR into master a build is triggered to copy the html folder to the blob store.