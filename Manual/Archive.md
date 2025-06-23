## Manager
(Event Type):
- `All` | Every single Event Archived.
- `Message` | Every single Message-Type Events archived.
- `Snipe` | Every single Message-Type Events archived that have either been deleted or edited.
- `Normal` | Only Message-Type Events archived that have never been deleted or edited.
- `Edited` | Only Message-Type Events archived that have been edited.
- `Deleted` | Only Message-Type Events archived that have been deleted.
- `System` | Only System-Type Events such as interactions that have been archived.

`/archive dump (Event_Type: Event_Type = "All")` - [Kernel] Uploads the JSON File containing all Events archived by Kosaka and filtered by (Event Type).  
__Quirk__: The uploaded JSON is not identical to what is stored, the JSON File is Compressed and is from Oldest Event to Newest on Kosaka's side.  

`/archive delete` - [Kernel] Wipes entirely the archive for the current channel.  

`/archive view (Event_Type: Event_Type = "Snipe")` - [Root] Initializes the Archive Browser, an interactive view which lets you visualize Archived Events.
- `←` | Advance 1 Event in the Future.
- `→` | Advance 1 Event in the Past.
- `↑` | Advance 1 Event History in the Future.
- `↓` | Advance 1 Event History in the Past.
- `👁️` | Displays the Event publicly.

## Loggers
This sub-module is in charge of automatically writing Events to the Archive.  
__The following Events are recorded__:
- Executed Slash Commands
- New / Edited / Deleted Message
- New / Leaving / Banned / Updated Members
- Reactions (History not recorded)
Message Archives are stored under `Data/Archive/Messages/[Guild_ID]/[Channel_ID].cjson` while User Archives at `Data/Archive/Users/[User_ID].cjson` as a 7z Compressed JSON file.