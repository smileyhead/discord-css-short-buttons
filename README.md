# discord-css-short-buttons
This is a simple CSS tweak for Discord to shorten the oversized buttons at the top of the DMs page. You may use it with Vencord, BetterDiscord, or your favourite CSS modifier extension.

It has been bugging me how uselessly large these buttons on the top of the Direct Messages page were, taking vertical space from the thing you probably actually care about: people. This tweak will shorten those buttons to around the same height as the channel list entries on a server (guild).

| Before | After |
| --- | --- |
| <img width="209" height="312" alt="image" src="https://github.com/user-attachments/assets/2e3eb2f3-e710-4f9e-b4af-5c9218d53323" /> | <img width="209" height="312" alt="image" src="https://github.com/user-attachments/assets/6dd472d4-2cba-48d0-8d63-b2e31c0fb172" /> |

```CSS
/* Smaller DM page top buttons */
a[data-list-item-id$="_friends"],
a[data-list-item-id$="_library"],
a[data-list-item-id$="_messageRequests"],
a[data-list-item-id$="_nitro"],
a[data-list-item-id$="_shop"],
a[data-list-item-id$="_quests"] {
    padding-top: 3px !important;
    padding-bottom: 3px !important;
}
```

It's not the cleanest, but it works.
