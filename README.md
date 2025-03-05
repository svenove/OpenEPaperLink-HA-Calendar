# OpenEPaperLink-HA-Calendar
On the [OpenEPaperLink discord](https://discord.gg/fekcBc5RN5), the user "hexifox" made a YAML for a calendar integration for the 7.4" tags. Based on that, "Corwin" adjusted the design to fit 4.2" tags.
The design was working almost flawlessly, but I made some improvements to the 4.2" YAML. Like making sure to only show days/events that would fit the tag (e.g if there are many events, reduce number of days instead of "overflowinf" below the edge). Also made the days easy to translate, fixed some issues with empty days, etc.

Since this YAML only was available on the discord, it was hard to find it for new users. So I desided to just put it up on Github for simplicity.

## Integrations needed:
* https://github.com/jonasniesner/open_epaper_link_homeassistant (Install via HACS)
* A calendar (I use [Google calendar](https://www.home-assistant.io/integrations/google/))

## Initial setup
1. Configure the OEPL-integration and your preferred calendar-integration.
2. Create a new automation from the 4.2_automation.yaml
3. Update the automation to use your preferred language and the calendar entity
