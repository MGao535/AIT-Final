# My Weeb List

# Overview

When you're a high key weeb with a bit too many animes in your watchlist (and possibly some you'd like to keep private), most commonplace websites just aren't sophisticated enough to deal with filering shows of a certain genre in your watchlist for custom recoomendation lists and even creating a private list unless you want to create a different account.   

My Weeb List is a web app that will allow users to keep track of their watchlist while also being able to sort the list according to genre and privacy. Users can register and login. Once they're logged in, they can either add a new anime or view their list. For the list, they will have the option to filter the list.

# Data Model

The application will store Users, a List and Items

Users will only have one list (via references).
Each list will have multiple items (by embedding).

An Example User:

{
  username: "xXW33B420Xx",
  hash: // a password hash,
  lists: // a reference to List documents
}

An Example List with Embedded Items: 

{
  user: // a reference to a User object
  name: user.name + "'s Weeb List",
  items: [
    { name: "Pokemon", rating: "8", genres: "Action, Adventure, Comedy, Kids, Fantasy", show: true},
    { name: "Mobile Suit Gundam 00", rating: "9", genres: "Action, Military, Sci-Fi, Space, Drama, Mecha", show: true},
  ],
  lastUpdated: // timestamp
}

# Link to Commented First Draft Schema

# Wireframes

/weeb/options

[![Alt text](/path/to/img.jpg?raw=true)][https://drive.google.com/file/d/1aPiPTTUtzlVLySl-ArD34NLXI01yTB0C/view?usp=sharing]

/weeb/add

[![Alt text](/path/to/img.jpg?raw=true)][https://drive.google.com/file/d/1ob2J8ielxbYqhpVJgXBMZvs-1KwYym_C/view?usp=sharing]

/weeb/list

[![Alt text](/path/to/img.jpg?raw=true)][https://drive.google.com/file/d/1YLkKDBRa9FyExKFqGO5tv-NMP2oVFMCT/view?usp=sharing]

# Site Map

# User Stories or Use Cases

1. As a non-registered user, I can register a new account with the site
2. As a user, I can log in to the site
3. As a user, I can add a new anime to my watchlist
4. As a user, I can view my watchlist
5. As a user, I can filter my watchlist to not show private entries
6. As a user, I can filter my watchlist by genre

# Research Topics
