# block-ru-by
Simple script to block ru &amp; by countries using iptables.

credits: http://www.cyberciti.biz/faq/?p=3402

requirements: wget, egrep, iptables

I updated mentioned above script so we remove only rules what we add, in original script all rules were flushed/deleted from iptables, in case if you have some additional rules there this might be useful.

Probably it is worth to add that script to cron to run it weekly or so:

```
@weekly /path/to/country.block.iptables.sh
```

After server reboot or restart of iptables, it will be worth to remember that those rules will disappear, probably it is worth to run those rules after such events.
