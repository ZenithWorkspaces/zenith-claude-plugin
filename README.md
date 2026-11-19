# Zenith Workspaces plugin for Claude

Zenith Workspaces is a coworking space at 106 Apple Street, Suite 200W, Tinton Falls, NJ 07724. This plugin connects Claude to our MCP server so it can show our rooms, check whether one is free on a given date, give you a booking link with the date and length filled in, and answer common questions about the space.

## What is included

- An MCP connection to `https://zenith-mcp.zenithworkspaces.workers.dev/mcp`. It needs no sign-in.
- Skill `zenith-rooms`: finds a free private office or the conference room and returns a booking link.
- Skill `zenith-info`: answers questions about hours, parking, pricing, memberships, mail service, and amenities.

## Tools on the server

All four tools only read data. None of them book, hold, or charge for anything. You finish booking and payment on our booking page.

- `list_spaces`: the six private offices and the Evergreen Conference Room, with size, price, and photos.
- `check_availability`: free and busy times for a room on a date, from our live booking calendar.
- `get_booking_link`: the booking page for a room, with date and length filled in and a price estimate.
- `get_info`: address, hours, parking, day passes, memberships, mail service, and amenities.

## Example prompts

- Is a private office free at Zenith Workspaces next Tuesday from 9 to 1?
- What does the Evergreen Conference Room at Zenith cost for a full day, and is it open this Friday?
- I need a business address in Monmouth County. What does Zenith Workspaces offer?

## Data and privacy

The plugin sends the room, date, time, and topic you ask about to our server and nothing else. It does not read your files or conversation history. Privacy policy: https://www.zenithworkspaces.com/mcp-privacy. Terms: https://www.zenithworkspaces.com/terms.

## Support

info@zenithworkspaces.com or 848-331-8382. Docs: https://www.zenithworkspaces.com/ai-assistants
