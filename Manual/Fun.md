## Coin
`/coin` - [All] Flips a coin and returns either Heads or Tails.  
-# This command can be called anywhere.

## Echo
`/echo (Message) (Reply) (Silent) (Attachment) (Spoiler)` - [Hardware] Make Kosaka say anything you want.  
- `Message` | String representing which message Kosaka should send.
- `Reply` (Optional) | String representing the Message ID of which message Kosaka should reply to.
- `Silent` (Optional, default False) | Boolean indicating if the message should ping or not.
- `Attachment` (Optional) | Attachment that Kosaka should upload.
- `Spoiler` (Optional, default False) | Boolean indicating if the Attachment is a spoiler.

## Random Message
`/random_message` - [All] Display a completely random message from the currently active channel.  
-# Notice: This command gets significantly slower the more messages the channel contains.

## Roll
`/roll (Min: int = 0) (Max: int = 100)` - [All] Randomly returns a number in-between (Min) and (Max) in a Terraria-styled message.  
__Notice__: This command warns the roll was rigged if a custom value for (Min) or (Max) was specified.
-# This command can be called anywhere.