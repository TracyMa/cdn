# Limits {#concept_um5_wdx_wdb .concept}

## Restrictions on the use of CDN {#section_zhn_q2x_wdb .section}

1.  Real-name registration must be performed for accounts on the Alibaba Cloud official website.
2.  A CDN domain must have an [ICP license](https://www.alibabacloud.com/icp?spm=a2796.7919406.1097650.dznavsolutions13.42552d23kqZiTG) and be connected to Alibaba Cloud.
3.  The origin site content of a CDN domain must be stored on Elastic Compute Service \(ECS\) or Object Storage Service \(OSS\).  If the origin site content is not stored on Alibaba Cloud, access must be reviewed.

**Domain Name reviewing standards**

All domains attempting to access CDN must be reviewed. CDN access is not allowed in any of the following scenarios:

-   The CDN domain cannot be accessed or the content does not include any substantive information.
-   The CDN domain is for a private game server.
-   The CDN domain is used for role playing games or card games.
-   The CDN domain name is for website that has no download rights such as pirate software
-   The CDN domain is for a P2P website.
-   The CDN domain is for a lottery website.
-   The CDN domain is for an illegal hospital or pharmaceutical website.
-   The CDN domain is for a site involving porn, gambling, drugs, etc.

**Note:** The losses incurred by attacks or malicious download because the CDN domain name does not comply with the previous rules will be born on you, and Alibaba Cloud CDN carries no responsibilities.

-   Domains that have accessed Alibaba Cloud CDN will be reviewed regularly. If any of these violations are detected, the system immediately terminates the CDN acceleration of the domain name, and stops the CDN service for all your domain names at the same time.
-   If your CDN domain name cannot be accessed normally or is denied due to reason which does not contain any substantive information, and your business is a compliance business, you can submit a ticket, and send the screenshots of the web site business content\(which contains the domain name\) through the ticket. After the ticket is reviewed separately, you will be informed of the results of the second audit.

## Restriction {#section_r1h_lgx_wdb .section}

|Quantity|Limit quantity|
|:-------|:-------------|
|Domain Name|The maximum number of CDN domains for each Alibaba Cloud account is **50** . |
|IP origin site|The maximum number of IP origin sites for each CDN domain is **10**.|
|Cache refresh and push operations|**refresh:**2000items/day/account. **Directory refresh:**100 items/day/account.|

If you have a large number of domain name acceleration needs, submit a ticket for special support.

## CDN domain name reclaiming rules {#section_p3p_qgx_wdb .section}

|If your CDN domain name...|The system will...|To continue using CDN acceleration, you must...|
|:-------------------------|:-----------------|:----------------------------------------------|
|not access traffic for more than 90 days \(including "normal operation"\)|Automatically deactivate the domain name to save the CDN domain name related records|Enable  CDN domain names.|
|Is in the disabled state for more than 120 days \(including auditing failed\)|Automatically delete the domain name related records.|Re-add the domain name.|

