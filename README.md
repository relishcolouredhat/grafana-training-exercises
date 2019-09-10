# Grafana for all workshop!

  Welcome: NX Week 2019's Grafana workshop!  

  Perhaps you've seen some cool dashboads. Perhaps you have not. I assure you, it
  is easier than it ever has been to create live data visualizations. Lets walk
  through getting started!

---

## Exercise 1: A Grafana for each and every one of us!

  The amount of data in a working Grafana instance can be confusing and
  intimidating.  To make things easier to get started, *In this first exercise,
  we will set up a fresh place to work!*

### Step 0: You're going to need an email address.

  To complete the exercises, you will need a working email address (you can
    also use oauth for most if you like & know what that is). These
  exercises do not require you to use any *specific* email address.

  _If you don't think you'll ever use your personal Grafana after this training,
  feel free to **not** use your real email address._

###### If you do NOT want to use your email address:

  - Sign up for a temporary email address:
    - Go to [temp-mail.org](http://temp-mail.org) or [guerrillamail.com](https://www.guerrillamail.com/)
    - Copy `Your Temporary Email Address`
    - Leave the window open - you'll need to come back here to verify at least once.  


### Step 1. Sign up for Grafana Cloud

  1.1 Go to [grafana.com/get](https://grafana.com/get) & click "Get your *free* instance now"

  ![](https://raw.githubusercontent.com/relishcolouredhat/grafana-training-exercises/master/free-instance-button.PNG)


  1.2a Enter Email  
    - Choose a username & password
    - If you used the disposable email generator & are stuck thinking of a password, use `h3mpr0p3`. It's a *terrible* password, but for the purpose of this training we don't want to waste time with password resets & etc. If you decide to keep your instance, change the password after. (look of dissaproval)
    - Confirm Email

    OR

  1.2b OAuth
    - Login using OAuth.
    - (those buttons that say 'login with Google/github')

    OR

  1.2c Canned Training Users

  If you are stuck - use one of the following users. The password is listed above in 1.1a.

    - trainingtestuser0.grafana.net
    - trainingtestuser1.grafana.net

  1.3 Choose Instance Name

  You probably do NOT want to get contacted about hosted metrics.

  1.4 Done! - Wait for a link to your instance!

  ![](https://raw.githubusercontent.com/relishcolouredhat/grafana-training-exercises/master/grafana-is-starting.PNG)


##### Step 2. Get our bearings

  Okay! We should be looking at the `Home Dashboard` right about now.

  Let's start with the most important part: *where to get help.*

  In the bottom left hand corner of the page, there is a `?` icon. Go this way
  for built-in help & keyboard shortcuts.

  ![](https://raw.githubusercontent.com/relishcolouredhat/grafana-training-exercises/master/grafana-is-starting.PNG)

##### Step 3. Add some plugins.

  You'll need a couple of plugins to complete the next exercise. Lets install them.

  ![](https://raw.githubusercontent.com/relishcolouredhat/grafana-training-exercises/master/explore-grafana-plugins.PNG)

  3.1 Click the `Explore plugin repository` button on the Home Dashboard.

  Wow! Look at all these plugins! Let's talk about two types.

  |                |                                                |
  |--              |--                                              |
  | Panel          | Ways to look at data                           |
  | Data Source    | Types of places where data can be pulled from. |

  Grafana has several `panel` types pre-installed. It also has `datasources`,
  but none that we can set up in less than 5 minutes!

  3.2 Install Plugins for the next few exercises
    - `USGS Water Services`
    - `DarkSky`
    - `Finance`

  You will need to visit the page for each plugin, and press the `install plugin`
  button. The plugins are installed automatically.

  3.3 Configure Datasource instances

  Now that we have added these new types of data sources, we still need to
  *configure* the data set.

  Every data source is a little different. The magic of Grafana is that you can
  bring in all these sources into one place - and essentially all the work has
  been abstracted away.

- From the
---
---

Show around the Instance
- Add datasources (later)
  - darksky api

- Add users (cannot in this free version)
- Explore plugins
  -

1. Navigate to Explore Plugins, add:
  - clock
  - darksky api
  - usgs water
  - finance (quand - if interested)

2. DS Config
  - add usgs water
  - add dasksky weather
    - set long and lat
      - click on spot in google maps


---

##### Step -1:

What did we accomplish in this exercise?
- Setup personal Free Grafana Cloud Instance
- Found where to get help
- Added a plugin to our personal Grafana Cloud
- Configured a datasource in our personal Grafana Cloud

This is the end of Exercise 1. If you have any questions, now may be a good time
to write them down - you may find the answers soon (but feel free to ask!)...

If we were doing this training using an on-premise instance, we would skip
exercise 1.

#### Exercise 2: Hello, Grafana Panels.

---

#### Exercise 3: Water Temperature Chart.
- The simplest of all charts. CSV data.
#### Exercise 4:
#### Exercise 5:
#### Exercise 6: Something Something Annotations
#### Exercise 7: Explore Fantastic Dashboards
#### Exercise 8: Break open somebody's dashboard
- Copy the JSON of a panel from Ex 6
- Copy the JSON of a Dashboard from Ex 6

      3. Add dashboard
        3.1 Query Editor
        - Add Query
        - Find a code
        - plot
        - `Add Query` button
        - `Query Inspector` button - debug
        - `Built in help`
        - Naming a series
        3.2 Visual Options & *bucketing*
          - Turn on staircase,
          - First tsdb conceptm *bucketing* the reprentation of real values with the data we have
            - in this case, we have no options to fill in the blanks (interpolate, to the fancier among us)


        Exercise 1:

        - Plot the temperature of two different streams on one chart
          - Site 1: 05527000 KANKAKEE RIVER Chicago
          - Site 2: 05083500 RED RIVER OF THE NORTH AT OSLO, MN

        Exercise 2:

        - Use another panel type to show current temperature


        -
        ```

        ```
  - ### Track 2:
  __goal: build dashboards using panels in the library

  - Common points:
    - Grafana Panel Library
    - Copy and edit
