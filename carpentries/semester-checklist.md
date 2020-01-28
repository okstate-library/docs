# Semester Checklist
One month before the end of each semester, the following logistics need to be in place. It is ideal if volunteer coordination is in place, but that depends on the response of volunteers. Try to have items in the Coordinating Volunteers and Participants section completed as soon as is practically possible.

# Logistics
- [ ] Set workshop dates.
  - We currently offer workshops just before and after a semester. We also offer a workshop during the mid-semester (Fall/Spring) break.
- [ ] Book room for selected dates.
  - Use [Room Bookings](https://okstate.libcal.com/booking/conference-rooms) to book room 206. for the selected dates (max capacity is 42).
  - Workshops typically run from 8:30 a.m.–4:00 p.m. Be sure to pad start and end times when you book.
- [ ] Set up workshop webpages for each workshop.
  - You will need to clone the [Carpentries Workshop Template](https://github.com/carpentries/workshop-template) into [OSU Carpentries](https://github.com/OSU-Carpentry) organizational account on GitHub. Be sure to follow the [directions](https://github.com/carpentries/workshop-template/blob/gh-pages/README.md) they have provided carefully. **Carpentries frequently updates the Workshop Template and instructions. It is important to re-clone a fresh copy of this repo each time this process is done. Don't be tempted to clone one of our previous workshops to avoid entering workshop details.** This often leads to errors and causes software installation instructions to fall out of date.
  - OSU Carpentries uses a script to automatically populate the [OSU Carpentries landing page](https://osu-carpentry.github.io/) with a list of current and past workshops. The script will only include repos that meet certain conditions (see https://github.com/OSU-Carpentry/2019-11-01-okstate as a working example of the next two points):
    - The repo title must follow the format `YYYY-MM-DD-okstate`.
    - Both the "Description" and "Website" fields at the top of the repo must be populated. Click the "Edit" button at the top, righthand corner—just under "Settings"—to edit these fields. Paste the URL for the live workshop website into "Website." In "Description," label the workshop appropriately: "Software Carpentry Workshop" or "Data Carpentry Workshop." The script uses all three pieces of information to create an entry for each workshop on the landing page.
  - Do not fill in the "Description" and "Website" fields until you are ready for the site to be linked live from the landing page.
- [ ] Set up [registration forms](https://info.library.okstate.edu/c.php?g=970224) for each workshop.
- [ ] Use the URL from the registration form to create a registration button on each workshop webpage.
  - Our registration button is a custom item. Use the code in the appendix below.
  - Paste the code into `index.md` for the workshop website. Paste it after the Eventbrite widget code and before the General Information heading.
  - Make sure to put the registration page URL in the `href` field where it says `REGISTRATION URL GOES BETWEEN THESE QUOTES`.
- [ ] Set up the [workshop Etherpad](https://tiger.hpc.okstate.edu/sites/etherpad/).
  - Name the Etherpad using the `YYYY-MM-DD-okstate` convention.
  - Copy the URL from the newly created Etherpad and paste it after `collaborative_notes:` in the preamble at the top of `index.md`.
- [ ] Fill out the workshop request form to let the Carpentries organization know about the workshop.
  - Since we are a member organization, we self-host workshops. The registration form for self-hosted workshops is [here](https://amy.carpentries.org/forms/self-organised/).
- [ ] Don't forget to update the description at the top of the repo for the landing-page script to work.
- [ ] Set reminders in the Carpentries Outlook calendar for [pre-workshop meetings](https://info.library.okstate.edu/c.php?g=970224), [post-workshop meetings](https://info.library.okstate.edu/c.php?g=970224), [monthly meetings](https://info.library.okstate.edu/c.php?g=970224) (once responses are in from the poll), workshops, and meeting to go through this process again at the end of the semester.


# Coordinating Volunteers and Participants
- [ ] Get commitments from certified instructors for teaching roles.
  - Try to get commitments before the beginning of the semester. Make sure to remind volunteers at monthly meetings if there are unfilled teaching opportunities once the semester begins.
- [ ] Get commitments from helpers for workshops.
  - Try to get commitments before the beginning of the semester. Make sure to remind volunteers at monthly meetings if there are unfilled teaching opportunities once the semester begins.
- [ ] Once the workshop webpages are linked from the [OSU landing page](https://osu-carpentry.github.io/), contact anyone who was on a waitlist in the current semester and notify them of the dates for next semester.
- [ ] Advertise the workshops
  - Give Communications the dates for next semester's workshops and set mailings to go out one month before the workshop.
  - Contact [Kate Adams](mailto:kate@greatplains.net) to let her know next semester's workshop dates.
  - Submit all the workshops to the [OSU Calendar](https://calendar.okstate.edu/) by clicking on "Submit Event." You will need to submit for each individual workshop.
  - Contact [Jennifer Borland](mailto:jennifer.borland@okstate.edu) who runs the Digital Humanities mailing list and let her know the dates of upcoming workshops.

# Appendix
## Button Code
Use this code for the registration button on workshop webpages.

```html
<p><a id="s_lc_event_5584425" href="REGISTRATION URL GOES BETWEEN THESE QUOTES">CLICK TO REGISTER</a>
<!-- Below is optional element styling  //--></p>
<style>
#s_lc_event_5584425 {
  background: #FF6600;
  border: 1px solid #DFDFDF;
  border-radius: 4px;
  color: white;
  font: 18px Arial, Helvetica, Verdana;
  padding: 8px 20px;
  cursor: pointer;
}
#s_lc_event_5584425:hover {
  opacity: 0.9;
}
</style>
```
