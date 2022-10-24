# REQUESTS FOR SECURITY INFORMATION (DRAFT)

## Classification Level
Publicly available

## Review Information

__Mandatory Reivew Period__

Quarterly

__Date of Last Review__

N/A

## Purpose

Fonticons, Inc. receives regular requests to supply security related information and often fill out security questionnaires.
While we understand that this is often a part of business and security process, we do not typically provide answers to 
these questions. However, in the interest of transparency and respect for others' processes, this document lays out our 
publically available security information. We will keep this document up-to-date. Please review these contents before 
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

We consider Font Awesome to be a very low risk solution in general. The core of our offering is effectively images in an 
SVG, WOFF, or WOFF2 format. To make it easy to consume these images we have various wrappers and features built for common
technologies such as CSS, JavaScript, and various other frameworks. This aspect of our code is open source, heavily
scrutinized, and used without issue by millions of people (who have never been shy about telling us if there is a problem).
Payment information is processed via secure 3rd parties and the only information about our clients that we must store is a 
contact email address. From a privacy perspective, while using Font Awesome, we collect some logs for standard 
troubleshooting and analytics purposes but we make no attempt associate the IP information with individuals, nor do we share 
or sell the information we do have.

#### Known Security Risks Associated with Font Awesome 

The following are a set of known security risks associated with the use of Font Awesome. These are risks specific to our 
product and do not include items such as phishing attempts or look-a-like domains which are common across the Internet.

1. Access and configuration of Font Awesome is done via an online portal with authentication and authorization via username and password.
   1. An attacker compromising the user name and password can deny the user access to Font Awesome.
   1. An attacker compromising the user name and password can use Font Awesome without paying for the service.
1. SVGs are just XML; they can have embedded CSS and JavaScript which, unless otherwise configured, a browser will execute.
   1. An attacker might gain access to our database and inject malicious code into our SVGs.
   1. An attacker might execute a man-in-the-middle attack to maliciously modify an SVG in transit.
1. SVGs and WOFF/WOFF2 files are graphical in nature and may be attacked to deface a consuming website or service.
   1. An attacker might gain access to our database and inject defaced images into our SVG and WOFF/WOFF2 files resulting in defacement.
   1. An attacker might execute a man-in-the-middle attack to maliciously modify our SVG and WOFF/WOFF2 files resulting in defacement.
   1. An attacker might execute a denial-of-service attack against our infrastructure resulting in poor performance on pages using Font Awesome icons.

#### Discussion of Privacy Risks Associated with Font Awesome 

Font Awesome collects a minimal amount of personal information/data. Detailed information about what we collect is available
in our privacy policy. In general, Font Awesome collects very little information about our clients and their users, only 
enough to provide our service and make sure it isn't being over taxed. Unlike free services that use your data as a source 
of revenue, Font Awesome's only source of revenue is our clients. In general the overall privacy risk is no higher with Font 
Awesome than any other publicly available website. We maintain some logs for troubleshooting purposes and we have our own 
internal analytics. Theoretically, an attacker could gain access to that information and determine that certain IP addresses 
had connected to sites that use Font Awesome. It is our opinion that exposure of this data is only marginally more likely
than it would be by simply connecting to the site via the Internet.

#### A Quick and Easy Way to Bypass Most Security Concerns When Using Font Awesome 

One of the main benefits of using Font Awesome is that we leverage a CDN to quickly deliver icons to your site, offloading 
that work from your servers. However, this is the main interaction where there is any risk. When you set up our Kits and your 
solution directs clients to our CDN, we have to exchange some data. In this way, it is possible for us to learn potentially
peronal data/information (as defined in things like the GDPR) about you and your users.

You can completely bypass this risk by hosting Font Awesome assets yourself. While you would be losing the benefit of our 
CDN you would have effective control of the assets and no way for Font Awesome to gain any additional information about you 
or your clients. The assets would be resident on your servers and you could scan them for security vulnerabilities, etc., in
accordance with your own best security practices.

