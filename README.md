# DominoReplicationHistoryCleaner
Cleare replication history for database using C API

Working example how to clear replication history programatically using C API.

STATUS LNPUBLIC NSFDbClearReplHistory(DBHANDLE  hDb, DWORD  dwFlags);

## Description

This function clears out the replication history information of the specified database replica.  This can also be done using the Notes user interface via the File/Replication/History menu item selection.

## Parameters

Input :
hDb  -  Handle to the database, already opened.

dwFlags  -  Must be zero.

## Output :
(routine)  -  Return status from this call: 

NOERROR - Successfully cleared replication history information.

ERR_xxx - Other errors returned by this function and includes errors returned by lower level functions. Call OSLoadString to obtain a string to display to the user.
