# PwrNote
Welcome to the [powernote](https://pwrnote.herokuapp.com/) wiki!

## Features

 1. User Authentication with persisting sessions
 2. Notes and Notebooks with rich text editing
   * Users will be able to Create, Edit and Delete their notes.
   * Notes will have rich text editing including charts and graphs
   * Notes will autosave
   * Users will be able to choose which notebooks to make public
 3. Tags
   * users will be able to create edit and delete tags
   * users and non-users can view tags and associated public notebooks
 4. Likes
   * Users will be able to create and delete Likes on public notebooks
 5. Search
   * Users will be able to search through notebooks and tags
   
## Store Shape 

``` js
store = {
    session: {},
    notebooks: {
        // note that evernote allows you to create notes without manually putting it in a notebook. Setup a default notebook for this. 
        notebookId: {
            ...notebookData,
            notes: {...normalizedNotes}
        },
        optionalOrderedList: []
    }
}
```

## [DB Diagram](https://dbdiagram.io/d/62aab2f79921fe2a96184f38)
![image](https://user-images.githubusercontent.com/63429309/175616996-27c05572-c2b7-4d69-b837-feef278f07f5.png)


[Scorecard](https://docs.google.com/spreadsheets/d/1ufo9p-QuN9B744p3FhCchIJ1g-N3zAK79jcrnhpRcx4/edit?usp=sharing)

