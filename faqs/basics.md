# FAQs

### Why do we need OlympusDAO in the first place?

Dollar-pegged stablecoins have become an essential part of crypto due to their lack of volatility as compared to tokens such as Bitcoin and Ether. Users are comfortable with transacting using stablecoins knowing that they hold the same amount of purchasing power today vs. tomorrow. But this is a fallacy. The dollar is controlled by the US government and the Federal Reserve. This means a depreciation of dollar also means a depreciation of these stablecoins.

OlympusDAO aims to solve this by creating a non-pegged stablecoin called OHM. By focusing on supply growth rather than price appreciation, OlympusDAO hopes that OHM can function as a currency that is able to hold its purchasing power regardless of market volatility.

### Is OHM a stable coin?

No, OHM is not a stable coin. Rather, OHM aspires to become an algorithmic
reserve currency backed by other decentralized assets. Similar to the idea of
the gold standard, OHM provides free floating value its users can always fall
back on, simply because of the fractional treasury reserves OHM draws its
intrinsic value from.

### OHM is backed, not pegged.

Each OHM is backed by 1 DAI, not pegged to it. Because the treasury backs every OHM with at least 1 DAI, the protocol would buy back and burn OHM when it trades below 1 DAI. This has the effect of pushing OHM price back up to 1 DAI. OHM could always trade above 1 DAI because there is no upper limit imposed by the protocol. Think pegged == 1, while backed >= 1.

You might say that the OHM floor price or intrinsic value is 1 DAI. We believe that the actual price will always be 1 DAI + premium, but in the end that is up to the market to decide.

### How does it work?

At a high level, OlympusDAO consists of its protocol managed treasury, protocol owned liquidity, bond mechanism, and high staking rewards that are designed to control supply expansion.

Bond generates profit for the protocol, and the treasury uses the profit to mint OHM and distribute them to stakers. With LP bond, the protocol is able to accumulate liquidity to ensure the system stability.

### What is the deal with (3,3) and (1,1)?

