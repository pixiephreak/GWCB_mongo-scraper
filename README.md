# Contactually Lite v1 (beta)
Contactually Lite allows users to manage their contacts and buckets 

## To use the app:

1) `yarn install` (`npm install yarn -g` if you don't have it yet)

2) `yarn start`

3) In your browser, you'll be prompted to sign in to a Contactually account on our staging environment.

4) if you have a verified account, you’ll be able to see/manage your contacts

## v1 Issues:

**Using react-router-dom v4 with redux, there is problem with receiving data asynchronously from the store and mounting components, which leads to a breaking error message on hot reloads. _For now, each page can be reloaded using a hard refresh_.  With more time, I will probably use redux-thunk middleware to set a loading variable in the store for each function in actions.js to make the app usable.**

- implement unit testing throughout the app.
- move omg assets to their own folder
- /index background and all tables should be responsive.
- create a fallback for users without contacts, buckets. etc.
- add header with name of each bucket at route bucket/:id
- address how to patch e-mail addresses (variance in API design between v1/v2)
- ask users to confirm before deleting a contact
- validate all form input fields with redux-form validation
- paginate contacts
- finish create/edit bucket feature
