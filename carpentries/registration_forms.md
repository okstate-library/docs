### Setting Up Registration Forms

Registration forms should be set up at the beginning of each semester once dates have been determined. The person setting up the registration forms will give the registration links to the individual charged with setting up workshop websites.

#### Outputs
This process produces registration forms for each workshop in a given semester.

#### Inputs
The individual needs access to LibCal in LibApps.

#### Roles
- Individual charged with creating registration forms in LibCal.
- Individual charged with creating workshop websites.

#### Activities
1. Open LibCal and click *Calendars*.
1. Click *Library Workshops*.
1. Click *Library Events*.
1. Select *Create From Scratch*.
1. Click *Continue*
1. Select the *Date*, *Start Time*, and *End Time*. Don't add padding.
1. All workshops span multiple days. Check *This Event Repeats* and fill in the appropriate information based on the workshops format (some workshops are two days back to back, and some workshops are half-day workshops across four Fridays).
1. Title the workshop (e.g., Data Carpentry Workshop or Software Carpentry Workshop)
1. Use the following event description for **Data Carpentry** workshops: [Data Carpentry](https://datacarpentry.org/) develops and teaches workshops on the fundamental data skills needed to conduct research. Its target audience is researchers who have little to no prior computational experience, and its lessons are domain specific, building on learners' existing knowledge to enable them to quickly apply skills learned to their own research. Participants will be encouraged to help one another and to apply what they have learned to their own research problems. *This workshop will include an introduction to R.*
1. Use the following event description for **Software Carpentry** workshops: [Software Carpentry](https://software-carpentry.org/) aims to help researchers get their work done in less time and with less pain by teaching them basic research computing skills. This hands-on workshop will cover basic concepts and tools, including program design, version control, data management, and task automation. Participants will be encouraged to help one another and to apply what they have learned to their own research problems. *This workshop includes an introduction to Python.*
1. Use the [JPEG version of the logo](https://okstate-library.github.io/docs/carpentries/TheCarpentries.jpg) from the [Carpentries Organization](https://carpentries.org/) for the *Featured Image*. **The workshop must be registered with the Carpentries Organization to use this logo. Otherwise, we cannot use the logo and must use phrasing along the lines of a "Carpentries inspired workshop" the workshop webpages.**
1. Select *Carpentries @ Oklahoma State University by Kay Bjornen* as the *Related LibGuide*.
1. In *Friendly URL*, put YYYY-MM-DD-okstate; YYYY-MM-DD indicates the date of the first day of the workshop in the indicated format.
1. Select the location (most workshops will be in *Computer Training Room 206, 2nd Floor, Edmon Low Library*.
1. Select the *Event Organizer*.
1. Type `30` for the *Anticipated Attendance*.
1. Select `Public Program` and `Instruction` in *Category*.
1. Ensure *Registration is required* is checked.
1. Input *Maximum registrations/seats*. The maximum registration we allow for room 206 is 30.
1. Select *Carpentries* as the *Registration Form*.
1. Set *Registrations Open* to *4 weeks before*.
1. Set *Registrations Close* to *24 hours before*.
1. Check *Enable a waiting list when fully booked*.
1. Check *Seris link registration* (this creates one registration form when a workshop spans multiple days).
1. Check *Enable registration until the last event in series*.
1. Set *Send Email Reminder* to *4 days before Event* (see below for text to paste into *Reminder Email Body*.
1. Set *Send Follow-up Email/Survey* to *1 day after Event* (see below for text to paste into *Follow-up Email Body*.
1. Set *Status* to *Submit for Review*.
1. Click *Submit: Add New Event!*
1. Click on the event in the *Library Events* calendar.
1. Copy *Event URL:* and send it to the person setting up the workshop website so they can add a registration link.
1. You can click the blue *Manage Event* button to manage attendees and the waitlist.

##### Reminder Email Body
Paste this exact text into the *Reminder Email Body* field. **Only change the series of X's, i.e. XXXXXXXXXX, with the relevant URLs from the workshop webpage***.
```
Hi {{FIRST_NAME}}, 
			
This is a reminder that {{TITLE}} starts at {{START_TIME}}, {{DATE}} at {{LOCATION}}.

Workshop webpage: XXXXXXXXXXXXXXX

Please make sure to install the necessary software before attending the workshop: XXXXXXXXXXXXXXX#setup. Instructors will be available starting at 8:30 a.m. to answer installation questions.

Before coming to the workshop, please complete the pre-workshop survey: XXXXXXXXXXXXXXXXXXXX.

To cancel this registration visit: {{{CANCEL_URL}}}.{{#REGISTRATION_COST}}
```

##### Follow-up Email Body
Paste this exact text into the *Follow-up Email Body* field. **Only change the series of X's, i.e. XXXXXXXXXX, with the relevant URLs from the workshop webpage***.
```
Hi {{FIRST_NAME}}, 
			
Thank you for attending {{TITLE}}. 

If you have not done so already, please complete the Post-Workshop survey: XXXXXXXXXXXXXXXXXXXXXXXXXXXXX.

If you have any further questions about this event, please contact {{OWNER_NAME}} via {{{OWNER_EMAIL}}}.
```


