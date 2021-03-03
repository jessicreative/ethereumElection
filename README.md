# ethereumElection

Go onto remix.ethereum.org

Add the file "Election.sol" in my repository under the contracts folder and get rid of other files ending in .sol.

Compile (turn auto compile on).

Go to the deploy and run transactions tab.

Set environment as Javascript VM.

Choose an account to start with as the owner of the account - it will be the only account that can authorize other accounts to vote and add candidates in this election. Copy paste in the address or name of the accounts you want to authorize (including this initial one you act as) by going to the top, switching to the specific person you want to authorize, and copying the "account" field. Then switch back to the original account since that's the only one allowed to authorize all. Press transact each time you paste the address name in the authorize field to authorize.

In the field "Add Candidate", add a candidate name with "" around it and click transact to add the candidate. Continue until you are done adding all the candidates. This will go into the array called candidates.

You can now put in index (starting from 0) with quotation "" around the number in the field "candidates", then press "call" to see the name of the candidate and the current number of votes that they have.

If you wish to vote for a certain candidate from a certain account, make sure first the first owner account has authorized the account. Then switch to the account. Then using the corresponding index that matches with the name (which you can double check from the call field), put that into the vote field and press transact. Now when you type in the candidate index in the candidates field you can see their updated vote count.

The other buttons below will show you more data about the election, including the number of votes, the owner accoutn, and if you put in address of the account in the "voters" field and press call, you will see the status of the voter - if they are shown to have already voted, they can't vote again.


Credits to https://www.youtube.com/watch?v=ucszgKGFnwc. A lot of the bugs that no longer work are fixed in my current code, and my readme has more thorough descriptions of how to navigate the IDE and proceed with the election.