The specific instructions to self-host are here: [https://fontawesome.com/docs/web/setup/host-yourself/webfonts](https://fontawesome.com/docs/web/setup/host-yourself/webfonts) or here [https://fontawesome.com/docs/web/setup/host-yourself/svg-js](https://fontawesome.com/docs/web/setup/host-yourself/svg-jsv).

## Common Security Questions and Answers

__Will you fill out our security questionnaire__

Maybe

We are a small company and we get a lot of these questionnaires. Many times they are many pages in length and the time spent 
filling them out would not be recouped on a standard contract for many years. However, as mentioned above, we do care about
the security of our solution and want you to feel secure in your choice as well. To that end we have helpfully provided 
answers to some of the most common security questions, along with explanations. If you read this document and fill out the 
portions of your questionnaire that these answers cover, we will be happy to fill in the blanks. Unfortunately we don't have 
the resources to answer all questionnaires from scratch every time. 

__Company Name, Parent or Holding Company, etc.__

Fonticons Inc.
307 S. Main St. Suite 202
Bentonville AR 72712
United States
Not affiliated, controlled, or owned by any other entity.
No subsidiaries

__Any significant data breaches in the last 5 years__

No 

__Do we have a dedicated information security team__

No 

We are a small company and our goal is to educate our engineers to address security concerns during design and initial 
implementation.

__Do you have or maintain any security certifications__

No 

While there is value in having certifications such as SOC 2 or ISO 27001 they do not guarantee security. For example the 
2017 attack on Experian that resulted in the loss of 147 million records happened while the company had ISO 27001 
certification. The cost of many of these certifications is not commensurate with the benefit we or our clients would receive 
given the low risk nature of our solution.

__How do you determine/manage security concerns__

We use a threat modeling approach to understand the primary risks to our system. From there we make determinations about the
highest level of risk and prioritize fixes.

__Can we review your threat model__

Maybe

We do provide a sanitized and simplified version of our threat model but we hide many of the details. We are open to sharing
that information more broadly under certain circumstances, specifically those where it is clear the client understands the 
low risk nature of our solution and has concerns that cannot be easily remedied via self-hosting.

__Do you have security policies__

Yes

__What security policies do you have__

Access Control, Change Management, Incident Response, and Privacy Policies.

Some of our practices are de facto and easily enforceable in a company of our size but we are open to documenting those
practices if a valid case can be made that is both useful for us and our clients.

__Are your staff trained on security__

Yes, on this point we're somewhat proud as we are building a true security culture as opposed to simply checking a security 
training box. In general we use a Socratic method of teaching security and allow our employees to develop their own 
interests in security via a buddy system of independent verification.

There is a mandatory training schedule, but we use the time to talk and engage instead of having people watch a simple 
online training video via an LMS. We do this because our goal is mastery first, compliance second.

__What data do you collect__

Our Privacy Policy explicitly lays out what data we collect. With the exception of some optional data, everything we collect 
is required for us to provide and maintain our service. For the most part we need some basic contact information and then 
any items you plan to host. We do not store payment card information and any other potentially sensitive data, e.g., IP 
addresses are stored only temporarily for troubleshooting or anonymized, aggregated, and deleted.

__How is our data protected__

As stated above, very little data is collected. The data we do collect is generally the lowest level of sensitivity, e.g., a 
contact email address and images you plan to make available via your website, service, or app. All communication between 
you and us is encrypted via HTTPS (thus your agent has some level of responsibility in determining the level of encryption). 
However, because of the low risk nature of what we store we don't use MFA on our main site nor do we have a specific multi-
tenancy scheme in our database, etc. All systems that store or transfer data are protected with username and password for 
login and many of those do use MFA to prevent unauthorized access to client data. We currently do not encrypt our data at 
rest but we are in the process of changing that.

__With who/which Vendors do you share our data__

From a general security perspective we do not share this information freely. We are open to sharing that information more 
broadly under certain circumstances, specifically those where it is clear the client understands the low risk nature of our 
solution and has concerns that cannot be easily remedied via self-hosting. 

We do have a cloud-based infrastructure where your data is stored (temporarily or permanently) but while they host the data 
there are standard agreements in place that those vendors do not access your data. Additionally, access to those 3rd party 
providers is secured. We process payments via well known and well established 3rd party providers.

__How do you validate the security of 3rd party vendors__

We try and select vendors that have a good security track record, meet our somewhat specific needs, and generally align with 
our values.

We do not have a standardized practice for selecting vendors as we are a small company and vendors are chosen on a project
by project or need by need basis. When possible or practical, we do try to use some of the best established vendors, such as 
PayPal or Amazon.

__Since you have a cloud-based infrastructure, how do you monitor that__

We have standard monitors for our infrastructure that monitor disk, processor, and network usage. We monitor all our key 
services to validate their status. We have alerting setup when something fails or experiences a degradation in performance.
Beyond that, large portions of our infrastructure are effectively immutable which provides an additional level of security 
in general.

__Is your network segmented/zoned/secured__

Yes and no. We don't have a traditional network where users and servers are in a big office so if someone sneaks in they can
sniff sensitive stuff off the wire, etc. We have a network that is inherently segmented. For our services to talk to one 
another they must but explicitly configured to do so because most are not necessarily resident on the same network (again, 
cloud-based infrastructure with various providers).

__Do services/employees interact with one another securely__

Yes

You can't access our database or configuration for our web server or CDN without some form of authentication and 
authorization. However, some security is up to the user to implement correctly such as limiting which domains can use their
kits token for example.
