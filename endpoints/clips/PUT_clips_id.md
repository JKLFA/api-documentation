# Modify clip - [Clip](https://github.com/kippt/api-documentation/blob/master/objects/clip.md) object

    PUT /api/clips/:clip_id/

## Description

Modify a clip. See [Clip](https://github.com/kippt/api-documentation/blob/master/objects/clip.md) object for fields which can be modified.

## Authentication required

Authentication required.

## Parameters

- _None_

## Example
**Request**

    PUT /api/clips/11267138/

    {
        "title": "When Did Twitter Grow Up?",
        "notes": "Good read about Twitter in 2013"
    }

**Return**

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
        title: "When Did Twitter Grow Up?",
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
        notes: "Good read about Twitter in 2013",
        list: "/api/lists/13/",
        resource_uri: "/api/clips/11267138/"
    }