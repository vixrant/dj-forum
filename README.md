DJ-Lit-Forum
============
Forum Application by DJ Literary Society
-----------------------------------------

A forum web app for the entire college of Dwarkadas J. Sanghvi by a member of the technical co-committee in DJ Literary Society. The forum makes use of different categories for the different departments and threads in each of these categories.

## Technology Stack

Base forum
- [Misago](https://misago-project.org) Forum Framework.
    - Built on top of Django.
    - Postgresql database.
    - React.JS frontend with Bootstrap4 theme.



_____



## Developer notes

1. The pages are generated using React.js.

2. Misago is kinda picky when it comes to customisation. Refer "Frontend" for more information.

3. I've left a few notes around the styling about what changes I've made to the theme. You can CTRL-F for "VIKINOTE" to find them. This will be useful for future maintenance.

4. Misago isn't documented very well. Use the debug toolbar on the development server and dev tools in your browser to figure crap out.

_____

### Frontend

The `_frontend_` folder is cloned from Misago's source code. 

#### How it's organised:

1. There are LESS files for separate components of the entire website.
2. HTML Templates can be found in the same folder.
3. React.JS scripts are also available for modifications.

#### How to work on these:

- Styling:
    1. `cd _frontend_`
    2. Install all Node.JS dependencies.
    3. Edit the gulp file to target Misago's template folder.
    4. Run `gulp watchstyle`.
    5. As you change the styling in the LESS files you'll see them reflect on every refresh.

- Templating:
    1. Copy a template from the `_frontend_/templates/` folder into the main project's `theme/templates/`.
    2. Make your changes and they will be registered on every refresh.

- Other styling:
    + `gulp --tasks` has a bunch of tasks you can use.

- Backend:
    + It's a Django backend! Still pretty flexible.

