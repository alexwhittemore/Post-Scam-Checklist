# Checklist for Post-Scam

# Facts

You fell for a tech support scam, called the scammers, wrote them a check for $400 and sent them an image of just the front. They had remote control of the PC for an extended period of time, effectively or actually unsupervised. 

This means **they have your checking account number, home address, phone number, and bank name**. It means they may have logged into any account with a password saved on your computer, provided they thought to try that account. **It should be assumed all accounts are compromised, though they probably aren't**. Since they were able to log into your bank account from your computer, **it's possible they know your account balance, which with the info on the check is enough to drain it in one transaction.** 

In particular, the fact that you can no longer log in to your primary bank account indicates either that it was locked, OR that the scammers DID log in and changed the username to keep you out. It would be unlikely for them to only change the username, but the account does not notify your email about a username change, so it's possible the scammer locked you out stealthily. 

The online banking interface for this account does not show the account ACH numbers, so it's unlikely any numbers but the checking account on the check have been compromised

It sounds like you placed a hold on the account, and it sounds like they said that hold will impact your mortgage payment and retirement distribution tomorrow, which implies the account itself is frozen and not just that they put a stop payment on the check. That's great. 

Immediately after realizing it was a scam, you shut the computer off, which is good both so they don't have ongoing access, if they maintained that, and so any potential ransomware can't carry on locking your files, if maybe they installed some. 

# Triage Steps

# At the bank physical branch

- [ ]  Verify that the main checking account IS, in fact held, which will prevent the check from clearing as well as any potential ACH withdrawals ("demand drafts") initiated with just the numbers.
- [ ]  Review recent transactions for ALL accounts with the bank - savings, checking, HELOC, and any credit cards that could be cash-advanced. Make sure there are NO unexpected transactions
- [ ]  Verify as well that NO ACH transactions have been initiated from the web account in the last couple days.
- [ ]  Open a new checking account, and transfer all the money out of the old checking account into it. The previous account number is compromised, and is now a scam funnel to India. If the account can't be opened immediately for some reason, transfer the money into savings instead, since that account number hasn't been compromised.
- [ ]  Log IN WRITING that all of this has happened, so that anything later landing in court can be appropriately explored.

# At the police station

( You've already done this ) 

- [ ]  File a police report, containing as many circumstantial details as you can, i.e. what website you think you visited, details of the scam, and so on. They won't care, and won't do anything with it, but 1) it's good for statistics, 2) the DOJ is actually maybe-kinda cracking down on scammers, so being on record might be useful and 3) you want to lay as long a paper trail as possible in case it becomes necessary legally trying to recover your money.

# On the Web

From your newly restored machine (below), or ideally from a separate machine that hasn't been compromised, systematically change all your passwords for all relevant accounts:

- Banking accounts
- Email accounts
- Social media accounts

Anything that could conceivably be used to steal money from you, impersonate you, or blackmail you should be sanitized

- [ ]  Email accounts (should be your biggest concern)
    - [ ]  Log in to each account. Check recently sent messages and make sure there's nothing you didn't personally send. The scammer might have tried to exfiltrate some data from your account lazily, or set up some subsequent scam.
    - [ ]  Check recently received email, and make sure there aren't any password reset emails or the like that you didn't personally initiate. Ditto any other banking transaction confirmations or the like.
    - [ ]  Change the account password. Use an entirely unrelated one, ideally random, ideally stored in a password manager. [Correcthorsebatterystaple.net](http://correcthorsebatterystaple.net) if you must have something memorable.
    - [ ]  Enable two-factor authentication if you can. This means you'll be alerted every time anyone anywhere tries to log in to your account, and they'll need your "second factor" to do so successfully. This might be a one-time-code from an app you configure (most secure, but save the setup code in a safe place like a password manager) or a text message to verify you mean to sign in (less secure; susceptible to "sim swap" attacks, but still better than not, and easier).
- [ ]  Bank and Credit Accounts
    - [ ]  Log in to each provider
    - [ ]  Check all recent transactions in each account, and make sure nothing odd is in there.
    - [ ]  View any pending transactions, and make sure there aren't any scheduled transfers or some such
    - [ ]  Change the password
    - [ ]  Enable two-factor authentication if you can.
- [ ]  Social Media accounts
    - [ ]  Log in to each.
    - [ ]  Make sure there are no weird or unexpected messages or posts, or newly approved friends.
    - [ ]  Change the password.
    - [ ]  Enable two-factor authentication if you can.

Ultimately, the goal of this step is to verify that you were the last person to access any and all of your accounts, then lock out future access by changing the password. You can assume the scammer read your password stored in your browser, if they wanted to, and still have it (i.e. didn't JUST log in on your computer while you were(n't) looking.

# Back at home

The computer is off. In a perfect world, you'd remove the hard drive and copy off any valuable files that way before booting it back up, in case there's ransomeware installed trying to encrypt it on you. The real point here is to assume that the computer now has persistent remote access installed on it, and perhaps whatever other malware, I don't know.

- [ ]  Remove the drive and copy data off it with a separate computer, if you can
- [ ]  Disconnect the internet (unplug the cable, or turn off the WIFI router if it's normally on WIFI)
- [ ]  Boot the computer, offline
- [ ]  Copy any files off to a separate disk, like pictures and whatnot.
- [ ]  Take note of any software you have installed, so it'll be easier to reinstall later (open add/remove programs and just write down everything you care about)
- [ ]  Consider what apps you have configured some which way, and how to recover those configurations, like password managers or Adobe Lightroom catalog files or that sort of thing. Any expensive software that has a license key might need to be deactivated to avoid some difficult relicensing process, like Matlab or some such.
- [ ]  Once all data is backed up and any unrecoverable program configurations are exported/saved/noted, reinstall windows from scratch. Click 'Start > Settings > Update & security > Recovery' and then choose 'Get started' under 'Reset this PC'. A full reinstall wipes your entire drive, so select 'Remove everything' to ensure a clean reinstall is performed. This is the most straightforward way to ensure your machine is no-longer compromised.
