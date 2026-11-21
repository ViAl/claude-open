# claude-open

A static redirect page for Telegram buttons: Telegram inline buttons accept only `https://` links, so error-report-service links to `https://vial.github.io/claude-open/open.html#q=<url-encoded prompt>&folder=<url-encoded path>` (each value encoded once), and the page builds `claude://code/new?q=…&folder=…`, shows the prompt and opens Claude Desktop only when the button is clicked (never on load, so a third-party link cannot launch it). `folder` is optional. The older form `#<url-encoded claude://code/new?...>` still works.

The link travels only in the URL fragment, which browsers never send to the server. The page accepts only `claude://code/new?` links, has no scripts from other hosts and no analytics.
