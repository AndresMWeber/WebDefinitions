# The Front End
**SEO** - **S**earch **E**ngine **O**ptimization

**CSS** - **C**ascading **S**tyle **S**heets

**SASS** - **S**yntactically **A**wesome **S**tyle **S**heets, is a preprocessor scripting language that is interpreted or compiled into *CSS*.

**SCSS** - Sassy CSS is a newer syntax for *SASS*. The formatting is similar to *CSS* with curly braces and semicolons. While the original syntax for *SASS* was more like *Python* with no curly braces and semicolons and heavy emphasis on tabbing.

**DNS** (**D**omain **N**ame **S**ervice) - when you register a domain, you can set many types of *DNS* Records.  Each record has a *Type*, a *Host*, and a *Value*

  1. **"Types"** are predefined
  1. **"Host"** represents the root (**@**) or a subdomain (**www**)
  1. **"Value"** is an IP or web address, or other value

<p align="center">
    <img width="425px" src=https://raw.githubusercontent.com/AndresMWeber/WebDefinitions/master/media/12_DNS.png>
    <img width="425px" src=https://raw.githubusercontent.com/AndresMWeber/WebDefinitions/master/media/13_DNSTypes.png>
</p>

## DNS Types:
**CNAME** - maps a subdomain to another domain name.  This can be another subdomain on the same site (like forwarding www to the root (**@**)).  Once you define a *CNAME* record for a subdomain (host), you *CAN'T DEFINE* another record for that same subdomain.  Because of this, you can't use *CNAME* at the root level (where you need other records to exist).  **CANNOT USE THIS ON THE ROOT (@)**

Ex: ```www.example.com => example.com```

**A/AAAA** - maps a subdomain to an *IPv4* address. This is most commonly used at the root, so it tells your browser where ```example.com``` lives.  **CAN DO THIS ON THE ROOT (@)**. If your domain does not have a static IP you cannot use A record.

Ex: ```example.com => 127.0.0.1```

Ex: ```example.com => ::1```

**ALIAS/ANAME/Virtual CNAME**- *ALIAS* is like *CNAME*, but it's a non-standard dns type.  So you can use *ALIAS* to forward your root domain (```example.com```) to your app's server (```example.herokudns.com```)

Ex: ```example.com => example.netlify.com```

**TXT** - *TXT* records, which provide extra info to any computer reading the *DNS* record.  *TXT* records are often used to prove you own a domain - because only the domain owner can set a *DNS* record.

Ex: ```@ => my-domain-is-awesome-123```