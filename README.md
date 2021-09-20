# InsightVM - Bulk delete assets

With my team we were trying to delete some assets that might be potentially ghost assets trying to follow InsightVM recommendations and we got an inconvenience because if we try to do this with the console we can only delete the selected assets that were showed per page up to a maximum 500 each time.
The thing is this task became a little tedious and we decided to 'automate' this with a cron job that runs from time to time and wipes out a ghost assets dinamic group that we created.

## Usage
_Replace the vars inside brackets with your own information_
```bash
./bulk_delete_assets
 ┌┐ ┬ ┬┬  ┬┌─  ┌┬┐┌─┐┬  ┌─┐┌┬┐┌─┐  ┌─┐┌─┐┌─┐┌─┐┌┬┐┌─┐
 ├┴┐│ ││  ├┴┐   ││├┤ │  ├┤  │ ├┤   ├─┤└─┐└─┐├┤  │ └─┐
 └─┘└─┘┴─┘┴ ┴  ─┴┘└─┘┴─┘└─┘ ┴ └─┘  ┴ ┴└─┘└─┘└─┘ ┴ └─┘
 Created by @buscoma
 Repo https://github.com/buscoma/bulk_delete_assets
 Enter your console URL - ex.[insightvm.yourdomain.com] >> {{CONSOLE_URL}}
 Username >> {{CONSOLE_USERNAME}}
 Password >> {{CONSOLE_PASSWORD}}
 Enter the name of the group from which you want to delete all assets - ex.[ghost-assets] >> {{GROUP_TO_DELETE}}
> The groupnumber is 90
 Are you sure you want to delete 750 assets? [y/n] >> {{CONFIRMATION}}
> This may take a while, you might want to grab a coffee meanwhile ☕ ...
> Assets deleted!!
```

## InsightVM Console Cleanup recommendations
[![InsightVM Console Cleanup](https://github.com/buscoma/bulk_delete_assets/blob/main/insightvm.png?raw=true)](https://share.vidyard.com/watch/oPgWFYHYc6Gnr2k6kB9fkb "InsightVM Console Cleanup")

## Contributing
Pull requests are welcome. Feel free to contribute on anything you think could be done better.

## Disclaimer
As the main functionality of this script is to massively delete assets associated to a dynamic group using InsightVM API calls, please use it under your own responsibility.
