[get-free-grafana-instance]: https://grafana.com/get
[free-instance-button]: https://raw.githubusercontent.com/relishcolouredhat/grafana-training-exercises/master/free-instance-button.PNG "Or Just click here I suppose 😒- but you'll need to click another one of these buttons!"


# Introduction to Grafana workshop!

  Perhaps you've seen some cool dashboads. Perhaps you have not. I assure you, it
  is easier than it ever has been to create live data visualizations. Lets walk
  through getting started!

  The first exercise has a relatively large amount of step-by-step details

---

## Exercise 001: A Grafana for each and every one of us!

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

#### 1.1 Go to [grafana.com/get]() **and** click "Get your *free* instance now"

  [![foo][free-instance-button]][get-free-grafana-instance]


#### 1.2a Enter Email  
    - Choose a username & password
    - If you used the disposable email generator & are stuck thinking of a
      password, use `h3mpr0p3`. It's a *terrible* password, but for the purpose
      of this training we don't want to waste time with password resets & etc.
      If you decide to keep your instance, change the password after.
      ಠ_ಠ
    - Confirm Email

##### `OR`

#### 1.2b OAuth
    - Login using OAuth.
    - (those buttons that say 'login with Google/github')

#### `OR`

#### 1.2c Canned Training Users

  If you are stuck - use one of the following users. The password is the weak one listed above in 1.2a.

    - trainingtestuser0.grafana.net
    - trainingtestuser1.grafana.net

#### 1.3 Choose Instance Name

  *You probably do NOT want to get contacted about hosted metrics.*

