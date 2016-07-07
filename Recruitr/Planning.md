# Recruitr

//TODO lookup authentication with firebase and sails.

Users
  - roles
    - admin
    - members
      - role?
    - potentials
          - background info
          - year gpa hometown
          - interest level?
  - all attributes
    - photo
    - phone number
    - possible social media links (fb, twitter etc)
    - major

Voting
  - stars or yes no?
  - like dislike
  - traits - (fraternal values)

Metrics /stats
  - votes
  - percentages
  - interest levels
  -

Nameslist
  - rankings
  - 
  
Richard's Notes: 

Architecture:
- Database and profiles on website
- Pushed out to phones for “tinder-like” swiping and rating
- Returned to web app for analytics

List of things to be worked on:
- Splash screen
- Goes into log in screen, with login options, and create new accounts
    - Create new account goes to user registration
    - User registration should consist of Rushee, and Member statuses
    - Login screen should have pin access?
- Login goes home page
- Home page brings you into your greek organizations homepage as set by the administrator
    - Should the home page for the administrator look different?
    - Should there be an administrator mode, or should you only be able to administer from the web client?
- As a Rushee user, you should have an ability to join a university, access to the names of the greek organizations, and their resulting rush chairs. 
    - You should have access to your profile, on which you could post pictures and stuff, similar to a linked in account
    - Maybe have a ranking system for organizations that you like?
- As a Member user you should have access to new recruit rating, past rating, and overall statistics about your greek organization
- As an admin user, you should have access to individual Member user statistics, organization statistics, and the abilities to add users to Member users recruit ratings
    - You should have a recruit pool, where you can add rushees by linking their accounts, or by creating new accounts for them.
        - If the the new user registration system senses that an organization admin has registered the same name and email, offer to use that already set up profile maybe?


Rating Tiers:
- First tier is swiping
    - Allow members to swipe left or right through the rushers
    - This will be used to generate a general like/dislike on each rushee

- Second tier is rating
    - Allow members to rate rushees with a star system for individual characteristics
    - Characteristics could be: Socialness, Coolness, Style
    - This will be used to analyze specific places where rushees succeed and fail
    - 
- Third Tier is Bid/No Bid
    - Allow members to finalize thoughts and see where they rank each of the rushees
    - Maybe you should only have access to this when every rushee has been ranked?

Statistics Idea:
- Have an average rating 

Development ideas

Branding:

- Changeable color schemes based on fraternity colors
    - Check out UIAppearance?

Marketing:

Software:
- Figure out how to make the save/modify button active when changing data about an entry.
    - As it stands currently, the save button is disabled when the keyboard is open.
    - Find the textFieldDidBeginEditing method to toggle this in the MealViewController

- Edit button implementation
    - In MealTableViewController, what is the point of (self.) before the navigationItem addition?
    - They both perform the same, but I’m wondering what behavior each has?
    - ANSWER: self refers to the particular instance. In general, self doesn’t really need to be used, unless the is an instance property with the same name as a method parameter

- Something to consider when building the app
    - Implement events!
    - Instead of using a class to do everything, make the class do it’s core functionality, and raise events to tell whoever is listening to take a separate action

- Unit Tests
    - Trust, but Verify
    - For instance, when using NSButton to have a message (action) sent to a particular object (target), you can trust that the action will be sent to the target.
    - HOWEVER, you should write a unit test to ensure that both the target and action were properly specified.
    - Trust, but verify

- We should start to design the actual app itself. The splash screen, the starting page, the different branches.

- How can we prove that registering users are themselves? What if someone registers a fake fraternity, or aren’t in the fraternity that they register for?
- 



