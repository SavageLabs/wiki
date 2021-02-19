---
title: FactionsX Setup Guide
description: A collection of setup guides for FactionsX
published: true
date: 2021-02-19T23:12:25.152Z
tags: 
---




# Chat Setup

FactionsX's internal chat listener can handle most of the work for you in the following example:

## EssentialsChat
1. Download EssentialsX & install the EssentialsX & EssentialsChat plugin.
2. Go to the chat format section in `/plugins/EssentialsX/config.yml`.
The default format is provided below.
```yaml
format: '<{DISPLAYNAME}> {MESSAGE}'
```

3. We can add `[FACTION]` into this format to add the chat format.
So we can change it to :
```yaml
format: '[FACTION] <{DISPLAYNAME}> {MESSAGE}'
```

4. Next, lets verify the following config options in `/plugins/FactionsX/config/general-config.json`
```json
"chatHandledByAnotherPlugin": false,
"chatFactionPlaceholder": "[FACTION]",
"chatFactionReplaceString": "[RELATIONAL_COLOR][TAG] [FACTION] ",
"chatNoFactionReplaceString": "",
```

From here a simple `/fx reload` & `/ess reload` should do the trick.
