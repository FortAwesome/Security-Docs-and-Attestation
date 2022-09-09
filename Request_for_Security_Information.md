# REQUESTS FOR SECURITY INFORMATION (DRAFT)

## Purpose

Fonticons Inc recieves regular requests to supply security related information and often fill out security questionnaires.
While we understand that this is often a part of business and security process, we do not typically provide answers to 
these questions.  However, in the interest of transparency and respect for other's processes, this document lays out our 
publically available security information.  We will keep this document up-to-date.  Please review these contents before 
requesting additional security information. 

## Font Awesome Security 

### Security Mission Statements

* We are committed to clear and easy to understand policies and statements around security so you can make informed decisions about the use of Font Awesome.
* We define security as actions taken to prevent a reduction or loss of value of an asset.
* We believe in doing the right thing for ourselves and our clients.
* We will take the necessary steps to protect all client assets in our care but will prefer the actual security action as opposed to a compliance, auditing, or management schemes.
* We will prefer to minimize the assets under our care.

### Understanding the Risk Associated with the Use of Font Awesome 

#### Font Awesome is Low Risk 

We consider Font Awesome to be a very low risk solution in general.  The core of our offering is effectively images in an 
SVG, WOFF, or WOFF2 format.  To make it easy to consume these images we have various wrappers and features built for 
common technologies such as CSS, JavaScript, and various other frameworks.  This aspect of our code is opensource, heavily
scrutinized, and used without issue by millions of people (who have never been shy about telling us if there is a problem).
Payment information is processed via secure 3rd parties and the only information about our clients that we must store is a 
contact email address.  From a privacy perspective, while using Font Awesome, we collect some logs for standard 
troubleshooting and analytics purposes but we make no attempt associate IP information with individuals, nor do we share 
or sell the information we do have.  Even if we did, we're not certain in what case anyone would care if a person happened 
to visit a site that happened to serve some awesome icons.

#### Known Security Risks Associated with Font Awesome 

The following are a set of known security risks associated with the use of Font Awesome.  These are risks specific to our 
product and do not include items such as phishing attempts or look-a-like domains which are common across the Internet.

1. Access and configuration of Font Awesome is done via an online portal with authentication and authorization via user name and password.
   1. An attacker compromising the user name and password can deny the user access to Font Awesome.
   1. An attacker compromising the user name and password can use Font Awesome without paying for the service.
1. SVGs are just XML; they can have embedded CSS and JavaScript which, unless otherwise configured, a browser will execute.
   1. An attacker might gain access to our database and inject malicious code into our SVGs.
   1. An attacker might execute a man-in-the-middle attack to maliciously modify an SVG in transit.
1. SVGs and WOFF/WOFF2 files are graphical in nature and may be attacked to deface a consuming website or service.
   1. An attacker might gain access to our database and inject defaced imagegs into our SVG and WOFF/WOFF2 files resulting in defacement.
   1. An attacker might execute a man-in-the-middle attack to maliciously modify our SVG and WOFF/WOFF2 files resulting in defacement.
   1. An attacker might execute a denial of service attack against our infrastructure resulting in poor performance on pages using Font Awesome icons.

## Common Security Questions and Answers

__Company Name, Parent or Holding Company, etc.__
Fonticons Inc.
307 S. Main St. Suite 202
Bentonville AR 72712
United States
Not affliated, controlled, or owned by any other entity.
No subsidiaries

__Any significant data breaches in the last 3 years__
No 

__Do we have a dedicated information security team__
No 
We are a small company and our goal is to educate our engineers to address security concerns during design and initial 
implementation.

__Do you have or maintain any security certifications__
No 
While there is value in having certifications such as SOC 2 or ISO 27001 they do not guarantee security.  For example the 
2017 attack on Experian that resulted in the loss of 147 million records happened while the company had ISO 27001 
certification.  The cost of many of these certifications is not comenserate with the benefit we or our clients would receive 
given the low risk nature of our solution.

