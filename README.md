A pretty dope template that works with any implementation of Atlassian's Statuspage. No auth or API keys required. I used https://status.zoom.us/ for testing but it's totally agnostic. 
It discovers all components on the statuspage api endpoint, creates an item for each component, and a trigger if that component is not either operational or degraded. Of course you could do four different triggers for each severity in the trigger prototypes.

To use, import the template, create a host (Vendor Status Page), assign the template to the host, and override the template macro {$STATUSPAGE.URL} with the statuspage base URL you're looking for. 

Inspired by this Reddit thread: https://www.reddit.com/r/zabbix/comments/1d9mifd/integrate_with_atlassian_status_page/

Happy monitoring!
