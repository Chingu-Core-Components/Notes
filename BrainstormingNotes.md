run python script in node using python-shell package

    python script needs
        import sys, json

    python output format: panda dataframe
        desired output: JSON

    node output format: JSON
        write a script to send the data into python on an interval


scoring

[ add other tags here ]k
[H] - heavy weighting

    GitHub Tracking - HEAVIEST WEIGHT

        look into the GitHub API and see what is available to see
        ideally:
            every new team repo sets up "milestone" issues
            whenever a milestone is met have the team send a commit that tags that issue #
            when that commit is merged then trigger a milestone complete action in the autobot
        help keep track of teams and their progress via actual code

        Data collection
            number of commits
            commits / user
            issues solved / milestones reached

        https://developer.github.com/v3/issues/milestones/
            all teams register a repo in the voyage team
            bot runs through and adds milestones according to tier
            bot monitors milestones on an interval
            bot reacts accordingly

    Chingu profile data

        certifications
            weigh each option

        [H] number of projects completed

        cohorts
            weigh by tier

        number of check-ins
            checkin streaks
            check-in to mentor sessions

        [H] helpfulness score in the community
                how is this defined?
                complaints? (tickets)


    slack data (AutoBot moderation)
        How to Gather:
        https://api.slack.com/events/message
            Real Time Data
                continuous counters
                    gather history and compare daily / interval deltas
                data visualization of Chingu RTD
                    an activity map of Chingu / specific cohorts


        number of *reactions* / message
            https://api.slack.com/events/reaction_added
            store the item
                update reactions counter per item
                // action if threshold reactions is met

        specific channels activity:
            activity counters:
                messages sent
                files shared

            help channel
            resource sharing
            community
            project managers

        team activity frequency

    after chingu data
        # applications / callbacks / offers
        job earned
        etc
        correlate score to professional data 


    BOTH TOGETHER
        how to score a user overall
            for pairings
            for cohort selection

        how to score a user based on activity


Project Milestones

    autobot would checkin in at set intervals and request deliverables
        conversation style requests / responses
            score based on deliverables met
                actions on deliverables failed

Automatic tasks

    near the end of cohorts take all the top users and message them
    about being a mentor

    New / returning users to Chingu Cohort
        Sorting Hat will provide the teams / team members
        AutoBot will then create a channel and insert the team members

    Monitoring channels
        user activity is low [team / other channel]
            message them to engage
                if no response then second message
                    decide whether to move / remove then
                        (generate a ticket and / or message chance with user name)
                            give details in the ticket/message about the user
                                data
                                previous contact attempts
                                    replies

                            chance makes final decision
                                bot moves / removes
            NEEDS:
                RTM data [counters]
                user score


Dashboard [admin]
    Front end and/or on the Slack app page
    display visual statistics
        global (all cohorts)
        per cohort
        per channel
        per team
        per user
    moderator methods
        add / move / remove users
        handle tickets
        view / export[formatted] most reacted message quotes for "heard around chingu"


Free Agents
    checks the user's current score / tier / project / strength/ dependability score
        pair them with other teams that have a need they can fulfill

Chingu Points
    check-ins
    github commits (scaled based on size of commit)
    projects completed
    giving help in the help channel
    giving help on the forum


GitHub SETUP
    separate by tiers (more structure to less structure)
    set up projects / cards with milestones
    premade file structure with folders than the bot can check for content / length of content

3 ACTS of milestones
    project setup
        1) everyone has communicated in the chat [AutoBot slack listen]
        2) schedule the first meeting [slack listen]
        3) first meeting [file - upload to gitHub]
            discuss the assigned project
            discuss the stack

    coding
    closure / showcase
        an article
        screencasts
        showcase on slack / website


Elon Musk image for bot 

