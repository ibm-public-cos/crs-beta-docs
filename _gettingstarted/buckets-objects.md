---
layout: page
title:  "Managing buckets & objects"
featured: true
weight: 3
tags: []
author: Nick
dateAdded: August 18th, 2016
---
> IBM COS Standard Cross Region is currently in beta, and only available to registered users.  Please contact [IBM sales](mailto:insidesales@cleversafe.com?subject=Beta Request) to enroll if not registered.

The user interface portal provides a high level view of a storage account.  It is possible to create buckets and upload objects using the portal, but typically most interaction with the object store is done through the API by a client application.

#### Using buckets
1. Click the Account Name in the above accounts list to open the details page for that account.
2. The details page shows the following info on the top header bar:
    * Name of the account currently being viewed
    * The current region being viewed
    * The total capacity usage in the current billing cycle
    * The total bandwidth usage in the current billing cycle
3. The page also shows the list of buckets present in the account.
4. A new bucket can be added by clicking on the **+** button at the right of the first row.
5. The new bucket name can be entered and the new bucket added, by clicking the **Add** button. Bucket names must be DNS-compliant (between 3 and 63 characters long, can not be formatted as an IP address, and can not begin or end with a period) and must be globally unique (possibly by appending a UUID or other disctictive suffix to bucket names). 
6. A bucket can be deleted, by clicking the red **-** button to the extreme right of the bucket name. This opens a confirmation window.
7. Click the **Delete** button to remove the bucket from the account. **Note: only empty buckets can be deleted**.  Attempting to delete a non-empty bucket will result in an error.

#### Using objects
1. The objects present within a bucket can be viewed, by clicking the bucket name on the buckets list.
2. The header is updated to include the following info:
    * Name of the account currently being viewed
    * The current region being viewed
    * The name of the bucket whose objects are currently displayed
    * The type of the bucket whose objects are currently displayed
3. Above the grid on the left is a link with the name of the bucket currently viewed. Click the link to show the list of buckets again.
4. The grid shows the list of objects in the bucket.
5. A new object can be added, by clicking the **+** button at the right of the first row.
6. The file can be selected from the file system, by clicking the **select** button and the new file uploaded, by clicking the **Add** button.  When using the portal to add an object, file size is limited to 20 megabytes.
7. An object can be deleted, by clicking on the red **-** button to the extreme right of the object name. This opens a confirmation window.
8. Click the **Delete** button to remove the object from the bucket.
