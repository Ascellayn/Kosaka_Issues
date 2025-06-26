## Guild
`/settings_guild dump` - [Kernel] Uploads the JSON File containing the Server's Configuration file.  
Here are the default values and description for each JSON Key and values:
```JSON
{
	# Archiver Related Settings
	"Archiver": {
		"Allow_Archiving": true # [Bool] Should the Archiver be allowed to Archive any events inside the server? Set to "false" for privacy reasons.
	},

	# Random Message Related Settings
	"Random_Message": {
		"Allow_Caching": true # [Bool] Should Random Message allow to cache the messages that have been fetched? Set to "false" for privacy reasons, note this will make subsequent usage of the command significantly slower.
	}
}
```
**Note that JSON files cannot contain comments, as such the comments (text that begin with "#") should not be included in the uploaded JSON file**  
The JSON file thus needs to be edited externally using a text editor such as Visual Studio Code, GNU/Nano, Notepad++, etc.

`/settings_guild load (File)` - [Kernel] Upload a JSON File containing the Server's Configuration file to be applied to the Server.  
See the information about `/settings_guild dump` for more information. Also don't try to be funny. Kosaka will get really mad if you fuck with the JSON file with malicious intent.