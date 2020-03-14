# Initial Installation

If you have completed the Scratch deployment on Cloud Platform, the following steps is for you to start use it quikly

## Preparation

1. Get the **Internet IP** on your Cloud Platform
2. Check you **[Inbound of Security Group Rule](https://support.websoft9.com/docs/faq/tech-instance.html)** of Cloud Console to ensure the TCP:80 is allowed
3. Make a domain resolution on your DNS Console if you want to use domain for Scratch

## Scratch Installation Wizard

1. Using local Chrome or Firefox to visit the URL *http://Domain* or *http://Internet IP*, you can use Scratch
   ![Scratch GUI](https://libs.websoft9.com/Websoft9/DocsPicture/en/scratch/scratch-gui-websoft9.png)

2. Scratch loads data for more than 20M for the first time. If your network bandwidth is insufficient, the loading will be slow and wait patiently.

> More useful Scratch guide, please refer to [Scratch Documentation](https://en.scratch-wiki.info)

## Q&A

#### I can't visit the start page of Scratch?

Your TCP:80 of Security Group Rules is not allowed so there no response from Chrome or Firefox

#### Is Scratch open very slowly?

Scratch first loaded data over 20M. For example, if you are using 2M bandwidth, then the ideal load time is: 2000k / (128k/s × 2) = 7.8s. Obviously, if the bandwidth is insufficient, the speed will be very slow.