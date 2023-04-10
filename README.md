# Channel List

The source data is in `/channels`. Each channel has its own file with the filename being the channelId representation as name and `.json` as extension.

## How to submit a new channel, or any changes

1. Fork the project
2. Clone your forked copy onto your PC
3. Create a new branch, make the required changes, test it locally using the above method
4. Commit to your branch and push to your repo
5. Go to your repo's github page and click Submit a pull request

This article is also a good explainer on the pull request system: https://opensource.com/article/19/7/create-pull-request-github

If you need help with the above process you can open a new Issue https://github.com/Social-xxx/channel-list/issues

## Channel Example

two files (`yourChannelId.json` and `yourChannelId.png` ) are required:

```
└── channels
    ├── info
    │   └── yourChannelId.json			e.g.: 1.json
    └── logo
        └── yourChannelId.png			e.g.: 1.png
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

- `channelId` : This is your channelId
- `name` : This is your channel name
- `description` : This is your channel description
- `website` : This is your website if you have
- `tag` : Your channel type. e.g. `["finance","forum"]`
- `logo` : Description of `logo/yourChannelId.png`

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
