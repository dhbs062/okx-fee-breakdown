# OKX fees: a practical guide to spot, futures, withdrawal and VIP trading costs

If you searched for **OKX fees**, you probably want a simple answer to a not-so-simple question: how much will OKX actually charge when you buy, sell, trade futures, convert crypto, or withdraw funds?

The short version is that OKX does not use one universal fee. Your cost depends on the product, trading pair, order execution, account tier, 30-day volume, asset balance and region. A market order can cost more than a limit order, and a limit order can still receive the taker rate if it fills immediately.

This guide explains the main OKX fees, the current public fee tiers, how maker and taker pricing works, where hidden costs can appear, and which steps can reduce your trading bill.

The information below was checked against OKX’s current public fee information and help documentation on **October 6, 2026**. Fees can change, and the rate shown after signing in to your OKX account is the one that should be treated as final.

## OKX fees at a glance

For the standard spot fee group, the public schedule currently begins at:

- **Regular spot maker fee:** 0.0800%
- **Regular spot taker fee:** 0.1000%
- **Regular futures maker fee:** 0.0200%
- **Regular futures taker fee:** 0.0500%

For a $1,000 spot trade, a 0.1000% taker fee equals approximately **$1**, before considering spread, slippage or any separate conversion cost.

For a $1,000 futures fill, a 0.0500% taker fee equals approximately **$0.50**. Futures traders must also account for funding fees, which are separate from trading fees and can move in either direction depending on the funding rate.

At higher VIP levels, maker fees can become negative. That means the trader may receive a maker rebate rather than pay a maker commission, although eligibility requirements are extremely high and the exact rules depend on the market and jurisdiction.

## What are maker and taker fees?

OKX uses a maker-taker fee model.

A **maker** adds liquidity to the order book. This normally happens when an order is placed at a price that does not immediately match an existing order and remains on the book until another trader fills it.

A **taker** removes liquidity from the order book. This usually happens when an order is filled immediately against an existing bid or ask.

Market orders are generally taker orders. Limit orders can be either maker or taker:

- A limit order that sits on the order book and is filled later is usually treated as a maker order.
- A limit order that matches an existing order immediately is treated as a taker order.
- The order type alone does not guarantee a maker fee.

This distinction matters because the fee is based on how the order actually executes, not simply on whether you clicked “market” or “limit.” OKX explains that a single order can also be filled in multiple parts, with each fill charged according to its execution type.

### A simple example

Suppose you buy $2,000 of BTC on the standard spot tier.

At a 0.0800% maker fee:

text
$2,000 × 0.0008 = $1.60


At a 0.1000% taker fee:

text
$2,000 × 0.0010 = $2.00


The difference on one trade is only $0.40. Over hundreds of trades, however, small differences become much more noticeable. This is why active traders pay close attention to execution type, fee tier and spread rather than looking only at the headline commission.

## OKX spot trading fees

Spot trading is the most straightforward place to start. You buy or sell an asset directly, and the trading fee is calculated against the filled amount.

The standard public spot schedule currently ranges from the Regular tier through VIP 9. The exact rate can vary by trading pair group and jurisdiction, so the following table should be used as a public reference rather than a guarantee for every pair.

### Current public spot fee tiers

| Tier | Asset balance requirement or 30-day spot volume | Maker fee | Taker fee |
| --- | ---: | ---: | ---: |
| Regular | Under $100,000 or under $1 million volume | 0.0800% | 0.1000% |
| VIP 1 | At least $100,000 or at least $1 million volume | 0.0675% | 0.0800% |
| VIP 2 | At least $200,000 or at least $5 million volume | 0.0600% | 0.0700% |
| VIP 3 | At least $2 million or at least $10 million volume | 0.0550% | 0.0650% |
| VIP 4 | At least $5 million or at least $20 million volume | 0.0300% | 0.0450% |
| VIP 5 | At least $20 million or at least $100 million volume | 0.0250% | 0.0350% |
| VIP 6 | At least $50 million or at least $200 million volume | 0.0000% | 0.0300% |
| VIP 7 | At least $100 million or at least $500 million volume | -0.0020% | 0.0250% |
| VIP 8 | At least $250 million or at least $1 billion volume | -0.0050% | 0.0200% |
| VIP 9 | At least $500 million or at least $5 billion volume | -0.0050% | 0.0150% |

The thresholds are based on either account assets or trading volume, depending on the tier rules. Spot volume is assessed separately from futures volume. The VIP level is reviewed daily rather than changing instantly at the moment a threshold is reached.

