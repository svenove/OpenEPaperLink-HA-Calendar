# OpenEPaperLink-HA-Calendar
On the [OpenEPaperLink discord](https://discord.gg/fekcBc5RN5), the user "hexifox" made a YAML for a calendar integration for the 7.4" tags. Based on that, "Corwin" adjusted the design to fit 4.2" tags.
The design was working almost flawlessly, but I made some improvements to the 4.2" YAML. Like making sure to only show days/events that would fit the tag (e.g if there are many events, reduce number of days instead of "overflowing" below the edge). 
Also made the days easy to translate, fixed some issues with empty days, etc.

Since this YAML only was available on the discord, it was hard to find it for new users. So I desided to just put it up on Github for simplicity.

## Integrations needed:
* https://github.com/jonasniesner/open_epaper_link_homeassistant (Install via HACS)
* A calendar (I use [Google calendar](https://www.home-assistant.io/integrations/google/))

## Initial setup
1. Configure the OEPL-integration and your preferred calendar-integration.
2. Create a new automation from the 4.2_automation.yaml
3. Install GothamRnd-Bold.ttf to the "media"-folder (or remove all the "fonts:"-lines from the automation to use the default font - but that might mess up the spacing-calculations)
4. Update the automation to use your preferred language and the calendar entity:
- Replace all 4 instances of "calendar.our_house" with your calendar
- Translate day-names and month-names into your preferred language
- Adjust the display format of days and time by changing all the "timestamp_custom"-entries in the automation to fit your needs.
- Select your tag-device
