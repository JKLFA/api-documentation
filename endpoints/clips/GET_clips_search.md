# Search own clips - [Clip](https://github.com/kippt/api-documentation/blob/master/objects/clip.md) collection

    GET /api/clips/search/

## Description

Search user's clips, both public and private.

## Authentication required

As this endpoint return clips for currently logged in user, authentication is required

## Parameters

Both <code>list</code> and <code>via</code> data for clips can be embedded into response.

- <code>q</code> - Search parameter
- <code>include_data</code>
    - <code>list</code>
    - <code>via</code>
    - <code>media</code>

E.g.

    GET /api/clips/search/?q=css+html&include_data=list,via

## Example
**Request**

[GET /api/clips/search/?q=twitter](https://grandcentral.kippt.com/api/clips/search/?q=twitter&include_data=media)

**Return**

    {
        {
            next: "/api/clips/search/?q=twitter&limit=20&offset=20",
            total_count: 96,
            previous: null,
            limit: 20,
            offset: 0
        },
        objects: [
            {
                via: null,
                saves: {
                    count: 0,
                    data: [ ]
                },
                favicon_url: "https://www.google.com/s2/u/0/favicons?domain=adage.com",
                is_favorite: false,
                likes: {
                    count: 0,
                    data: [ ]
                },
                id: 11267138,
                app_url: "/jorilallo/awesome/clips/11267138",
                title: "When Did Twitter Grow Up? - Advertising Age",
                media: {
                    description: "As a cultural force, Twitter has logged many defining moments. But as an ad platform and marketing tool, Twitter's coming-of-age appears to be happening now. That news stories like the hacking of the Jeep and Burger King Twitter accounts generated so much heat last week tells you how much brands have made Twitter part of their marketing infrastructure.",
                    title: "When Did Twitter Grow Up? | Digital - Advertising Age",
                    provider: {
                        url: "https://kippt.com",
                        name: "Kippt"
                    },
                    images: {
                    tile: {
                        url: "https://d19weqihs4yh5u.cloudfront.net/links/98d15454fc0d17322a66b2f2b9e042e5613d13fe/350x200",
                        width: 350,
                        height: 200
                    },
                    original: {
                        url: "https://d19weqihs4yh5u.cloudfront.net/links/98d15454fc0d17322a66b2f2b9e042e5613d13fe/original",
                        width: 100,
                        height: 67
                    }
                },
                type: "link"
                },
                comments: {
                    count: 0,
                    data: [ ]
                },
                type: null,
                updated: 1361811656,
                user: {
                    username: "jorilallo",
                    bio: "Co-founder of Kippt. I love building products.",
                    twitter: "jorilallo",
                    counts: {
                        follows: 1059,
                        followed_by: 20670
                    },
                    full_name: "Jori Lallo",
                    dribbble: "jorilallo",
                    id: 1,
                    app_url: "/jorilallo",
                    github: "jorde",
                    avatar_url: "http://kippt-image-vault.herokuapp.com/vaults/avatars/images/147d86b9-0830-49d8-a449-0421a6a4bf05/sizes/160x160",
                    is_pro: true,
                    website_url: "http://about.me/jorilallo",
                    resource_uri: "/api/users/1/"
                },
                url_domain: "adage.com",
                created: 1361811131,
                url: "http://adage.com/article/digital/twitter-grow/239992/",
                notes: "",
                list: "/api/lists/13/",
                resource_uri: "/api/clips/11267138/"
            },
            ...
        ]
    }