(3,3) is the idea that, if everyone cooperated in Olympus, it would generate the greatest gain for everyone (from a [game theory](https://en.wikipedia.org/wiki/Game_theory) standpoint). Currently, there are three actions a user can take:

- Staking (+2)
- Bonding (+1)
- Selling (-2)

Staking and bonding are considered beneficiary to the protocol, while selling is considered detrimental. Staking and selling will also cause a price move, while bonding does not (we consider buying OHM from the market as a prerequisite of staking, thus causing a price move). If both actions are beneficiary, the actor who moves price also gets half of the benefit (+1). If both actions are contradictory, the bad actor who moves price gets half of the benefit (+1), while the good actor who moves price gets half of the downside (-1). If both actions are detrimental, which implies both actors are selling, they both get half of the downside (-1).

Thus, given two actors, all scenarios of what they could do and the effect on the protocol are shown here:

![](../.gitbook/assets/faqs/game_theory.png)

- If we both stake (3, 3), it is the best thing for both of us and the protocol (3 + 3 = 6).
- If one of us stakes and the other one bonds, it is also great because staking takes OHM off the market and put it into the protocol, while bonding provides liquidity and DAI for the treasury (3 + 1 = 4).
- When one of us sells, it diminishes effort of the other one who stakes or bonds (1 - 1 = 0).
- When we both sell, it creates the worst outcome for both of us and the protocol (-3 - 3 = -6).

### Why is PCV important?

As the protocol controls the funds in its treasury, OHM can only be minted or burned by the protocol. This also guarantees that the protocol can always back 1 OHM with 1 DAI. You can easily define the risk of your investment because you can be confident that the protocol will indefinitely buy OHM below 1 DAI with the treasury assets until no one is left to sell. You can't trust the FED but you can trust the code.

As the protocol accumulates more PCV, more runway is guaranteed for the stakers. This means the stakers can be confident that the current staking APY can be sustained for a longer term because more funds are available in the treasury.

### What will happen if there is a bank run on Olympus?

Fractional reserve banking works because depositors don’t withdraw their funds all at once. A depositor’s faith in the banking system rests on regulations and agencies like Federal Deposit Insurance Corporation (FDIC).

OHM does not have FDIC insurance but it has an incentive structure that protects stakers. Let’s take a look at how it performs during a hypothetical bank run. In this scenario, we assume the majority of stakers would panic and unstake their tokens from Olympus - the staking percentage which stands at 92% now quickly collapses to 3.3%, leaving only 20,000 OHM staked.

Next, we assume the Risk-Free Value (RFV) inflows to the treasury completely dry up. For context, RFV is currently growing at about $1 million every 3 days. However, during a bank run this growth will likely stop.

Finally, we assume that those last standing stakers bought in at a price of $500 per OHM. The initial investment of these stakers would be:

$$
\$500/OHM * 20,000\ OHM = \$10\ million
$$

As of July 12 2021, the total OHM supply is 734,421 and the RFV is $13,905,970. Remember that 1 OHM is backed by 1 USD (DAI or FRAX). By subtracting these two numbers, we know 13,171,549 OHM will eventually get issued to the remaining stakers. In roughly a year, these stakers who are holding 20,000 OHM will have:

$$
20,000 + 13,171,549 = 13,191,549\ OHM
$$

$10 million investment made by these stakers will turn into about $13.2 million based on cash flow alone if they stay staked (recall that 1 OHM is backed by 1 USD). In this bank run scenario, the stakers who stay staked not only get their money back, but also make some profit. Therefore, [(3,3)](#what-is-the-deal-with-33-and-11) isn’t just a popular meme, it is actually a dominant strategy.

The above scenario is unlikely to play out because when other people find out that extremely high rewards are being paid to the stakers, they will copy the strategy by buying and staking OHM. This is also why the percentage of OHM staked in Olympus has consistently remained over 90% since launch.

*Note: Most of the data referenced above are taken from [this Dune Analytics page](https://duneanalytics.com/shadow/Olympus-(OHM)).*

### Why is the market price of OHM so volatile?

It is extremely important to understand how early in development the OlympusDAO protocol is. A large amount of discussion has centered around the current price and expected a stable value moving forward. The reality is that these characteristics are not yet determined. The network is currently tuned for expansion of OHM supply, which when paired with the staking, bonding, and yield mechanics of OlympusDAO, result in a fair amount of volatility.

OHM could trade at a very high price because the market is ready to pay a hefty premium to capture a percentage of the current market capitalization. However, the price of OHM could also drop to a large degree if the market sentiment turns bearish. We would expect significant price volatility during our growth phase so please **do your own research** whether this project suits your goals.

### What is the point of buying it now when OHM trades at a very high premium?

When you buy and stake OHM, you capture a percentage of the supply (market cap) which will remain close to a constant. This is because your staked OHM balance also increases along with the circulating supply. The implication is that if you buy OHM when the market cap is low, you would be capturing a larger percentage of the market cap.

### What is a rebase?

Rebase is a mechanism by which your staked OHM balance increases automatically. When new OHM are minted by the protocol, a large portion of it goes to the stakers. Because stakers only see staked OHM balance instead of OHM, the protocol utilizes the rebase mechanism to increase the staked OHM balance so that 1 staked OHM is always redeemable for 1 OHM.

### What is reward yield?

Reward yield is the percentage by which your staked OHM balance increases on the next epoch. It is also known as *rebase rate*. You can find this number on the [Olympus staking page](https://app.olympusdao.finance/#/stake).

### What is APY?

APY stands for annual percentage yield. It measures the real rate of return on your principal by taking into account the effect of compounding interest. In the case of OlympusDAO, your staked OHM represents your principal, and the compound interest is added periodically on every epoch (2200 Ethereum blocks, or around 8 hours) thanks to the rebase mechanism.

One interesting fact about APY is that your balance will grow not linearly but exponentially over time! Assuming a daily compound interest of 2%, if you start with a balance of 1 OHM on day 1, after a year, your balance will grow to about 1377. That is a lot!

<p align="center">
   <img width="721" height="446" src="../.gitbook/assets/faqs/apy.png" alt="The power of compounding">
</p>

### How is the APY calculated?

The APY is calculated from the reward yield (a.k.a rebase rate) using the following equation:

$$
APY = ( 1 + rewardYield )^{1095}
$$

It raises to the power of 1095 because a rebase happens 3 times daily. Consider there are 365 days in a year, this would give a rebase frequency of 365 * 3 = 1095.

Reward yield is determined by the following equation:

$$
rewardYield = OHM_{distributed} / OHM_{totalStaked}
$$

The number of OHM distributed to the staking contract is calculated from OHM total supply using the following equation:

$$
OHM_{distributed} = OHM_{totalSupply} \times rewardRate
$$

Note that the reward rate is subject to change by the protocol. For example, it has been revised due to [this latest proposal](https://forum.olympusdao.finance/d/37-oip-11-reducing-reward-rate).

### Why does the price of OHM become irrelevant in long term?

As illustrated above, your OHM balance will grow exponentially over time thanks to the power of compounding. Let's say you buy an OHM for $400 now and the market decides that in 1 year time, the intrinsic value of OHM will be $2. Assuming a daily compound interest rate of 2%, your balance would grow to about 1377 OHMs by the end of the year, which is worth around $2754. That is a cool $2354 profit! By now, you should understand that you are paying a premium for OHM now in exchange for a long-term benefit. Thus, you should have a long time horizon to allow your OHM balance to grow exponentially and make this a worthwhile investment.

### What will be OHM's intrinsic value in the future?

There is no clear answer for this, but the intrinsic value can be determined by the treasury performance. For example, if the treasury could guarantee to back every OHM with 100 DAI, the intrinsic value will be 100 DAI. It can also be decided by the DAO. For example, if the DAO decides to [raise the price floor of OHM](https://forum.olympusdao.finance/d/31-use-price-floor-as-tool-for-monetary-policy), its intrinsic value will rise accordingly.

### How does the protocol manage to maintain the high staking APY?

Let’s say the protocol targets an APY of 100,000%. This would translate to a rebase rate of about 0.6328%, or a daily growth of about 2%. Please refer to the equation above to learn [how APY is calculated from the rebase rate](#how-is-the-apy-calculated).

If there are 100,000 of OHM staked right now, the protocol would need to mint an additional 2000 OHM to achieve this daily growth. This is achievable if the protocol can bring in at least 2000 DAI daily from bond sales. If the protocol fails to achieve this, the APY of 100,000% cannot be guaranteed.

### Do I have to unstake and stake OHM on every epoch to get my rebase rewards?

No. Once you have staked OHM with OlympusDAO, your staked OHM balance will auto-compound on every epoch. That increase in balance represents your rebase rewards.

### How do I track my rebase rewards?

You can track your rebase rewards by calculating the increase in your staked OHM balance.

1. Record down the Current Index value on the [staking page](https://app.olympusdao.finance/#/) when you first stake your OHM. Let's call this the Start Index.

    ![Start index](../.gitbook/assets/faqs/start_index.png)

2. After staking for some time, if you want to determine by how much your balance has increased, check the Current Index value again. Let's call this the End Index.

    ![End index](../.gitbook/assets/faqs/end_index.png)

3. By dividing the End Index by Start Index, you would get the ratio by which your staked OHM balance has increased.

    $$
    ratio = endIndex / startIndex
    $$