For most casual users, the Regular tier is the relevant starting point. VIP 1 may become relevant to users who maintain substantial assets or trade around $1 million in spot volume over 30 days. VIP 4 and above are mainly designed for professional, institutional or very active traders.

## OKX futures fees

Futures fees are calculated on the value of the filled position, not simply on the margin posted.

Using 10x leverage does not automatically multiply the trading fee rate by ten. However, leverage allows you to control a larger position with less margin, so the dollar value of the fee can still be large compared with the capital committed.

### Current public futures fee tiers

| Tier | Asset balance requirement or 30-day futures volume | Maker fee | Taker fee |
| --- | ---: | ---: | ---: |
| Regular | Under $100,000 or under $5 million volume | 0.0200% | 0.0500% |
| VIP 1 | At least $100,000 or at least $5 million volume | 0.0160% | 0.0450% |
| VIP 2 | At least $200,000 or at least $10 million volume | 0.0150% | 0.0360% |
| VIP 3 | At least $2 million or at least $50 million volume | 0.0100% | 0.0280% |
| VIP 4 | At least $5 million or at least $200 million volume | 0.0080% | 0.0270% |
| VIP 5 | At least $20 million or at least $600 million volume | 0.0050% | 0.0260% |
| VIP 6 | At least $50 million or at least $1 billion volume | 0.0000% | 0.0250% |
| VIP 7 | At least $100 million or at least $1.5 billion volume | -0.0020% | 0.0200% |
| VIP 8 | At least $250 million or at least $2 billion volume | -0.0050% | 0.0200% |
| VIP 9 | At least $500 million or at least $20 billion volume | -0.0050% | 0.0150% |

A futures position usually creates at least two trading events: opening and closing. If both sides are taker executions, both sides can receive the taker rate. That makes the difference between maker and taker execution more important for frequent futures traders.

Futures traders should also separate three different costs:

1. **Opening trading fee**
2. **Closing trading fee**
3. **Funding fee**

Funding is exchanged between long and short traders and is not the same as an OKX trading commission. Depending on the funding rate, longs may pay shorts or shorts may pay longs. The rate and settlement schedule vary by contract.

## Does OKX charge deposit and withdrawal fees?

Crypto deposits into OKX do not normally carry an OKX deposit fee. The asset still has to be sent over a supported network, so the sending wallet or originating platform may charge its own withdrawal or network fee.

Crypto withdrawals from OKX do carry a fee. The amount depends on the asset, network, transaction conditions and the fee currently displayed on the withdrawal page. Fees for networks such as ERC-20, TRC-20 and BEP-20 may differ, and network congestion can affect the amount shown.

The withdrawal fee is generally charged once per withdrawal transaction rather than as a simple percentage of the amount withdrawn. A small withdrawal can therefore be disproportionately expensive. For example, withdrawing $20 worth of an asset with a $2 network fee is very different from withdrawing $2,000 with the same fee.

OKX states that the withdrawal amount should be checked on the specific withdrawal page because network fees can change and may not exactly match the underlying on-chain gas cost.

### Practical ways to reduce withdrawal costs

- Compare supported networks before confirming the withdrawal.
- Avoid sending a small amount when the fixed network fee is high.
- Check that the receiving wallet supports the selected network.
- Do not choose a cheaper-looking network unless the destination accepts it.
- Review the final “amount received” field before submitting.

A low withdrawal fee is not useful if the wrong network is selected. Crypto transfers are generally difficult or impossible to reverse.

## Are OKX Convert and Buy/Sell fees the same as trading fees?

No.

Order-book trading displays maker and taker fees separately. OKX’s Convert and express Buy/Sell flows may instead show one quoted price without presenting a separate trading commission.

That does not necessarily mean the transaction is free. The cost can be incorporated into the quoted price or spread. The price offered to buy an asset and the price offered to sell the same asset at the same moment may differ because of spread, liquidity and conversion pricing.

For a small, occasional conversion, convenience may matter more than the difference. For larger trades or frequent transactions, compare the final amount received through Convert with the result of placing an order on the spot order book.

OKX describes Convert as a separate route from order-book trading and notes that its quoted price includes the relevant spread rather than showing the standard maker-taker fee line.

## Does OKX charge account or inactivity fees?

OKX’s trading fee FAQ states that it does not charge a fee for opening an account or keeping an account open. Holding spot assets without placing a trade also does not create a daily spot trading fee.

The important exception is derivatives funding. A perpetual futures position can incur funding at scheduled settlement times even though funding is not classified as a spot trading fee.

