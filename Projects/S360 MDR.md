---
Description: Autofill analysis templates
Status: Not started
tags:
  - projects
---
Current implementation keeps track of the message and sees if that equals the message found in the message set, restructure to take in valuable data, src, target, device, and if all those equal then note it (maybe add an array property in the object for the dates and devices).

- This may also allow for one passthrough of the alerts rather than requiring the code to check multiple times.