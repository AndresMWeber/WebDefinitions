# The Front End

## Site Rendering (React)

**CSR** - **C**lient **S**ide **R**endered - The client's compute power is leveraged in the browser to render the blank HTML which is filled in through the generated JavaScript React files.
![image](https://user-images.githubusercontent.com/1587270/104630545-df6d4580-5668-11eb-9391-eca6b595451f.png)


**SSR** - **S**erver **S**ide **R**endered - The server that you host the site on is responsible for rendering the page instead of the client's computer, which lessens the load on their resources and provides a more stable experience. However since the data is being fed through the server it could result in a longer latency versus something client side. You also have to run a server, however you can keep client side code and server side code in the same deployment.
![image](https://user-images.githubusercontent.com/1587270/104630552-e2683600-5668-11eb-9d15-4f6affd3d330.png)


**SSG** - **S**tatic **S**ite **G**eneration - Instead of on demand rendering, the server renders your static html at build time maximizing efficiency and load times and does not use any resources generating the content like SSR, however these pages are static.

**PR** - **P**re **R**endering - A hybrid approach of SSR and SSG where you pre-render static html files which approximate a load screen while the SSR page is rendered.
![image](https://user-images.githubusercontent.com/1587270/104660924-81a32280-5695-11eb-8145-f293763c6d8c.png)

## Site Properties/Configurations

**SEO** - **S**earch **E**ngine **O**ptimization

**CSS** - **C**ascading **S**tyle **S**heets

**SASS** - **S**yntactically **A**wesome **S**tyle **S**heets, is a preprocessor scripting language that is interpreted or compiled into _CSS_.

**SCSS** - Sassy CSS is a newer syntax for _SASS_. The formatting is similar to _CSS_ with curly braces and semicolons. While the original syntax for _SASS_ was more like _Python_ with no curly braces and semicolons and heavy emphasis on tabbing.

**DNS** (**D**omain **N**ame **S**ervice) - when you register a domain, you can set many types of _DNS_ Records. Each record has a _Type_, a _Host_, and a _Value_

1. **"Types"** are predefined
1. **"Host"** represents the root (**@**) or a subdomain (**www**)
1. **"Value"** is an IP or web address, or other value

<p align="center">
    <img width="425px" src=https://raw.githubusercontent.com/AndresMWeber/WebDefinitions/master/media/12_DNS.png>
    <img width="425px" src=https://raw.githubusercontent.com/AndresMWeber/WebDefinitions/master/media/13_DNSTypes.png>
</p>

## DNS Types:

**CNAME** - maps a subdomain to another domain name. This can be another subdomain on the same site (like forwarding www to the root (**@**)). Once you define a _CNAME_ record for a subdomain (host), you _CAN'T DEFINE_ another record for that same subdomain. Because of this, you can't use _CNAME_ at the root level (where you need other records to exist). **CANNOT USE THIS ON THE ROOT (@)**

Ex: `www.example.com => example.com`

**A/AAAA** - maps a subdomain to an _IPv4_ address. This is most commonly used at the root, so it tells your browser where `example.com` lives. **CAN DO THIS ON THE ROOT (@)**. If your domain does not have a static IP you cannot use A record.

Ex: `example.com => 127.0.0.1`

Ex: `example.com => ::1`

**ALIAS/ANAME/Virtual CNAME**- _ALIAS_ is like _CNAME_, but it's a non-standard dns type. So you can use _ALIAS_ to forward your root domain (`example.com`) to your app's server (`example.herokudns.com`)

Ex: `example.com => example.netlify.com`

**TXT** - _TXT_ records, which provide extra info to any computer reading the _DNS_ record. _TXT_ records are often used to prove you own a domain - because only the domain owner can set a _DNS_ record.

Ex: `@ => my-domain-is-awesome-123`