Other services may have their own pricing or transaction conditions. Before using card purchases, fiat payment methods, margin borrowing, options, copy trading or third-party payment services, check the cost shown on that specific product screen.

## How to reduce OKX fees

### Use limit orders carefully

A limit order can receive the lower maker rate when it rests on the order book. It can still receive the taker rate if it executes immediately.

Do not place a limit order solely because the button says “limit.” Check whether the order is likely to match immediately and review the fee shown in the order panel.

### Avoid unnecessary market orders

Market orders are convenient, but they generally pay the taker rate and can experience slippage when the order book is thin or the market moves quickly.

For liquid pairs and ordinary-sized trades, the difference may be manageable. For larger trades, splitting an order or using a price-controlled limit order may reduce execution costs, although it introduces the risk that the order will not fill.

### Check your actual account tier

Logged-out fee pages may show reference rates that do not match your account. OKX advises users to sign in and check **Assets > My trading fees** on the web interface, or the trading fee tier section in the app.

The fee displayed on the order placement panel for the specific pair is more useful than a general fee table because it reflects the instrument and account tier you are actually using.

### Consider VIP eligibility realistically

OKX’s VIP program uses asset balances and 30-day trading volume. The platform reviews tiers daily, and users may also be able to apply for a status match by submitting proof of assets or trading volume from another exchange.

For an occasional buyer, deliberately increasing trading volume to reach VIP status usually makes little economic sense. The trading activity required for the higher levels is substantial. VIP pricing becomes more relevant when a trader already has high volume and is comparing execution costs across platforms.

### Do not assume OKB reduces trading fees

OKX’s current help documentation says that holding OKB does not offset exchange trading fees or automatically reduce the fee tier. This is an easy assumption to make if you have seen token-based discounts on other exchanges, but it should not be treated as an OKX rule.

## Is OKX cheap for crypto trading?

For the standard public spot schedule, OKX lists a 0.0800% maker fee and 0.1000% taker fee at the Regular level. Its standard futures schedule lists a 0.0200% maker fee and 0.0500% taker fee.

Whether that is cheap for you depends on how you trade.

OKX may make sense when:

- You mostly use the order book rather than instant conversion.
- You trade enough volume for maker-taker differences to matter.
- You use limit orders that genuinely add liquidity.
- You compare withdrawal costs before moving assets.
- You check the exact fee for the pair and region you use.
- You trade products supported by the platform and understand their additional costs.

The headline rate is less useful if the spread on a small market is wide, the withdrawal fee is high, or a limit order repeatedly executes as a taker.

## What is the OKX referral code CASH20?

The supplied referral link uses the invitation code **CASH20**. It is intended for users who want to create an OKX account through the referral route and check whether the applicable referral or fee-rebate offer is available in their region.

The supplied promotion is described as offering a **20% rebate**, but referral benefits can depend on jurisdiction, account status, campaign conditions and whether the user is new or already registered. The final terms shown during signup should take priority.

[👉 Check OKX fees and sign up with the CASH20 referral link](https://okx.com/join/CASH20)

Do not assume that entering a referral code changes the published maker or taker table for every product. It is better to confirm the actual fee shown inside the account after registration and before placing a trade.

## How to check the fee before trading

Before submitting an order, use this checklist:

1. Select the exact trading pair.
2. Confirm whether you are trading spot, margin, futures or another product.
3. Check the maker and taker rates in the order panel.
4. Review the estimated fee amount.
5. Check the expected receive amount after fees.
6. For futures, review the contract size and funding information.
7. For withdrawals, confirm the network and final amount received.
8. After execution, open the order details to verify the actual fee.

The fee shown before trading is an estimate based on the displayed rate and order conditions. A partially filled order may have multiple fills, and the final amount can differ from a quick calculation based on the first displayed market price.

## Bottom line

OKX fees are built around a tiered maker-taker system rather than one flat commission.

For standard spot trading, the public reference rates currently start at **0.0800% maker** and **0.1000% taker**. For standard futures trading, they start at **0.0200% maker** and **0.0500% taker**. Higher VIP tiers offer lower rates, but the volume and asset requirements rise quickly.

The most important habits are simple:

- Check the fee for the exact pair.
- Know whether your order executed as maker or taker.
- Treat Convert pricing separately from order-book fees.
- Review withdrawal costs before sending funds.
- Remember that futures funding is separate from trading commission.
- Use the logged-in account fee schedule as the final reference.

[👉 View the current OKX trading interface and review your applicable fee tier](https://okx.com/join/CASH20)
