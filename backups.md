# Backups

I've fiddled with a few different backup setups, but none really striked the balance of performance, open source-ness, and low battery impact that I was looking for. Prior to my most recent setup, I was using Arq to backup to Backblaze B2, and nearly continued using it after upgrading my personal Macbook Pro. However, after reading [several](https://www.reddit.com/r/Arqbackup/comments/fxt2j3/arq_6_help_needed_i_honestly_have_no_idea_what_to/) [threads](https://www.reddit.com/r/ArqBackup_Community/comments/gk0eym/arq_6_restore_testing_not_real_good/) about major issues with the newest release of Arq, I decided to reevaluate options and ended up choosing [duplicacy](https://github.com/gilbertchen/duplicacy) backed up to B2. 

The CLI is free and the program is open source, and the results have been phenomenal so far, to the extent that I should probably pay for the program just to support its creator. I use [launchd](https://www.launchd.info/) on my Mac to automatically run a python script that backs up the directories I've selected every evening. The configuration is all available on my [Github](https://github.com/lazyIoad/dotfiles/tree/master/backup).

