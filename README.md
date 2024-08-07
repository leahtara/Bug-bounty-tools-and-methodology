# Bug-bounty-tools-and-methodology
#### Tools to use in each phase of a bug bounty

What to do after choosing a target...

## Recon

Go through the scope of the target (very important)


### Subdomain Enumeration 
The goal is to find the subdomains that exist which other people are not finding.
You can make a custom script to combine many tools together (Either code it (python or bash) or use chatgpt).
Tools:
[assetfinder](https://github.com/tomnomnom/assetfinder.git)
[crtsh](https://github.com/YashGoti/crtsh.git)
[github-subdomains](https://github.com/gwen001/github-subdomains.git)
To remove duplicate subdomains: [anew](https://github.com/tomnomnom/anew.git)

Now to find the working subdomainsfrom the subdomain list, use either [httpx](https://github.com/projectdiscovery/httpx.git) or [httprobe](https://github.com/tomnomnom/httprobe.git)


### Automatic scanners
Run automatic scanners on the subdomains (unless instructed not to) Nuclei, Nikto, Nmap. These give you a rough idea of the target.

### Finding known tech
We already know a lot about the tech used from the automatic scanners. For more info: wappalyzer, builtwith, whatruns. After finding the versions for all the tech, we can search for any known vulnerabilities and report it.

### Tools for known bugs
Now some automatic tools that can be run to find the basic bugs in the subdomains. [Subdomain takeover](https://github.com/PentestPad/subzy.git), [Broken Link Hijacking](https://github.com/utkusen/socialhunter.git), [XSS](https://github.com/devanshbatham/ParamSpider.git), Open Redirect, Paramspider.

### Screenshots
[Aquatone](https://github.com/michenriksen/aquatone.git) for getting screenshots of all the subdomains.

