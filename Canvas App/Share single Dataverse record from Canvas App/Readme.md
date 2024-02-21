The unmanaged solution CanvasAppShareRecord\_1\_0\_0\_1.zip contains a Canvas App which showcases the capability of the logged in user to share a single Dataverse record from a list of records with a specific user. That user may not have access into the App or the entire Dataverse table, a direct link to the Canvas App screen with the read only view of that specific record will be send via email.

It has been implemented with below logic -

- Deep Linking to a specific screen in the Canvas App
- Calling a Flow from Canvas App to perform below operations-
  - Check if the requested user already has access into the App, if not, provide Read Only access.
  - Check if the requested user already has access into the App, if not, provide Read Only access.
  - Check if the requested user already has access into the Dataverse Record, if not, provide Read Only access.
  - Send a mail to the user with Deep link to that specific screen containing the record.

Please follow the document Canvas App Share Records.docx to make necessary changes in the App and the Flow
