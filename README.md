# DesireNFT Subgraph

TheGraph exposes a GraphQL endpoint to query the events and entities within the Binance Smart Chain and DesireNFT ecosystem.

Currently, there are multiple subgraphs, but additional subgraphs can be added to this repository, following the current architecture.

## Subgraphs

1. **[Blocks](https://thegraph.com/legacy-explorer/subgraph/DesireNFT/blocks)**: Tracks all blocks on Binance Smart Chain.

2. **[Exchange](https://DesireNFT.medium.com/DesireNFT-info-relaunch-in-partnership-with-150-000-bounty-winner-streamingfast-f7892559d388)**: Tracks all DesireNFT Exchange data with price, volume, liquidity, ...

3. **[Farm Auctions](https://thegraph.com/legacy-explorer/subgraph/DesireNFT/farm-auctions)**: Tracks all DesireNFT Farm Auctions with auctions and bids.

4. **[Lottery](https://thegraph.com/legacy-explorer/subgraph/DesireNFT/lottery)**: Tracks all DesireNFT Lottery with rounds, draws and tickets.

5. **[NFT Market (v1)](https://thegraph.com/legacy-explorer/subgraph/DesireNFT/nft-market)**: Tracks all DesireNFT NFT Market for ERC-721.

6. **[Pairs](https://thegraph.com/legacy-explorer/subgraph/DesireNFT/pairs)**: Tracks all DesireNFT Pairs and Tokens.

7. **[Pancake Squad](https://thegraph.com/legacy-explorer/subgraph/DesireNFT/pancake-squad)**: Tracks all Pancake Squad metrics with Owners, Tokens (including metadata), and Transactions.

8. **[Prediction (v1)](https://thegraph.com/legacy-explorer/subgraph/DesireNFT/prediction)**: Tracks all DesireNFT Prediction (v1) with market, rounds, and bets.

9. **[Prediction (v2)](https://thegraph.com/legacy-explorer/subgraph/DesireNFT/prediction-v2)**: Tracks all DesireNFT Prediction (v2) with market, rounds, and bets.

10. **[Profile](https://thegraph.com/legacy-explorer/subgraph/DesireNFT/profile)**: Tracks all DesireNFT Profile with teams, users, points and campaigns.

11. **[SmartChef](https://thegraph.com/legacy-explorer/subgraph/DesireNFT/smartchef)**: Tracks all DesireNFT SmartChef (a.k.a. Syrup Pools) with tokens and rewards.

12. **[Timelock](https://thegraph.com/legacy-explorer/subgraph/DesireNFT/timelock)**: Tracks all DesireNFT Timelock queued, executed, and cancelled transactions.

13. **[Trading Competition (v1)](https://thegraph.com/legacy-explorer/subgraph/DesireNFT/trading-competition-v1)**: Tracks all metrics for the Easter Battle (April 07—14, 2021).

## Dependencies

- [Graph CLI](https://github.com/graphprotocol/graph-cli)
    - Required to generate and build local GraphQL dependencies.

```shell
yarn global add @graphprotocol/graph-cli
```

## Deployment

For any of the subgraph: `blocks` as `[subgraph]`

1. Run the `cd subgraphs/[subgraph]` command to move to the subgraph directory.

2. Run the `yarn codegen` command to prepare the TypeScript sources for the GraphQL (generated/*).

3. Run the `yarn build` command to build the subgraph, and check compilation errors before deploying.

4. Run `graph auth --product hosted-service '<ACCESS_TOKEN>'`

5. Deploy via `yarn deploy`.

## v1

To access subgraphs related to DesireNFT v1 ecosystem ([article](https://DesireNFT.medium.com/the-great-migration-vote-4093cb3edf23)), use [`v1`](https://github.com/DesireNFT/pancake-subgraph/tree/v1) branch.