#### 1.4 Done! - Wait for a link to your instance!

  ![](https://raw.githubusercontent.com/relishcolouredhat/grafana-training-exercises/master/grafana-is-starting.PNG)


#### Step 2. Get our bearings

  Okay! We should be looking at the `Home Dashboard` right about now.

  Let's start with the most important part to keep from getting lost-
   *How do I get back to where I am?*

#### 2.1 Going `Home`

  By default, your home dashboard will have some buttons to help you get setup.

  Any dashboard can be your home - but you might want to leave it set as default
  for now.

#### 2.1 Finding help

  In the bottom left hand corner of the page, there is a `?` icon. Go this way
  for built-in help & keyboard shortcuts.

  ![](https://raw.githubusercontent.com/relishcolouredhat/grafana-training-exercises/master/where-to-get-grafana-help.PNG)

  You can also just google the questions - the community is great. However, at
  first, you may have better luck asking somebody in person. It can be hard
  to know what people call the thing you are trying to do, and the amount of
  information out there is huge!



#### Step 3. Add some plugins.

  You'll need a couple of plugins to complete the next exercise. Lets install them.

  ![](https://raw.githubusercontent.com/relishcolouredhat/grafana-training-exercises/master/explore-grafana-plugins.PNG)

##### 3.1 Click the `Explore plugin repository` button on the Home Dashboard.

  Wow! Look at all these plugins! Let's talk about two types.

  | Plugin Type     | What it is used for                             |
  |--               |--                                               |
  | Panel           | Ways to look at data                            |
  | Data Source     | Types of places where data can be pulled from.  |

  Grafana has several `panel` types pre-installed. It also has `datasources`,
  but none that we can set up in less than 5 minutes!

##### 3.2 Install Plugins for the next few exercises
    - `USGS Water Services`
    - `DarkSky`
    - `Finance`

  You will need to visit the page for each plugin, and press the `install plugin`
  button. The plugins are installed automatically.

##### 3.3.1 Configure Datasource instances

  Now that we have added these new types of data sources, we still need to
  *configure* the data set.

  Every data source is a little different. The magic of Grafana is that you can
  bring in all these sources into one place - and essentially all the work has
  been abstracted away.

  - From the 'Home Dashboard', click `Add data source`

  ![](https://raw.githubusercontent.com/relishcolouredhat/grafana-training-exercises/master/add-data-source.PNG)

##### 3.3.2 Add `Grafana TestData DB`

  This is the most basic DS (data source) of all. It's full of sample data,
  like "all zeros", or an option for you to paste in csv (excel-ish) data.

  You can name it whatever you wish. After pressing `Save & Test`, you will
  need to click `Back`

  - Add `Finance`

  `Quandl API Key`?! Nobody signed you up for this!

  Quandl is a service with has a bunch of free (low quality) finance data
  available - they have a paid service as well, but the free is more than
  enough to use as a freely available learning tool.

  We will need an api key to use it though. If you have any interest in this
  data (you walk out of the door with this grafana instance today) please
  sign up for a key.

  If you will be using this key for the one exercise below and do NOT plan on
  using your Grafana in the future, you can skil signing up for this one, and:

  For the purpose of these exercises alone - use the following key:
  <REMOVED>


##### 3.3.3 Add  `DarkSky`

 This one will require signing up for your own API key. It's 100% free for 1000
 calls per day. Do not abuse their API, they may be one of the the last free
 access weather APIs available.

 Go to [darksky.net/dev](http://darksky.net/dev) and press `TRY FOR FREE`.  
 Use the email address from step 0.

 You will also need a latitude and longitude to get data for. This plugin can
 be configured many times, one for each location.

 Perhaps you may want to compare the weather between the London and Montreal
 offices? Perhaps you want to see just how cold Winnipeg is?

 Choose one or more longitude/latitude combinations to use in the next exercise.

###### Tip: 'left click' directly on a google map to get the lat/lon.

##### Exercise 001 Conclusion:

What did we accomplish in this exercise?
- Setup personal Free Grafana Cloud Instance
- Found where to get help
- Added a plugin to our personal Grafana Cloud
- Configured a datasource in our personal Grafana Cloud

This is the end of Exercise 1. If you have any questions, now may be a good time
to write them down - you may find the answers soon (but feel free to ask!)...

If we were doing this training using an on-premise instance, we would skip
exercise 1.

---


#### Exercise 002: Hello, Grafana Dashboards.
- Add dashboard
- Add Panel
  - Introduce Query Editor
  - Introduce Datasource picker
    - Pick `TestData DB` (or whatever you named it!)
  - Select `Scenario` `CSV Metric Values`
  - Wow! CSV Data in a chart!
- Save dashboard with comment
  - Data saved is within the dashboard.

---
#### Exercise 003: Water Temperature Chart.
- USGS Data source with given configuration `01646500`
- Introduce Visualization Tab
- Turn on 'staircase'
- Introduces "bucket" concept
  - Width of 'staircase step' = uncertainty zone
- Turn on 'points'


---
#### Exercise 004: Two Charts, Two Metrics
- Clone chart from Ex 3
- Change to different config
- Change colour of lines
- Set Graph Title & Description
- Introduce concept of 'idosyncracies of data sources'
  - usgs cannot show two data one one panel

---
#### Exercise 005: A Panel to show Current Status.
- Clone Panel Again
- Change to singlestat
- Concept of single value panel
- Concept of value aggregation

---
#### Exercise 006: Weather Graph
Goal
- Sign up for DarkSky API (if not already done)
- Configure Dark Sky data source plugin with a lat/lon
- Create a panel with the temperature at that lat/lon
- Multiple Metric per query:
  - Make a graph with two or more metrics
    - e.g. UVindex and Temperature
- Save as second dashboard for Exercise 7

---
#### Exercise 007: Weather and Sun
- Add `Sun and Moon` data source plugin
- Configure same lat/lon as your weather
- Use the `--Mixed--` datasource to add a second query
---
#### Exercise 008: Convert Graph into table format & Export Data
- Use dashboard from Ex7
- Export CSV
  - This works on other panels, but is usually advised to convert to table to
  better see what columns will be included.

#### Exercise 009: Grafana Annotations
---
#### Exercise 010: Explore Fantastic Dashboards
- https://grafana.com/blog/2019/05/16/worth-a-look-public-grafana-dashboards/


---
#### Exercise 101 : Compare GDP Estimates of 3 Countries
- Finance config for above is `UNAE` `{item}_{country}`
- https://www.quandl.com/data/UNAE-United-Nations-National-Accounts-Estimates/documentation
- For example, `Per capita GDP` of `Canada` is `GDPCDPC_CAN`
- Create a chart comparing the GDP of 3 Countries
---
#### Exercise 102: Managing Dashboards with the dashboard Manager
- Folders
- Tags
- Version Reversion
---
#### Exercise 1xx: Copy a panel via JSON
#### Exercise 1xx: Copy a dashboard via JSON
#### Exercise 1xx: Great Colours from Adobe
#### Exercise 1xx: Introducing InfluxDB Data Sources using grafana playground
#### Exercise 1xx: Introducing Template Variables
#### Exercise 1xx: Embedded Graph Links
---
#### Exercise 2xx: External Datasource Annotations
#### Exercise 2xx: Autofilling Template Variables
#### Exercise 2xx: Filter on field values
#### Exercise 2xx: Convert counter to Rate
#### Exercise 2xx: Break open somebody's dashboard
---
#### Exercise 3xx:
#### Exercise 3xx: Where to find Conference Talks
https://www.grafanacon.org/2019/videos


---
