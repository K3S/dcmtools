## Purpose

I have created this guide as a reference on how to create and install SSL certificates for the [IBM i OS](https://en.wikipedia.org/wiki/IBM_i) with the command line DCM Tools. Understanding the current encryption offerings, setup, and what everything means is kinda confusing. The current GUI tools for DCM is... ok. The hope of this guide is to make it significantly easier to understand, use, and issue your own certificate OR incorporate [Let's Encrypt](https://letsencrypt.org/), a free service to provide SSL certificates.

Notably, thank you to [Jesse Gorzinski](https://twitter.com/IBMJesseG){:target="_blank" rel="noopener"}, for developing such great tools! 

## Synopsis

From a high level were going to create a certificate as our own Certificate Authority (CA) or on Let's Encrypt, import it via command line tools onto the IBM i, make it available for applications, and then apply it to an Apache instance, 5250, System Navigator, and HMC. 

## What does it mean to encrypt our applications?

In a very 'plain but somewhat innacurate' way of explaining when first designed the web applications we all use and function with were designed to transmit the information back and forth between the server and client in easy to read data. This is so easy to read that someone could watch the traffic and see exactly what was being transmitted back and forth. If you were to type a password an viewer could watch the stream and literally see your password. To fix this technologies like SSL was created to encrypt all the traffic between the server and client so only the server and client know what is being sent back and forth. SSL is not the first, but has the main standard used today. 

The basic concept of SSL is that you request a certificate from a Certificate Authority (usually referred to as a CA). If you create the CA yourself, this is called a 'self signed' certificate. You can also pay to get a certificate from a publicly trusted CA. These publicly trusted CAs usually charge for their certificates, and depending on the repuation of the CA and purpose they can charge a lot of money for the certificate. 

Let's Encrypt is a publicly trusted CA whose goal is to help encrypt the entire internet freely. This guide will focus on either self signing or using Let's Encrypt. If you were looking to use a different publicly trusted CA, just transpose the instructions over to that CA. 

## Creating the Certificate 

### Creating the Certificate on Let's Encrypt

### Create a CA

### Create a Certificate from your own CA

## Import Your Certificate

## Apply Certificate to Apache

## Apply Certificate to ACS 5250


# About K3S (King III Solutions, Inc)

[K3S](https://k3s.com) is a software development company that specializes in inventory management and procurement solutions for the distribution industry. Their applications and solutions are developed to run on the IBM i OS (the best enterprise level OS!) and interface with any ERP application on any platform. 

As well K3S open sources many of its [Guides & Utilities ](https://technical.k3s.com/docs/utilities/) in an effort to improve the IBM i community. 
