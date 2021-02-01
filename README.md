# README: Turnitin Viewer Team Front-end Coding Exercise

Welcome! We're excited you've decided to talk with us about a position on our
engineering team.

The purpose of this exercise is so we can have a conversation about your
technical background and abilities. We think that asking you to code on a
whiteboard during an interview isn't a great way to have a conversation. And
even if we sit down and pair during an interview it's a higher pressure
situation than it could be.

Instead we ask that you read these instructions and do *at most* a few hours of
work, on your time, to complete the exercise. During the interview we'll talk
about decisions you've made, the resulting application, and how you might
change it given different circumstances.  We don't necessarily expect you to complete
_every_ aspect of the challenge, but wanted to provide enough specification/ideas
that you have direction if you complete the more basic aspects quickly.

Below are two sections:

* *Instructions*: the problem we'd like you to solve along with expectations we
  have about your solution.
* *Logistics*: constraints around the problem, and how we'd like you to
  communicate your solution to us

# Instructions

## Problem

We're launching a new application to help search and store gifs (to improve our team's
communication and morale in Slack, of course!).  We'd like you to create a single-page
application that meets the following requirements:

-  The application uses [React](https://reactjs.org/).  You may use whatever other packages or frameworks you'd like.
-  The application should use the [Giphy api](https://developers.giphy.com/docs/api/) to fetch and display gifs that match a keyword provided by the user.
   We'll provide an api key you can use, or you can create your own key and app.
-  The application should conform to the provided [wireframes](#wireframes).

## Part One (search and display)
-  The user can search for gifs by typing in the input box and interacting with the 'search' button.  The current search term should remain displayed in the input field as the results are displayed.
-  Searches will load and display the first 12 gifs per the wireframes.
-  Interacting with the 'reset' button will remove the current search term and any currently displayed gif results.
-  Conducting a new search by keying a new term and interacting with the 'search' button should clear any existing results before displaying the new ones.
-  Interacting with the 'more results' button will load the next 12 gifs and append them to the current display.
-  If there are no gifs, or are no more gifs, this should be indicated to the user in some way.

## Part Two (save your faves)
-  The user can 'favorite' gifs in the results list that they like by interacting with the 'favorite' button (star icon)
-  'Favoriting' a gif will add it to the 'Favorites' display and remove it from the 'Search Results' display.
-  The 'favorite' gifs are displayed within the 'Favorites' display under the heading of the search term that was active when the gif was returned as part of the result set, in the order in which they were added to the favorites.
-  Clearing or changing the search term in the input does not remove a gif from the favorites display.
-  Clearing the favorites display removes all gifs (and headings) from the favorites display.  Any gifs that were added under the currently active search term are returned to their place in the active search display.
-  Removing a single gif from the favorites display... removes it from the display :).  If it is from the current search result set it re-appears in its previous location in the results list.  If it is not from the currently active search, it just vanishes.

## Documentation

-  Please update this readme with any other instructions about stuff we might want to look at: minmally how to run the app, and if applicable how to run tests, how to produce a production bundle, etc.
-  Please preserve your commit history in the posted repo!  We'll likely take a look through how the app was produced in addition to where it ended up.

## Wireframes

1.  [On Load](wireframes/GiphySearch_Mock1_OnLoad.png)
2.  [Search Results](wireframes/GiphySearch_Mock2_SearchResults.png)
3.  [No Results](wireframes/GiphySearch_Mock3_NoResults.png)
4.  [Favorite](wireframes/GiphySearch_Mock4_Favorite.png)
5.  [Reset](wireframes/GiphySearch_Mock5_Reset.png)
6.  [New Search](wireframes/GiphySearch_Mock6_NewSearch.png)
7.  [Mobile / Small Screen](wireframes/GiphySearch_Mock7_Mobile.png)

# Logistics

__1.__ Timeframe

You should take a max of around three hours to complete this exercise. We want to be
both respectful of your time and fair to other candidates who might not have
a whole weekend to work on it.  If you don't get all the way through all of
the things, no worries.

__2.__ Git

You will need to use git for this exercise. To get these instructions and a
repo with test scripts do the following:

1. [Create a Github account](https://github.com/join) if you don't already have
   one. For the examples below we assume a user `myusername`.
2. Clone our repository:

```
# Using ssh
$ git clone git@github.com:turnitin/viewer-coding-exercise.git

# Using https
$ git clone https://myusername@github.com/turnitin/viewer-coding-exercise.git
```

__3.__ Remote

Once you are done you can put your solution in your own repository by adding it
as a remote and pushing to it.

1. Create a new repo via the github UI, let's assume you call it
   `viewer-coding-exercise` to mirror ours.
2. If possible use a private repo (we'd just like to make sure that every candidate's work is
   his or her own).
3. Add your repo as a remote and push:

```
$ git remote add my-github-remote git@github.com:myusername/viewer-coding-exercise.git
$ git push my-github-remote master
```

__4.__ Access

Give Github user `marktfrey` read access to your repository.

__5.__ Notify us

At least a day before your in-person interview, email `mfrey@turnitin.com`
your repo address.

__6.__ Questions, Feedback, etc.

Feel free to contact any of us if you have questions or feedback about this challenge:
-  Mark Frey (`mfrey@turnitin.com`)
-  Ron de las Alas (`rdelasalas@turnitin.com`)
-  Nelson Wong (`nwong@turnitin.com`)


