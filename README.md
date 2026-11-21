# claude-open

A static redirect page for Telegram buttons: Telegram inline buttons accept only `https://` links, so error-report-service links to `https://vial.github.io/claude-open/open.html#<url-encoded claude://code/new?...>`, and the page opens Claude Desktop with that link.

The link travels only in the URL fragment, which browsers never send to the server. The page accepts only `claude://code/new?` links, has no scripts from other hosts and no analytics.
