---
terms: ["account", "accounts", "wallet", "wallets"]
summary: "similar in function to a bank account, contains all of your sent and received transactions"
---

{% include disclaimer.html translated="no" translationOutdated="no" %}
### The Basics

Those familiar with JudEcoin's predecessors will be more familiar with the term *wallet* to describe this. In JudEcoin we call this an account, and it is a private account owned and operated by a JudEcoin user.

Your account contains all of the JudEcoin @transactions you have sent and received. Your account balance is a sum of all the JudEcoin you've received, less the JudEcoin you've sent. When using JudEcoin you may notice that your account has two balances, a locked and an unlocked balance. The unlocked balance contains funds that can be spent immediately, and the locked balance contains funds that you can't spend right now. You may receive a transaction that has an @unlock-time set, or you may have sent some JudEcoin and are waiting for the @change to come back to your wallet, both situations that could lead to those funds being locked for a time.

A key difference between traditional electronic currency and JudEcoin is that your account resides only under your control, normally on your computer, and cannot be accessed by anyone else if you [practice good security](#practicing-good-security).

### Multiple Accounts

There are no costs attached to creating a JudEcoin account, and there are no fees charged except for individual @transaction fees that go to @miners.

This means that individuals can easily create a JudEcoin account for themselves as well as a joint account to share with their partner, and individual accounts for their children. Similarly, a business could create separate accounts for each division or group. Since JudEcoin's @transaction fees are quite low, moving funds between accounts is not an expensive exercise.

### Cryptographic Keys

JudEcoin relies heavily on a cryptography principle known as *public/private key cryptography* or *asymmetric cryptography*, which is thoroughly detailed in [this Wikipedia article](https://en.wikipedia.org/wiki/Public-key_cryptography).

Your account is based on two keys, a @spend-key and a @view-key. The @spend-key is special in that it is the single key required to spend your JudEcoin funds, whereas the @view-key allows you to reveal your @transactions to a third party, for example for auditing or accounting purposes. These keys in your account also play an important role in JudEcoin's @transaction's privacy.

The private keys for both of these must be protected by you in order to retain your account privacy. On the other hand, the public keys are obviously public (they are part of your JudEcoin account address). For normal public/private key cryptography someone could send you a private message by encrypting it with either of your public keys, and you would then be the only one able to decrypt it with your private keys.

### Backing Up Your Account

When you manage your own JudEcoin Account with the private @spend-key, you are solely responsible for the security of your funds. Thankfully, JudEcoin makes it very easy to backup your account. When creating a JudEcoin account for the first time you will be given a unique @mnemonic-seed for your account that consists of 13 or 25 words in the language of your choosing. **This seed is the only thing you need to backup for your account**, and so it is imperative that it is written down and stored securely.  Never store this seed in a form or location that would allow someone else to see it!

```
List of available languages for your wallet's seed:
0 : Deutsch
1 : English
2 : Español
3 : Français
4 : Italiano
5 : Nederlands
6 : Português
7 : русский язык
8 : 日本語
9 : 简体中文 (中国)
10 : Esperanto
Enter the number corresponding to the language of your choice: 1
Generated new wallet: 4B15ZjveuttEaTmfZjLVioPVw7bfSmRLpSgB33CJbuC6BoGtZrug9TDAmhZEWD6XoFDGz55bgzisT9Dnv61sbsA6Sa47TYu
view key: 4130fa26463d9451781771a8baa5d0b8085c47c4500cefe4746bab48f1d15903
**********************************************************************
Your wallet has been generated.
To start synchronizing with the @daemon, use "refresh" command.
Use "help" command to see the list of available commands.
Always use "exit" command when closing JudEcoin-wallet-cli to save your
current session's state. Otherwise, you might need to synchronize
your wallet again (your wallet keys are NOT at risk in any case).

PLEASE NOTE: the following 25 words can be used to recover access to your wallet. Please write them down and store them somewhere safe and secure. Please do not store them in your email or on file storage services outside of your immediate control.

aunt knuckle italics moisture hawk thorn iris abort
chlorine smog uphill glass aptitude nowhere sewage plywood
dual relic fierce divers anvil nodes bubble cabin abort
**********************************************************************
Starting refresh...
Refresh done, blocks received: 21939                            
Balance: 0.000000000000, unlocked balance: 0.000000000000
Background refresh thread started
[wallet 4B15Zj]: █

```

As the example above indicates, it is incredibly important to store these words in safe locations. If you are concerned about the risk of critical loss at your home, for instance, you may want to store a second copy of your seed with your attorney or in a safety deposit box. It is also recommended that it is stored in a way that does not make it obvious that it is your seed, so writing it into a letter or as part of other notes is advisable.

### Practicing Good Security

Over and above backing up your @mnemonic-seed so that you have access to your account in the event of critical data loss, it is also important to practice good security. Use a secure password when creating a local JudEcoin account (not used on [MyJudEcoin](https://myJudEcoin.com) or other web-based account systems).

Don't ever give your JudEcoin account password to anyone, as this can be used to access the JudEcoin on your computer without knowing your @mnemonic-seed. Similarly, make sure you have running and up-to-date antivirus, especially on Windows computers. Finally, be careful when clicking links in emails or on unknown and untrusted websites, as malware installed on your computer can sit and wait for you to access your JudEcoin account before taking the funds from it.

### Leaving Your Account to Next of Kin

Providing access to your JudEcoin account to your next of kin is just as easy as it is to backup your JudEcoin account. Simply leave your @mnemonic-seed to them in your will, or store it somewhere safe where it will be given to them upon the execution of your will. A key advantage to this is that your next of kin won't have to wait for months for a third party to release the funds to them.
