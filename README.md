# InsightVM - Bulk delete assets

With my team we were trying to delete some assets that might be potentially ghost assets trying to follow InsightVM recommendations and we got an inconvenience because if we try to do this with the console we can only delete the selected assets that were showed per page up to a maximum 500 each time.
The thing is this task became a little tedious and we decided to 'automate' this with a cron job that runs from time to time and wipes out a ghost assets dinamic group that we created.

## Usage
_Replace the vars inside brackets with your own information_
```bash
./bulk_delete_assets -h
 ┌┐ ┬ ┬┬  ┬┌─  ┌┬┐┌─┐┬  ┌─┐┌┬┐┌─┐  ┌─┐┌─┐┌─┐┌─┐┌┬┐┌─┐
 ├┴┐│ ││  ├┴┐   ││├┤ │  ├┤  │ ├┤   ├─┤└─┐└─┐├┤  │ └─┐
 └─┘└─┘┴─┘┴ ┴  ─┴┘└─┘┴─┘└─┘ ┴ └─┘  ┴ ┴└─┘└─┘└─┘ ┴ └─┘
 Created by @buscoma - amocsub@pm.me
 Repo https://github.com/buscoma/bulk_delete_assets

Delete assets from an InsightVM console massively from a specified Asset Group

USAGE:
    ./bulk_delete_assets [OPTIONS]

OPTIONS:
    -c <insightvm-console>
        Your console URL - ex.[insightvm.yourdomain.com]
    -u <username>
        Username to authenticate with the console
    -p <password>
        Password to authenticate with the console
    -n <asset-group-name>
        Asset group name to be deleted
    -f
        Force the script to run without asking for confirmation
    -h
        Print this help message

```

## InsightVM Console Cleanup recommendations
[![InsightVM Console Cleanup](https://github.com/buscoma/bulk_delete_assets/blob/main/insightvm.png?raw=true)](https://share.vidyard.com/watch/oPgWFYHYc6Gnr2k6kB9fkb "InsightVM Console Cleanup")

## Contributing
Pull requests are welcome. Feel free to contribute on anything you think could be done better.

## Disclaimer
As the main functionality of this script is to massively delete assets associated to a dynamic group using InsightVM API calls, please use it under your own responsibility.
