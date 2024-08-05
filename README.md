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
