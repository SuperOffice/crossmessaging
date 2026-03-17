# Cross messaging between SuperOffice CRM (Web) and embedded web panel (iframe) applications

This sample demonstrates how window.postMessage can be used for communication from embedded web panels to SuperOffice CRM.

The script file `SoClientCrossMessaging.js` is provided as a convenience wrapper around window.postMessage with the supported commands.

There are three supported commands:

- SuperOffice.ClientCrossMessaging.refresh()
- SuperOffice.ClientCrossMessaging.executeSoProtocol(soprotocol)
- SuperOffice.ClientCrossMessaging.openDocument(documentId)

## Sample instructions

- Add a web panel to your SuperOffice CRM installation linked to index.html
- Open SuperOffice and the web panel
- Click refresh or soprotocol buttons, or enter a document id and click 'open document'.
- Observe the changes in the SuperOffice CRM client

## Add to your partner application/web panel

- Include the file `SoClientCrossMessaging.js` file in your application
- Call the methods `SuperOffice.ClientCrossMessaging.refresh`/`SuperOffice.ClientCrossMessaging.executeSoProtocol` when necessary

## Availability

Note that this functionality was made available from version 8.1, released october 2016.
