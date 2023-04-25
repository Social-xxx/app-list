# App List

The source data is in `/apps`. Each app has its own file with the filename being the app_id representation as name and `.json` as extension.

## How to submit a new app, or any changes

1. Fork the project
2. Clone your forked copy onto your PC
3. Create a new branch, make the required changes, test it locally using the above method
4. Commit to your branch and push to your repo
5. Go to your repo's github page and click Submit a pull request

This article is also a good explainer on the pull request system: https://opensource.com/article/19/7/create-pull-request-github

If you need help with the above process you can open a new Issue https://github.com/Social-xxx/app-list/issues

## App Example

two files (`yourAppId.json` and `yourAppId.png` ) are required:

```
└── apps
    ├── info
    │   └── yourAppId.json			e.g.: 1.json
    └── logo
        └── yourAppId.png			e.g.: 1.png
```

If you wish to add your app, please follow the app template :

```json
{
	"app_id": 1,
	"name": "XXX",
	"description": "xxx",
	"website": "https://xxxx.xxx",
	"admin_address": ["0x886...688", "0x123...456"],
	"tag": ["forum"],
	"logo": {
		"width": 1000,
		"height": 1000,
		"format": "png"
	}
}
```

- `app_id` : This is your app_id
- `name` : This is your app name
- `description` : This is your app description
- `website` : This is your website if you have
- `admin_address` : This is your admin address. (This is the login address for the future administration website.)
- `tag` : Your app type. e.g. `["finance","forum"]`
- `logo` : Description of `logo/yourAppId.png`

## Aggregation

There are also aggregated json files with all apps automatically assembled:

- https://xxxx.org/apps.json

## Collision management

- We cannot allow more than one app with the same appID.
- The first pull request gets the appID assigned.
- All pull requests trying to replace a appID because they think their app is better than the other will be closed.

## Listing sites

- [xxxx.org](https://xxxx.org)

Your project - contact us to add it here!
