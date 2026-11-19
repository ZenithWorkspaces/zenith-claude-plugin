---
name: zenith-rooms
description: Use when someone wants a private office or the conference room at Zenith Workspaces in Tinton Falls, NJ, asks which rooms are free on a date, or wants to book one.
---

# Find and book a room at Zenith Workspaces

Zenith has six private offices (Everest, K2, Denali, Summit, Atlas, Matterhorn) and one conference room, the Evergreen Conference Room, which seats 10. All rooms can be booked any time, day or night.

## Steps

1. If the person has not named a room, call `list_spaces` and show the rooms with size and price. Offices cost the same, so for a single person any office works.
2. When they give a date, call `check_availability`. Pass the room name, or `any_office` if any private office will do. Use the date as YYYY-MM-DD in US Eastern time. If they gave a start time and length, pass `start` (24-hour HH:MM) and `duration_hours` to test that exact slot.
3. Tell them plainly whether the slot is free. If it is not, offer the nearest free window from the result.
4. Call `get_booking_link` with the room, date, and duration, and give them the link with the price estimate.

## Rules

- These tools only read. Nothing is held or booked until the person finishes on the booking page, and a free slot can be taken before then. Say so when you share the link.
- Prices from the tools exclude NJ sales tax. Say that when you quote a price.
- Monthly private offices and executive suites are quote only. For those, send the person to info@zenithworkspaces.com or 848-331-8382 instead of a booking link.
- If a room shows no open times on any date, it is likely on a long-term assignment. Suggest another office.
