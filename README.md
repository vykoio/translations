# Vyko Translations

Help translate our platform into your own language.

**It is highly advised you do not attempt to translate into a language which you are not relatively fluent in**

## Why translate?

Whilst you may be lucky enough to understand English to a certain degree, others may not. Sure, tools like Google Translate exist but the accuracy is limited. Therefore we've decided the best way to move forward is via human interpretation. So, if you're close to being a native speaker in a given language, we'd like to invite you to help those people who are not as proficient in understanding English as you. As thanks, all contributors will receive a mention in the site credits (along with their relevant submitted links) as well as a "Translator" badge on their public profile and of course for those translators with shopfronts, your assistance will allow for a higher usability and satisfaction amongst your visitors as those visiting from more "international" regions will be able to understand the given text.

## Full Guide

1. You will first need to obtain the [two letter language code](https://en.wikipedia.org/wiki/List_of_ISO_639-1_codes) of the language you wish to translate.

2. Then, for you to be able to begin editing, you will need to [Fork this Repository](https://github.com/vykoio/translations/fork).

3. Select the file(s) or location(s) where you wish to perform your translations ([see `What file am I looking for?`](#what-file-am-i-looking-for)).

   - **If a file/directory with your two letter language code does not exist**, you'll need to create it. Put it in the correct location (see others for an example) and name it with either the two letter language code - `xx.vyko` (replacing xx with code) or the valid page name (again, see what others have done for a reference). Then, copy the contents of `new.vyko` or, if you created a directory, the `new/` folder into your newly created file(s) for guidance (if required).

4. You may now begin translating from English into your language of choice. Removing the `//` infront of whatever you decide to translate so our system knows a translation is available for the said "key" in your language. E.g `//account.creation.activation = "Success"` would become `account.creation.activation = "Success"`

   - If you are unsure of what a certain "key" means, [open an issue here](https://github.com/vykoio/translations/issues) or email us - [translations@vyko.io](mailto:translations@byko.io)

5. When you've finished translating some or all of the "keys", [create a pull request](https://guides.github.com/activities/forking/#making-a-pull-request) so we can implement it into our official Repository and have it reflected across our platform. Within a pull request, please leave the information required for us to add you to the sites credit (Your Name/Alias and [optionally] your website/social platform) and/or your Vyko username so we can add your rewards to your account.

## What file am I looking for?

If you're looking to translate messages for the API (messages the user receives after performing a task - e.g registration) - see the `api/` directory. Each language has it's own file.

If you're looking to translate messages for the site's pages, see the `front/` directory. Each language has it's own directory and within that are files for each page (e.g `landing.vyko` for the landing/home page).

If you're looking to translate messages for the Emails sent to user's, see the `mail/` directory. Each language has it's own file.

## Formatting

If you'd like to add another line e.g

```
line1
line2
```

It can be achieved like: `multiline = "line1\nline2` where `\n` represents the new line. **Do not literally press enter for a new line.** Keep it all in one.

This is handy in email templates.

## Variables

Variables can also be used in email templates. Paste them in exactly as they are.

`{{username}}`: The user this email is for

`{{fromUser}}`: The user that caused such an email to send (invitation e.t.c)

`{{project}}`: The name of the storefront that caused such an email to send (invitation e.t.c).

`{{link}}`: The link associated with the action of the email (e.g activation link) **Only to be used in plaintext (non HTML) emails**

`{{privacy_link}}`: The link to the privacy policy page
