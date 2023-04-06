# Channel List

The source data is in `/channels`. Each channel has its own file with the filename being the channelId representation as name and `.json` as extension.

## Example

two files (`yourChannelId.json` and `yourChannelId.png` ) are required:

```
└── channels
    ├── info
    │   └── yourChannelId.json
    └── logo
        └── yourChannelId.png
```

If you wish to add your Channel, please follow the Channel template :

```json
{
	"channelId": 1,
	"name": "XXX",
	"description": "xxx",
	"website": "https://xxxx.xxx",
	"tag": ["forum"],
	"logo": {
		"width": 1000,
		"height": 1000,
		"format": "png"
	}
}
```

## Aggregation

There are also aggregated json files with all channels automatically assembled:

- https://xxxx.org/channels.json

## Collision management

- We cannot allow more than one channel with the same channelID.
- The first pull request gets the channelID assigned.
- All pull requests trying to replace a channelID because they think their channel is better than the other will be closed.

## Listing sites

- [xxxx.org](https://xxxx.org)

Your project - contact us to add it here!
