---
title: Restart an App
objective: 
layout: docs
nav: firecracker
order: 70
---

Running `fly deploy` on an App creates a new release of the App, and restarts the Machines that it manages.

Sometimes you don't want to update anything; you just want to reboot and start the root file system afresh. (Yes, restarting wipes the ephemeral file system, just as a `fly deploy` or `fly machine update` will.)

## Restart every Machine in the App

`fly apps restart <app-name>` restarts all Machines in the App&mdash; Machines that belong to `fly deploy` as well as any other Machines you may have created within the App.

## Restart an Individual Machine

If one particular Machine needs a kick, restart it using `fly m restart <machine-id>`.