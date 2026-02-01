# REQUESTS FOR SECURITY INFORMATION

## Classification Level

Publicly available

## Review Information

__Mandatory Review Period__

Semi-Annually

__Date of Last Review__

February 1, 2026

## Purpose

Fonticons, Inc. receives regular requests to supply security related information and often fill out security questionnaires.
While we understand that this is often a part of business and security process, we do not typically provide answers to 
these questions. However, in the interest of transparency and respect for others' processes, this document lays out our 
publicly available security information. We will keep this document up-to-date. Please review these contents before 
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
personal data/information (as defined in things like the GDPR) about you and your users.

You can completely bypass this risk by hosting Font Awesome assets yourself. While you would be losing the benefit of our 
CDN you would have effective control of the assets and no way for Font Awesome to gain any additional information about you 
or your clients. The assets would be resident on your servers and you could scan them for security vulnerabilities, etc., in
accordance with your own best security practices.

The specific instructions to self-host are here: [https://fontawesome.com/docs/web/setup/host-yourself/webfonts](https://fontawesome.com/docs/web/setup/host-yourself/webfonts) or here [https://fontawesome.com/docs/web/setup/host-yourself/svg-js](https://fontawesome.com/docs/web/setup/host-yourself/svg-jsv).

## Common Security Questions and Answers

### General Information

__Will you fill out our security questionnaire__

Maybe

See our security questionnaire policy here: [Security Questionnaire Policy](https://github.com/FortAwesome/Security-Docs-and-Attestation/blob/main/Security_Questionnaire_Policy.md)

__Company Name, Parent or Holding Company, etc.__

Fonticons Inc.
307 S. Main St. Suite 202
Bentonville AR 72712
United States
Not affiliated, controlled, or owned by any other entity.
No subsidiaries

__General Contact Information__

General help & support, including security requests: [help@fontawesome.com](mailto:help@fontawesome.com)
General privacy questions: [privacy@fontawesome.com](mailto:privacy@fontawesome.com])
Data Protection Officer: [dpo@fontawesome.com](mailto:dpo@fontawesome.com)

### Services Overview

| Technology / Service              | Category                    | Usage in Font Awesome                                                                        |
| --------------------------------- | --------------------------- | -------------------------------------------------------------------------------------------- |
| Elixir & OTP                      | Language / Runtime          | Primary backend runtime for the Font Awesome application, releases, and supervision tree.    |
| Phoenix & LiveView                | Web framework               | HTTP endpoints, templating, and real-time dashboards for the customer portal and APIs.       |
| Node.js + Webpack/Babel           | Frontend build tooling      | Asset pipeline for bundling, linting, and testing the Vue-based UI.                          |
| Vue 2 + Vuex + Vue Router         | Frontend application        | Renders dashboard, kit builder, and account management screens with shared state management. |
| Apollo GraphQL + JSON:API clients | API consumption             | Frontend retrieves icon metadata and account data via GraphQL and JSON:API endpoints.        |
| Redis                             | Cache / session store       | Stores kit state, CDN flags, and other fast-changing data through Redix pools.               |
| Oban Pro/Web                      | Background jobs             | Manages scheduled kit builds, downloads, and cleanup workflows.                              |
| AWS S3 via ExAws                  | Object storage              | Provides buckets for kit assets and Stripe log archival.                                     |
| SendGrid                          | Email delivery              | Sends transactional, marketing, and feedback email from the platform.                        |
| Stripe                            | Payments                    | Handles subscription billing, price overrides, and webhook verification.                     |
| Braintree                         | Payments                    | Supports drop-in card collection and related rate-limited endpoints.                         |
| PayPal                            | Payments                    | Alternative checkout flow with webhook verification.                                         |
| Algolia + InstantSearch           | Hosted search               | Powers icon/library search experiences in the app.                                           |
| Cloudsmith API                    | Package distribution        | Uploads, publishes, and monitors kit npm packages.                                           |
| Google Analytics + reCAPTCHA      | Tracking & abuse prevention | Toggles GA tracking, implements vue-gtag, and secures auth forms with reCAPTCHA.             |
| GitHub OAuth & GraphQL APIs       | Developer integration       | Links customer accounts to GitHub for OAuth flows and metadata sync.                         |
| Guardian JWT + Phoenix session    | Authentication              | Issues and validates JWTs plus secure cookies for user sessions.                             |

### Service Details

Below are the services we provide along with details about the services germane to security concerns

__Icon Library & Tooling__

A web application that helps search, browse, and implement icons as part of a broader toolkit for designers and developers.

__Kits__

Scripts that load and make icon assets easily and programmatically available via our servers.

[https://docs.fontawesome.com/web/setup/get-started/](https://docs.fontawesome.com/web/setup/get-started/)

__Self-Hosted Icon Collections & Tools__

A collection of icons in various formats as well as JavaScript, CSS, and other wrappers packaged for use in your website or
application. These resources are available from our web application or via npm, yarn, pnpm, etc.

[https://docs.fontawesome.com/web/dig-deeper/conflict-detection/](https://docs.fontawesome.com/web/dig-deeper/conflict-detection/)
[https://docs.fontawesome.com/web/setup/packages/](https://docs.fontawesome.com/web/setup/packages/)

__APIs__

1. JavaScript API for advanced control using the SVG+JS method (layering, counters, subsetting/tree-shaking, etc.). 
1. GraphQL API to programmatically retrieve icon/release metadata (and account/kit data with auth). 
1. Conflict Detection API for diagnosing conflicts when other Font Awesome versions are present.

[https://docs.fontawesome.com/apis/](https://docs.fontawesome.com/apis/)

__Plugins__

1. Official WordPress plugin with guidance for using Kits, Pro icons, uploaded icons, and troubleshooting conflicts. 
1. Official Figma plugin to search and insert icons as SVGs (and optionally include Kit custom icons for Pro users). 
1. Framework components (React/Vue/Angular/etc.) maintained under the FortAwesome GitHub org.

[https://docs.fontawesome.com/web/use-with/wordpress/](https://docs.fontawesome.com/web/use-with/wordpress/)
[https://docs.fontawesome.com/desktop/add-icons/figma-plugin/](https://docs.fontawesome.com/desktop/add-icons/figma-plugin/)
[https://github.com/FortAwesome](https://github.com/FortAwesome)

### Service Technology Details

__Icon Formats & Rendering Toolkits__

1. SVG, webfonts and CSS toolkits
1. SVG+JS rendering and JavaScript API

__Package Distribution & Developer Tooling__

1. Package-manager distribution (npm/yarn/pnpm) for Font Awesome packages, including Kit Packages.
1. Kit Packages delivered as installable packages (@awesome.me/kit-*) with assets and configuration with modern package exports.
1. Tokens for controlled access (package-manager tokens and API tokens for third-party apps).

__Public APIs__

1. GraphQL API hosted at api.fontawesome.com.
1. JavaScript API and method references (e.g., layering/counters/tree-shaking, and SVG+JS usage).

__Edge Network and Operational Infrastructure__

1. Cloudflare CDN used for icon delivery.
1. Cloudflare Load Balancing used to keep icon delivery performant and resilient.
1. Cloudflare Workers for GraphQL API under high load.
1. Phoenix framework and Docker.

### Security History and Posture

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
highest level of risk and prioritize fixes. This is roughly aligned with NIST practices but, as a small firm we can either
focus on actual security or compliance.

__Can we review your threat model__

Maybe

We do provide a sanitized and simplified version of our threat model but we hide many of the details. We are open to sharing
that information more broadly under certain circumstances, specifically those where it is clear the client understands the 
low risk nature of our solution, has concerns that cannot be easily remedied via self-hosting or some other means, and
understands and agrees to not store sensitive security information about our organization without agreed upon controls, etc.

__Do you have security policies__

Yes

__What security policies do you have__

Access Control, Change Management, Incident Response, and Privacy Policies, etc.

Some of our practices are de facto and easily enforceable in a company of our size but we are open to documenting those
practices if a valid case can be made that is both useful for us and our clients. These policies are found in the same 
directory as this document.

__Are your staff trained on security__

Yes, on this point we're somewhat proud as we are building a true security culture as opposed to simply checking a security 
training box. In general we use a Socratic method of teaching security and allow our employees to develop their own 
interests in security via a buddy system of independent verification.

There is a mandatory training schedule, but we use the time to talk and engage instead of having people watch a simple 
online training video via an LMS. We do this because our goal is mastery first, compliance second.

### Data Collection and Security

__What access do you require to our network/infrastructure__

None.

In general, we do not need any direct access to your network or infrastructure. Your developers and designers will either
download the assets they require and use them on your project or add a kit code in your site or web application. This also
means that we don't offer an SSO feature and any communication between you and us is done via a password based login or a
token.

__What data do you collect__

Our Privacy Policy explicitly lays out what data we collect. With the exception of some optional data, everything we collect 
is required for us to provide and maintain our service. For the most part we need some basic contact information and then 
any items you plan to host. We do not store payment card information and any other potentially sensitive data, e.g., IP 
addresses are stored only temporarily for troubleshooting or anonymized, aggregated, and deleted.

Please review the following for more details:

* https://fontawesome.com/tos
* https://fontawesome.com/privacy
* https://fontawesome.com/support#dpfPrinciples
* https://fontawesome.com/support#dataCollectionDetail

__How is our data protected__

As stated above, very little data is collected. The data we do collect is generally the lowest level of sensitivity, e.g., a 
contact email address and images you plan to make available via your website, service, or app. All communication between 
you and us is encrypted via HTTPS (thus your agent has some level of responsibility in determining the level of encryption). 
However, because of the low risk nature of what we store we don't use MFA on our main site nor do we have a specific multi-
tenancy scheme in our database, etc. All systems that store or transfer data are protected with username and password for 
login and many of those do use MFA to prevent unauthorized access to client data. We currently do not encrypt our data at 
rest but we are in the process of changing that.

Additionally, from a risk management and general security perspective, confidentiality is not and likely should not be the 
primary concern except for items like tokens and passwords. In general, the data you provide us is meant to be shared on
your site, application, or web application making they primary concern integrity and availability. To that end, while we do
protect some of your information, the main purpose of our service is to distribute what you provide us.

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
