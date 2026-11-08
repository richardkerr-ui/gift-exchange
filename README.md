# Gift exchange draw

One web page. No server, no accounts, no tracking. Built so a helper does the setup and a not-so-techy organizer only has to tap big buttons.

## 1. Put it online (helper, about 5 minutes)

The page has to be online so the links open on everyone's phone.

GitHub Pages:

1. Create a new public repo on GitHub, for example `gift-exchange`.
2. Upload `index.html` to it.
3. Settings → Pages → Source: "Deploy from a branch", branch `main`, folder `/ (root)`. Save.
4. After a minute the page is at `https://<your-username>.github.io/gift-exchange/`.

Netlify Drop also works: drag this folder onto https://app.netlify.com/drop.

Links carry their data after a `?` (iPhone Messages link previews drop anything after a `#`, so `#` links broke). That means the website host receives each link when it's opened:

- **Personal links:** each one holds that person's result in readable form, so the link itself is the secret. The organizer sends it to that person only, as a private Telegram message.
- **Wishlist links:** the wishlist inside is encrypted, so the host only sees scrambled data.
- **Setup link:** names, phone numbers and couples are readable.
- **Backup link:** everything, including who has who, is readable.

The host here is GitHub Pages, which doesn't publish these requests, but keep the setup and backup links between the helper and the organizer, and never post a personal link in a group chat.

## 2. Set it up (helper)

Open the online page and fill in:

- The exchange name, spending limit and gift day
- The organizer's name, plus your own name and phone so they can message you for help
- Everyone in the exchange. Phone numbers are optional but worth it. Add the country code, like `+1 555 123 4567`. The organizer's Telegram button then opens a chat with each person with the message already filled in.
- Couples to keep apart
- Last year's results file or backup link, if you have one, so nobody gets the same person again

Tap **Send to [organizer]** and send them the message on Telegram (or by text).

## 3. What the organizer does

1. Tap the setup link, check the names, tap **Everything looks right. Draw names!**
2. Work through two jobs, one screen at a time:
   - **Send everyone their private link**, one Telegram message each, with a big button per person. People without a phone number use the share sheet instead, and there are Text and Copy backups on every screen.
   - **Save a backup** by sending it to the helper. With about ten people the backup is too long for a Telegram message, so the page sends it by text message instead.
3. Done. If someone loses their message, **Need help?** on the same page covers it. The ticks on the jobs screen show who has been sent a link.

If the organizer taps the setup link again later, it goes straight back to their jobs. It doesn't redo the draw.

If they do need to draw again (under **Need help?**), nobody gets the same person as the draw before, and the "Names are drawn!" screen offers a way back to the old draw until the first new link is sent.

## 4. What everyone else does

Tap the private link the organizer sent you, then tap to see who you got. There is no family link and there are no codes. Opening your own link again any time brings your page back. Telegram's built-in browser can forget things, so keep the message from the organizer.

Wishlists are posted to the group chat as locked links. A wishlist opens only for the person who drew you.

## Good to know

- Phone numbers need the country code, like `+1 555 010 0004`. Without it the organizer's Telegram button may open the wrong chat.
- The private link holds that one pairing in readable form. Send it to that person only, never in the group chat.
- The setup link holds names and phone numbers. The backup link and the results file hold everything: every pairing and every key. Keep those three between the helper and the organizer.
- Whoever hosts the page (GitHub Pages) and any chat app that previews links receives what comes after the `?`.
- Drawing again does not switch off old links, so everyone must use the newest message.
- The organizer can see everything if they choose to look (it's tucked under Need help). Their phone doesn't show it unless they ask.
- The helper who receives the backup can read every pairing too, including their own. Pick a helper who is happy with that, or send the backup to yourself.
- Only open the link that arrives in the organizer's own chat with you. The page trusts the first link it sees for your name; if a second, different one turns up it asks before switching.
- Anyone who picks up an unlocked phone that has opened a personal link can get back to that person's page from the bare address, but they still have to tap to see the name, and the same message sits in that phone's Telegram anyway.
