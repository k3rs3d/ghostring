# 👻 Ghostring 👻

This is a webring for horror/witchy themed sites. 

It also serves as an example for how to configure and use the [ringfairy](https://github.com/k3rs3d/ringfairy/) webring generator. You can use this repo as a starting point to launch your own webring!  

## [Visit the webring here!](https://ghostring.neocities.org)

Signups are currently **open**!

## How to Join 
The only required information is your site's **URL** and your desired **slug** (a keyword for your site, e.g. "kersed" for kersed.net).

Optionally, you can also include the following for your site listing: 

- Full **title** of your site
- A brief **description** of your site
- Some form of **contact info** (email, fedi, neocities, etc)
- If you have one, your **RSS** link

Include your information by adding a new entry to *`websites.json`* in a pull request.

### JSON Example

```json
    {
        "name": "Example Website",
        "slug": "example",
        "about": "I'm an example!!! ",
        "url": "https://example.com/",
        "rss": "https://example.com/index.xml"
        "owner": "person@example.com"
    }
```

## Webring HTML

After that, add the webring HTML somewhere on your site, like the sidebar or footer. 
Remember to replace "YOUR_SLUG" with your actual slug: 

```html
<a href="https://ghostring.neocities.org/YOUR_SLUG/previous"><-</a><a href="https://ghostring.neocities.org/">Ghostring</a><a href="https://ghostring.neocities.org/YOUR_SLUG/next">-></a> 
```

It's crucial that every site in the webring has these links (with their slug) accessible on the front page. [Ringfairy](https://github.com/k3rs3d/ringfairy/) will only add your site to the webring if the links can automatically be found. Without the proper links, the ring structure would be broken, and that site would need to be removed from the list. 

## Cloning 

You may clone this repo if you want a starting point for your own ringfairy-based webring, or if you want to make a backup/mirror of Ghostring. 

You can create your own webring by replacing `websites.json` with your own list of sites, and editing the HTML/CSS files in the `/data` folder!

However, this repo doesn't include [ringfairy](https://github.com/k3rs3d/ringfairy/) binaries. To generate a webring yourself, you'll need to download or compile [ringfairy](https://github.com/k3rs3d/ringfairy/) separately. 
