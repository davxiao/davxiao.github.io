---
layout: post
title:  "AWS IAM Essentials"
date:   2018-12-11
author: David Xiao
categories: cybersecurity aws iam
tags:  cybersecurity aws iam
---

IAM group

They exist solely to make it easier to manage user permissions

IAM user credential

IAM users can have any combination of credentials that AWS supports, such as an AWS access key, X.509 certificate, SSH key, password for web app logins, or an MFA device. This allows users to interact with AWS in any manner that makes sense for them. An employee might have both an AWS access key and a password; a software system might have only an AWS access key to make programmatic calls; IAM users might have a private SSH key to access AWS CodeCommit repositories; and an outside contractor might have only an X.509 certificate to use the EC2 command-line interface. For details, see Temporary Security Credentials in the IAM documentation.