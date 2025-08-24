# Kuprum's Audits

I am `kuprum`, an experienced Web3 security researcher with main areas of expertise being L1 (EVM & Cosmos SDK chains), cross-chain communication (IBC / Bridges), complex infrastructure projects. Currently an independent security researcher. Previously worked at various companies, including being a Lead auditor in a Web3 security company, also have experience in Web2 security, secirity architectures, testing, and verification.

Like copper (Cuprum in Latin) — probably the most versatile, essential, and reliable metal we have today — I am going to bring a lot for the success and security of your project. In my audits I deliver you the _highest quiality work_, and also tend to find severe but hard/rare bugs that most others miss. I strive to both understand the broadest context of a project, it's security architecture and assumptions, and to go to the deepest bit level to find where the security assumptions may be violated. Please feel free to browse my portfolio below, and also at [audits.sherlock.xyz/watson/kuprum](https://audits.sherlock.xyz/watson/kuprum) or [cantina.xyz/u/kuprum](https://cantina.xyz/u/kuprum). 

To book a solo audit with me send a DM via [x/kuprumxyz](https://x.com/kuprumxyz) or [t.me/kuprumxyz](https://t.me/kuprumxyz). You can also engage me for a team audit via [Sherlock](https://sherlock.xyz), the leading security provider, with whom I am closely collaborating.

## Audit porfolio

<table>
  <thead>
    <tr>
      <th>Begin / Duration</th>
      <th>Project</th>
      <th>Category</th>
      <th>Language / Framework</th>
      <th>Provider</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>2025-05 / 5&nbsp;weeks</td>
      <td><a href="https://github.com/cosmos/evm/blob/main/docs/audits/sherlock_2025_07_28_final.pdf">Cosmos EVM audit</a></td>
      <td>Cosmos L1, Cross-chain</td>
      <td>Cosmos SDK / EVM / Go / Solidity</td>
      <td>Sherlock</td>
    </tr>
    <tr>
      <td colspan=5>
        <details>
          <summary>Notable findings</summary>
          <ul>
            <li>Dynamic precompiles may be weaponized to halt Cosmos EVM</li>
            <li>Internal EVM calls from Cosmos transactions can be abused to steal gas or halt Cosmos EVM</li>
            <li>Conversion errors on processing IBC acks / timeouts for native ERC20 coins break IBC packet lifecycle</li>
          </ul>
        </details>
      </td>
    </tr>
    <tr>
      <td>2025-03 / 2&nbsp;weeks</td>
      <td>Lombard IBC V2 Integration audit</td>
      <td>Cosmos L1, Cross-chain, Bitcoin staking</td>
      <td>Cosmos SDK / CosmWasm / Go / Rust / Solidity</td>
      <td>Sherlock</td>
    </tr>
    <tr>
      <td colspan=5>
        The report is not yet public
      </td>
    </tr>
    <tr>
      <td>2025-02 / 3&nbsp;weeks</td>
      <td><a href="https://github.com/cosmos/ibc-go/blob/main/docs/audits/IBC-v2/IBC-v2-April-2025-Collaborative-Audit-Report.pdf">IBC V2 (Eureka) audit</a></td>
      <td>Cross-chain</td>
      <td>Cosmos SDK / Go / Solidity</td>
      <td>Sherlock</td>
    </tr>
    <tr>
      <td colspan=5>
        <details>
          <summary>Notable findings</summary>
          <ul>
            <li><code>ICS26Router::recvPacket</code> can be DoSed via gas griefing attack, resulting in IBC unreliability</li>
            <li>Malicious ERC-20 contracts may fail acks/timeouts, forcing relayers to lose funds</li>
          </ul>
        </details>
      </td>
    </tr>
    <tr>
      <td>2024-12 / 4&nbsp;weeks</td>
      <td>14th in <a href="https://cantina.xyz/competitions/0561defa-eeb2-4a74-8884-5d7a873afa58/leaderboard">Story Protocol competition</a></td>
      <td>Cosmos/Geth L1, BFT Consensus</td>
      <td>Cosmos SDK / EVM / Go / Solidity</td>
      <td>Cantina</td>
    </tr>
    <tr>
      <td colspan=5>
        <details>
          <summary>Notable findings</summary>
          <ul>
            <li><a href="https://cantina.xyz/code/0561defa-eeb2-4a74-8884-5d7a873afa58/findings/782">Computing rewards shares with banker's rounding during undelegation will lead to permanent delegations freeze</a></li>
            <li><a href="https://cantina.xyz/code/0561defa-eeb2-4a74-8884-5d7a873afa58/findings/31">Genesis validators may get slashed/jailed right after Singularity</a></li>
          </ul>
        </details>
      </td>
    </tr>
    <tr>
      <td>2024-10 / 3&nbsp;weeks</td>
      <td>5th in <a href="https://cantina.xyz/competitions/d139882b-2d3a-49ac-9849-9dccef584090/leaderboard">Omni Network competition</a></td>
      <td>Cosmos/Geth L1, BFT Consensus</td>
      <td>Cosmos SDK / EVM / Go / Solidity</td>
      <td>Cantina</td>
    </tr>
    <tr>
      <td colspan=5>
        <details>
          <summary>Notable findings</summary>
          <ul>
            <li><a href="https://cantina.xyz/code/d139882b-2d3a-49ac-9849-9dccef584090/findings/607">Omni chain halt via post-quorum votes poisoning</a></li>
            <li><a href="https://cantina.xyz/code/d139882b-2d3a-49ac-9849-9dccef584090/findings/713"><code>FinalizeBlock</code> is non-deterministic; will lead to consensus failures</a></li>
          </ul>
        </details>
      </td>
    </tr>
    <tr>
      <td>2024-10 / 1&nbsp;week</td>
      <td>🥈in <a href="https://audits.sherlock.xyz/contests/561?filter=results">Predict.Fun contest</a></td>
      <td>Lending, Prediction market</td>
      <td>Solidity</td>
      <td>Sherlock</td>
    </tr>
    <tr>
      <td colspan=5>
        <details>
          <summary>Notable findings</summary>
          <ul>
            <li><a href="https://github.com/sherlock-audit/2024-09-predict-fun-judging/issues/119">Using wrong format of <code>questionId</code> for <code>NegRiskCtfAdapter</code> leads to loan operations on resolved multi-outcome markets</a></li>
          </ul>
        </details>
      </td>
    </tr>
    <tr>
      <td>2024-09 / 2&nbsp;weeks</td>
      <td>🥇in <a href="https://audits.sherlock.xyz/contests/468?filter=results">Flayer contest</a></td>
      <td>NFTs, Uniswap V4</td>
      <td>Solidity</td>
      <td>Sherlock</td>
    </tr>
    <tr>
      <td colspan=5>
        <details>
          <summary>Notable findings</summary>
          <ul>
            <li><a href="https://github.com/sherlock-audit/2024-08-flayer-judging/issues/117">Frequency-dependent <code>TaxCalculator.sol::calculateCompoundedFactor</code> leads to interest loss either for users or for protocol</a></li>
            <li><a href="https://github.com/sherlock-audit/2024-08-flayer-judging/issues/173">Stale shutdown params can be reused to drain all funds from <code>CollectionShutdown</code> contract</a></li>
          </ul>
        </details>
      </td>
    </tr>
    <tr>
      <td>2024-08 / 2&nbsp;weeks</td>
      <td>🥉in <a href="https://code4rena.com/audits/2024-08-phi">Phi competition</a></td>
      <td>Cross-chain, Identity management</td>
      <td>Solidity</td>
      <td>Code4rena</td>
    </tr>
    <tr>
      <td colspan=5>
        <details>
          <summary>Notable findings</summary>
          <ul>
            <li><a href="https://github.com/code-423n4/2024-08-phi-findings/issues/254">Signature replay in <code>signatureClaim</code> results in unauthorized claiming of rewards</a></li>
            <li><a href="https://github.com/code-423n4/2024-08-phi-findings/issues/282">DoS in <code>CuratorRewardsDistributor</code> due to accumulation of curators with 0 shares in <code>Cred</code></a></li>
          </ul>
        </details>
      </td>
    </tr>
    <tr>
      <td>2024-08 / 0.5&nbsp;weeks</td>
      <td>4th in <a href="https://audits.sherlock.xyz/contests/516?filter=results">Winnables Raffles contest</a></td>
      <td>Cross-chain</td>
      <td>Solidity / Chainlink VRF & CCIP</td>
      <td>Sherlock</td>
    </tr>
    <tr>
      <td colspan=5>
        <details>
          <summary>Notable findings</summary>
          <ul>
            <li><a href="https://github.com/sherlock-audit/2024-08-winnables-raffles-judging/issues/413">Won prizes may get permanently locked due to out-of-gas reverts</a></li>
          </ul>
        </details>
      </td>
    </tr>
    <tr>
      <td>2024-07 / 2&nbsp;weeks</td>
      <td>8th in <a href="https://code4rena.com/audits/2024-07-optimism-superchain">Optimism Superchain competition</a></td>
      <td>L1/L2, Cross-chain, Dispute games</td>
      <td>Optimism / Solidity</td>
      <td>Code4rena</td>
    </tr>
    <tr>
      <td colspan=5>
        <details>
          <summary>Notable findings</summary>
          <ul>
            <li><a href="https://github.com/code-423n4/2024-07-optimism-findings/issues/13">An attacker can bypass the challenge period during LPP finalization</a></li>
            <li><a href="https://github.com/code-423n4/2024-07-optimism-findings/issues/27">LPP metadata can be altered after the challenge period is over, allowing incorrect states to be proven</a></li>
          </ul>
        </details>
      </td>
    </tr>
    <tr>
      <td>2024-03 / 0.5&nbsp;weeks</td>
      <td>🥉 in <a href="https://audits.sherlock.xyz/contests/191?filter=results">RadicalxChange contest</a></td>
      <td>Auctions</td>
      <td>Solidity</td>
      <td>Sherlock</td>
    </tr>
    <tr>
      <td colspan=5>
        <details>
          <summary>Notable findings</summary>
          <ul>
            <li><a href="https://github.com/sherlock-audit/2024-02-radicalxchange-judging/issues/41"><code>_cancelAllBids</code> allows to cancel the highest bid; can be exploited to steal all contract funds</a></li>
          </ul>
        </details>
      </td>
    </tr>
    <tr>
      <td>2024-02 / 2&nbsp;weeks</td>
      <td>🥇 in <a href="https://code4rena.com/audits/2024-02-unistaker-infrastructure">UniStaker Infrastructure competition</a> (team CodeWasp)</td>
      <td>Staking, Governance</td>
      <td>Solidity</td>
      <td>Code4rena</td>
    </tr>
    <tr>
      <td colspan=5>
        <details>
          <summary>Notable findings</summary>
          <ul>
            <li><a href="https://github.com/code-423n4/2024-02-uniswap-foundation-findings/blob/main/data/CodeWasp-Q.md">Adapting UniStaker test infrastructure to UNI token</a></li>
          </ul>
        </details>
      </td>
    </tr>
  </tbody>
</table>

Before that I've done dozens of audits as a Lead Auditor in a Web3 security company with the main focus on Cosmos SDK / IBC / Cross-chain / CosmWasm / Solidity.

More before that I've done a PhD in formal verification, and worked at various companies as a developer.

## Judging experience

I've had a single judging experience so far, namely judging the [Mightly competition](https://cantina.xyz/competitions/616d8bb4-16ce-4ca9-9ce9-5b99d6e146ef) at Cantina. 
It was a challenge in many respects: many findings (1344), many AI-generated submissions, and difficulties of communications with the sponsor, to name a few. 
I am very proud that together with my fellow judge [Jiri123](https://cantina.xyz/u/Jiri123) we've been able to judge it with record-breaking speed, efficiency, 
and communication transparency. 
Our judging has attracted numerous praise from fellow SRs, see e.g. [this](https://x.com/Ril11111/status/1932805270822137964) 
and [this](https://x.com/0xhammadghazi/status/1927356751818436648) posts on X, and also the below screenshots from Discord:

<details>
        <summary>Screenhot 1 (click to show)</summary>
        <img src="https://raw.githubusercontent.com/kuprumxyz/audits/main/judging/Mighty-Judging-Praise1.png"/>
</details>

<details>
        <summary>Screenhot 2 (click to show)</summary>
        <img src="https://raw.githubusercontent.com/kuprumxyz/audits/main/judging/Mighty-Judging-Praise2.png"/> 
</details>

