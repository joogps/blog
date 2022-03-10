# blog <a href="https://blog.joogps.codes"> <img src="https://img.shields.io/static/v1?label=open&message=blog.joogps.codes&color=blue"> </a>
This repository stores the JavaScript [worker code](https://github.com/joogps/blog/blob/main/index.js) that serves my Notion blog on Cloudflare.

## How does it work?
First, I have my [Notion](https://notion.so) blog set up as a [public page](https://blog.joogps.codes) in my Workspace. To serve it in a custom domain, I used the free [Fruition](https://fruitionsite.com) script hosted on a Cloudflare Worker. The domain used is the same as the one from my personal website, but with an added `.blog` subdomain.

A wrangler deploy GitHub action is executed at every branch push, so that the code always stays up to date. The code for the action can be found in the repository.
