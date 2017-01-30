---
title: Billing information 
keywords: 
last_updated: November 18, 2016
tags: 
summary: 
sidebar: crs_sidebar
permalink: crs-billing.html
folder: crs
toc: false
---

{% include note.html content="Information on pricing can be found at [IBM Cloud](https://www.ibm.com/cloud-computing/products/storage/object-storage/public-service/#othertab2){:new_window}." %}

### Invoices
Account invoices can be found at **Account** > **Billing** > **Invoices** in the navigation menu.

{% include tip.html content="Each account receives a single bill. If you need separate billing for different sets of containers, then creating multiple accounts is necessary." %}

### How does IBM COS pricing work?

Storage costs for IBM COS are determined by total volume of data stored, the amount of public outbound bandwidth consumed, and the total number of operational requests processed by the system.

{% include important.html content="Bluemix infrastructure offerings are connected to a three-tiered network, segmenting public, private, and management traffic. Infrastructure on a customer's Bluemix account may transfer data between one another across the private network at no cost. Infrastructure offerings (such as bare metal servers, virtual servers, and cloud storage) connect to other applications and services in the Bluemix catalog (such as Watson services, containers, runtimes) across the public network, so data transfer between those two types of offerings is  metered and charged at standard public network bandwidth rates." %}

### What is the difference between 'Class A' and 'Class B' requests?

'Class A' requests are operations that involve modification or listing.  This includes creating buckets, uploading or copying objects, creating or changing configurations, listing buckets, and listing the contents of buckets.

'Class B' requests are those related to retrieving objects or their associated metadata/configurations from the system.

There is no charge for deleting buckets or objects from the system.

| Class | Requests | Examples |
|--- |--- |--- |
| Class A | PUT, COPY, and POST requests, as well as GET requests used to list buckets and objects | Creating buckets, uploading or copying objects, listing buckets, listing contents of buckets, setting ACLs, and setting CORS configurations |
| Class B | GET (excluding listing), HEAD, and OPTIONS requests | Retrieving objects and metadata |

### What is the difference between the Standard and Vault billing tiers?
 
Vault billing is a way to control costs for infrequently accessed data, such as compliance or backup data. These objects incur lower storage costs but higher costs for operational requests. Unlike the Standard billing tier, additional costs are incurred on a per-GB basis for objects retrieved from the system.  