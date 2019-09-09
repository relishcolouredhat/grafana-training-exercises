
- #### Grafana Training

foo.


  - ### Track 1: Metrics for all. Build a weather dashboard in half an hour!
  __goal: increase general comfort with the software in an approachable way__
    - Sign up for grafana cloud
      - GitHub
      - Google
      - Any Email
      - temp-mail.org/en

      0. Get email
        - temp-mail.org/en or temp-mail.org/fr
        - copy address
      1. grafana.com/get - "We Host it" Get your *free* instance now  
        1.1 Enter Email  
          - Pick username & password
          - If you used the disposable email generator & can't think of a password, use h3mpr0p3. It's a terrible password, but for the purpose of this training we don't want to waste time with password resets & etc. If you decide to keep your instance, change the password after. (look of dissaproval)
          - Confirm Email
        1.2 OAuth
        1.3 Canned Training Users
          - trainingtestuser0.grafana.net
          - trainingtestuser1.grafana.net
      2. Choose Instance Name
          - Do not get contacted about hosted metrics.
      3. Done! - Follow link to instance!

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
