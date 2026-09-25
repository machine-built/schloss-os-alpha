# SchlossOS

Hello world!

I'm not a developer, and I'm still new to git and GitHub, so please bear with the formatting here. I'm a former Windows sysadmin/IT person who has spent the last few years learning Linux under the hood. This project is me trying to take my old Windows image-building and fleet-deployment skills and apply them to Linux, while learning the core concepts where Linux really differs from Windows or macOS.

**tl;dr** this is rough in places, and that's exactly why I'm sharing it. I want to do this right, so if you know more than me, please take a look and tell me what I'm missing. This is an alpha release. Things will break.

## What is SchlossOS?

Schloss is a workspace "solution" I'm building, centered on an atomic Linux image currently called SchlossOS. It's built on AlmaLinux 10 KDE. I picked that foundation because I'm betting that following IBM's direction for enterprise Linux will pay off long term, but true FOSS is still the way, so big thanks to the AlmaLinux Atomic SIG for making this possible.

The obvious goal is to simulate an opinionated Windows-like experience, with the long-term intent of replacing Windows on enterprise PCs. Planned pieces include, an identity layer, Element connected to a hosted Matrix server (still work in progress as of this update), Office and collaboration apps (Collabora in the browser, EuroOffice as it matures), Cloud drive storage synced locally, and other "enterprise productivity" apps

## Current State (v0.0.5)

A few things you should know before trying this:

- I run a Beszel server for device monitoring, and every image ships with a monitoring agent.
- If you set a device name during setup, a script will quietly change it afterward.
- Your device and a partial serial number get reported to my server and dashboard.
- I can only see things like disk, memory, and network state (when the device is awake and connected). I cannot see your account name or any other personal info.
- If that's a dealbreaker for you, feel free to skip this distro for now :)

Everything else is pretty vanilla. This image probably won't work well on the latest-gen machines, especially anything with a dedicated NVIDIA GPU. The target hardware is Lenovo AMD Ryzen or equivalent Dell/HP machines. Stray too far outside that hardware matrix and things will likely break, but I'd love to hear about the result if you try!
</content>
