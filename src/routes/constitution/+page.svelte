<script>
    import { dues } from '$lib/utils/helper';
    let one, oneOne, oneTwo, oneThree, oneFour;
    let two, twoOne, twoTwo, twoThree;
    let three, threeOne, threeTwo, threeThree, threeFour;
    let four, fourOne, fourTwo, fourThree, fourFour, fourFive;
    let five, fiveOne, fiveOneOne, fiveOneTwo, fiveTwo;
    let six, sixOne, sixTwo, sixThree, sixFour;
    let seven, sevenOne, sevenTwo, sevenThree, sevenFour, sevenFive;

    const goToSection = (section) => {
        const top = section.getBoundingClientRect().top + window.pageYOffset;
        window.scrollTo({left: 0, top, behavior: 'smooth'});
    }
</script>

<style>
    .constitution {
        position: relative;
        z-index: 1;
        width: 92%;
        max-width: 800px;
        margin: 8em auto 10em;
    }

    h1 {
        font-size: 2em;
        line-height: 1.2em;
        text-align: center;
        margin: 2em 0 1.5em;
    }

    h2 {
        font-size: 1.5em;
        line-height: 1.2em;
    }

    h3 {
        text-decoration: underline;
        font-size: 1.3em;
        line-height: 1.2em;
    }

    h4 {
        text-decoration: underline;
        margin-left: 2em;
        font-size: 1.2em;
        line-height: 1.2em;
    }

    h5 {
        margin-left: 6em;
        font-size: 0.8em;
        line-height: 1.1em;
    }

    .subBlock {
        margin-left: 2.4em;
    }

    .sectionHeading {
        margin: 4em 0 1.5em;
    }

    .subSectionHeading {
        margin: 1.5em 0 1.5em;
    }

    .underscore {
        text-decoration: underline;
    }

    .right {
        text-align: right;
    }

    .positionMaximums td {
        min-width: 3em;
    }

    .noUnderscore {
        text-decoration: none;
    }

    .clickable {
        cursor: pointer;
    }

    .clickable:hover {
        color: #00316b;
    }

    p {
        color: #777;
    }
</style>

<div class="constitution">
    <h1 class="noUnderscore">LEAGUE CONSTITUTION</h1>
    
    <h2 class="noUnderscore">TABLE OF CONTENTS</h2>
    
    <h3 class="noUnderscore clickable" on:click={() => goToSection(one)}>Section 1: General Information</h3>
        <h4 class="noUnderscore clickable" on:click={() => goToSection(oneOne)}>1.1 - Changes for 2024</h4>
            <!-- <h5 class="noUnderscore clickable" on:click={() => goToSection(oneOneOne)}>1.1.1 Position Maximums</h5> -->
        <h4 class="noUnderscore clickable" on:click={() => goToSection(oneTwo)}>1.2 - Fantasy Platform</h4>
            <!-- <h5 class="noUnderscore clickable" on:click={() => goToSection(oneTwoOne)}>1.2.1 Trade Collusion</h5>
            <h5 class="noUnderscore clickable" on:click={() => goToSection(oneTwoTwo)}>1.2.2 Lending Players Prohibition</h5>
            <h5 class="noUnderscore clickable" on:click={() => goToSection(oneTwoThree)}>1.2.3 Trade Deadline</h5>
            <h5 class="noUnderscore clickable" on:click={() => goToSection(oneTwoFour)}>1.2.4 Trade Restrictions</h5>
            <h5 class="noUnderscore clickable" on:click={() => goToSection(oneTwoFive)}>1.2.5 Veto/Trade Process</h5> -->
        <h4 class="noUnderscore clickable" on:click={() => goToSection(oneThree)}>1.3 - League Fees</h4>
	<h4 class="noUnderscore clickable" on:click={() => goToSection(oneFour)}>1.4 - League Payout</h4>
    
    <h3 class="noUnderscore clickable" on:click={() => goToSection(two)}>Section 2: Rosters</h3>
    
        <h4 class="noUnderscore clickable" on:click={() => goToSection(twoOne)}>2.1 - Starters</h4>
        <h4 class="noUnderscore clickable" on:click={() => goToSection(twoTwo)}>2.2 - Bench</h4>
        <h4 class="noUnderscore clickable" on:click={() => goToSection(twoThree)}>2.3 - Injured Reserved</h4>
    
    <h3 class="noUnderscore clickable" on:click={() => goToSection(three)}>Section 3: Draft Rules</h3>
    
        <h4 class="noUnderscore clickable" on:click={() => goToSection(threeOne)}>3.1 - Draft Type</h4>
	<h4 class="noUnderscore clickable" on:click={() => goToSection(threeTwo)}>3.2 - Draft Lottery (Draft Order)</h4>
	<h4 class="noUnderscore clickable" on:click={() => goToSection(threeThree)}>3.3 - League Divisions</h4>
	<h4 class="noUnderscore clickable" on:click={() => goToSection(threeFour)}>3.4 - Consolation Pick</h4>
    
    <h3 class="noUnderscore clickable" on:click={() => goToSection(four)}>Section 4: Scoring</h3>
    
        <h4 class="noUnderscore clickable" on:click={() => goToSection(fourOne)}>4.1 - Passing</h4>
        <h4 class="noUnderscore clickable" on:click={() => goToSection(fourTwo)}>4.2 - Rushing</h4>
	<h4 class="noUnderscore clickable" on:click={() => goToSection(fourThree)}>4.3 - Receiving</h4>
	<h4 class="noUnderscore clickable" on:click={() => goToSection(fourFour)}>4.4 - Kicking</h4>
	<h4 class="noUnderscore clickable" on:click={() => goToSection(fourFive)}>4.5 - Defensive</h4>

    <h3 class="noUnderscore clickable" on:click={() => goToSection(five)}>Section 5: Transactions</h3>
        <h4 class="noUnderscore clickable" on:click={() => goToSection(fiveOne)}>5.1 - Waivers</h4>
	    <h5 class="noUnderscore clickable" on:click={() => goToSection(fiveOneOne)}>5.1.1 - FAAB (Free Agent Acquisition Budget)</h5>
            <h5 class="noUnderscore clickable" on:click={() => goToSection(fiveOneTwo)}>5.1.2 - Waiver Schedule</h5>
	<h4 class="noUnderscore clickable" on:click={() => goToSection(fiveTwo)}>5.2 - Trades</h4>

    <h3 class="noUnderscore clickable" on:click={() => goToSection(six)}>Section 6: Playoffs</h3>
    
        <h4 class="noUnderscore clickable" on:click={() => goToSection(sixOne)}>6.1 - 8-team League</h4>
	<h4 class="noUnderscore clickable" on:click={() => goToSection(sixTwo)}>6.2 - 10-team League</h4>
	<h4 class="noUnderscore clickable" on:click={() => goToSection(sixThree)}>6.3 - 12-team League</h4>
	<h4 class="noUnderscore clickable" on:click={() => goToSection(sixFour)}>6.4 - 14-team League</h4>
	    	<!--<h5 class="noUnderscore clickable" on:click={() => goToSection(sixOneOne)}>6.1.1 - 8-team League</h5>
            	<h5 class="noUnderscore clickable" on:click={() => goToSection(sixOneTwo)}>6.1.2 - 10-team League</h5>
		<h5 class="noUnderscore clickable" on:click={() => goToSection(sixOneThree)}>6.1.3 - 12-team League</h5>
		<h5 class="noUnderscore clickable" on:click={() => goToSection(sixOneFour)}>6.1.4 - 14-team League</h5> -->
        <!-- <h4 class="noUnderscore clickable" on:click={() => goToSection(sixTwo)}>6.2 Replacing Managers</h4>
        <h4 class="noUnderscore clickable" on:click={() => goToSection(sixThree)}>6.3 Replacement Incentive</h4> -->

    <h3 class="noUnderscore clickable" on:click={() => goToSection(seven)}>Section 7: Keepers</h3>
    
        <h4 class="noUnderscore clickable" on:click={() => goToSection(sevenOne)}>7.1 - Changes for 2024</h4>
        <h4 class="noUnderscore clickable" on:click={() => goToSection(sevenTwo)}>7.2 - Drafted Players</h4>
        <h4 class="noUnderscore clickable" on:click={() => goToSection(sevenThree)}>7.3 - Undrafted Players</h4>
	<h4 class="noUnderscore clickable" on:click={() => goToSection(sevenFour)}>7.4 - Trading Keepers</h4>
	<h4 class="noUnderscore clickable" on:click={() => goToSection(sevenFive)}>7.5 - Keeper Scenarios</h4>
    
    
    <hr />
    
    <h2 class="sectionHeading" bind:this={one}>Section 1: General Information</h2>
    
    <h3 class="subSectionHeading" bind:this={oneOne}>1.1 - Changes for 2024</h3>
    
    <!-- <p>28 Total Players</p>
    
    <p class="underscore">Starters</p> -->
	
    <ul>
	<li>Draft pick trading is limited to the period between the draft pick lottery and the end of the draft. The draft picks involved must be for the draft that year.</li>
	<li>Several changes to scoring this year. See class="noUnderscore clickable" on:click={() => goToSection(four)}>"Section 4: Scoring" for details.</li>
	<li></li>
    </ul>
    
    <!-- <p>18 Bench (Expanded by 5 between the keague draft and start of regular season)</p>

    <p>1 IR Spots (Player must be labeled as IR, Out, or Covid in the Sleeper App)</p>
    
        <h4 bind:this={oneOneOne}>1.1.1 Position Maximums</h4>
        
        <div class="subBlock">
            <table class="positionMaximums">
                <tr><td>QB</td><td class="right">3 active, 5 total</td></tr>
                <tr><td>RB</td><td class="right">20</td></tr>
                <tr><td>WR</td><td class="right">20</td></tr>
                <tr><td>TE</td><td class="right">10</td></tr>
                <tr><td>D/ST</td><td class="right">3</td></tr>
                <tr><td>K</td><td class="right">3</td></tr>
            </table>
        </div> -->


    <h3 class="subSectionHeading" bind:this={oneTwo}>1.2 - Fantasy Platform</h3>

    <p>We use the Sleeper fantasy football platform: <a href="https://sleeper.app">https://sleeper.app</a>. Sleeper has been around for a few years, and is built on a modern platform that allows for custom scoring, roster positions, keeper rules, etc. Sleeper has a web app, iOS, and Android app for real-time updates and notifications.</p>
        
    <!-- <p>Trading of players and draft picks (up to 3 drafts away) are allowed. Trades will process immediately and will be reversed if vetoed or under investigation for collusion. Tradable assets include players, draft picks, and FAAB $.</p>
    
    <h4 bind:this={oneTwoOne}>1.2.1 Trade Collusion</h4>
    <div class="subBlock">
        <p>If any owners are suspected of accepting bribes/offering bribes to enhance their/another owners team via trade, trading any assets other than fantasy players, draft picks, FAAB $, or otherwise found guilty of engaging in any form of collusion*, all parties involved in the trade will be susceptible to punishment. The punishments will go as followed:</p>
        
        <ul>
            <li>First Offense – Immediate reduction of FAAB budget by 80%</li>
            <li>Second Offense – Immediate freeze on all transaction types for the next 18 weeks of regular season and playoff fantasy football games, including trades and waiver wire bids</li>
            <li>Third Offense – A league meeting of all members not involved in any of the improper trades/activity in question will take place to discuss next steps.</li>
        </ul>

        <p>All trades that are found guilty of collusion, will be reversed/denied. If the trade had affected the outcome of previous games, the results of those games will be revised.  </p>

        <p>*Collusion includes the organizing of veto votes against an acceptable trade.</p>

        <p>The commissioner will err on the side of letting owners manage their teams the way they see fit. Any collusion will need to be clear. The commissioner reserves the right to step in and at the very least assess the thinking of any team involved in a heavily lop-sided trade. </p>
    </div>

    <h4 bind:this={oneTwoTwo}>1.2.2 Lending Players Prohibition</h4>
    <div class="subBlock">
        <p>Any player traded from a team may not be re-acquired via trade within 6 weeks of the original trade. Any teams involved in this behavior will be subject to the aforementioned collusion punishments.</p>
    </div>
    
    <h4 bind:this={oneTwoThree}>1.2.3 Trade Deadline</h4>
    <div class="subBlock">
        <p>The trade deadline will be set for the Saturday of the week 11 games of the NFL season.</p>
    </div>
    
    <h4 bind:this={oneTwoFour}>1.2.4 Trade Restrictions</h4>
    <div class="subBlock">
        <p>You will not be able to trade draft picks that are more than 3 drafts away. For example, during the 2021 season you cannot trade any picks in or after the 2025 draft. You may only trade FAAB $ from the current season.</p>
    </div>
    
    <h4 bind:this={oneTwoFive}>1.2.5 Veto/Trade Process</h4>
    <div class="subBlock">
        <p>A total of 7 veto votes are required to veto a trade. Vetoes are only appropriate in instances of collusion or an egregious mismatch of value (i.e. CMC for a backup kicker). Not liking a trade does not warrant a veto.</p>
    </div> -->
    
       
    <h3 bind:this={oneThree}>1.3 - League Fees</h3>
    
    <p>League fees are ${dues} every season. Fees are collected through <a href="https://www.leaguesafe.com/league/4044415">LeagueSafe</a> and are due the day of the draft pick lottery. The draft pick lottery is one week before the draft, which is held two Fridays before Labor Day weekend. All managers must be fully paid before the draft pick lottery will be performed.</p>
	
    <!-- <p>FAAB Waiver wire system. Each team will begin the season with $100. $0 bids are allowed. Bids will process Thursdays and Sundays at 9AM EST.</p>

    <p>FAAB budgets will reset each season in January.</p> -->
    
    <h3 bind:this={oneFour}>1.4 - League Payout</h3>
    
    <p>The league payout is structured as follows for a 12-team league:</p>
    <ul>
        <li>1st place: ${dues * 5.5}</li>
        <li>2nd place: ${dues * 3}</li>
        <li>3rd place: ${dues * 2}</li>
    	<li>4th place: ${dues}</li>
	<li>Side pot: ${dues * .5} (highest weekly point total for the entire season)</li>
    </ul>

    <p>The league payout is structured as follows for a 10-team league:</p>
    <ul>
        <li>1st place: ${dues * 5}</li>
        <li>2nd place: ${dues * 2.5}</li>
        <li>3rd place: ${dues * 1.5}</li>
    	<li>4th place: ${dues * .5}</li>
	<li>Side pot: ${dues * .5} (highest weekly point total for the entire season)</li>
    </ul>
    
    <h2 class="sectionHeading" bind:this={two}>Section 2: Drafting</h2>
    
    <h3 bind:this={twoOne}>2.1 - Starters</h3>
    <ul>
        <li>QB</li>
        <li>RB</li>
	<li>RB</li>
	<li>WR</li>
    	<li>WR</li>
    	<li>FLEX (RB/WR/TE)</li>
    	<li>FLEX (RB/WR/TE)</li>
	<li>K</li>
    	<li>DEF</li>
    </ul>
    <p>Note: There is no explicit starting TE position.</p>

    <h3 bind:this={twoTwo}>2.2 - Bench</h3>
    <p>There are six bench spots with no position limits.</p>
    
    <h3 bind:this={twoThree}>2.3 - Injured Reserved</h3>
    <p>There is one injured reserved spot. The following designations are allowed: OUT, Doubtful, IR, and COVID-19.</p>
    
    <h2 class="sectionHeading" bind:this={three}>Section 3: Draft Rules</h2>

    <h3 bind:this={threeOne}>3.1 - Draft Type</h3>
    <p>Traditional snake draft with 90 seconds per draft pick. The CPU will automatically draft a player (based on ADP) if the entire 90 seconds is exhausted and there is no player in the owner's draft queue.</p>

    <h3 bind:this={threeTwo}>3.2 - Draft Lottery (Draft Order)</h3>
    <p>A draft lottery will be held to determine the draft pick order. The draft lottery will not be held until all of the league fees are paid.</p>
	
    <p>Each owner/team will have one entry in the lottery with the exception of the winner of fifth place game the previous year, who will receive two entries. The owners who placed fifth through last the previous year, or are newcomers to the league, will have their entries placed in a bowl. 
	A entry will be selected at random from the bowl. The owner of the entry will have an opportunity to choose their draft position. If the owner cannot be reached, they will be given the highest draft position available.</p>

    <p>Once everyone from the first pool of owners is selected, the entries for owners/teams who finished first through fourth will be placed in the bowl and randomly chosen.</p>

    <h3 bind:this={threeThree}>3.3 - League Divisions</h3>
    <p>League divisions will be set according to the draft lottery pick order. A twelve-team league will have three divisions. The first four people selected will be in a division together, followed by the next four, and then the final four. An eight-team league will have one division. 
	    A ten-team league will have two divisions of five. A fourteen-team league, heaven forbid, will have two divisions of seven.</p>
	
    <h3 bind:this={threeFour}>3.4 - Consolation Pick</h3>
    <p>To give owners something to play for in the consolation bracket, the winner of the consolation bracket will be granted a very unique power for next year’s draft. The ability to move up or down one draft position once the draft order is determined.</p>
    
    <p>If the owner decides not to use this ability, they may trade it to another owner. The receiving owner may move up or down one draft position, but at a cost. 
	    The winner of the consolation bracket may select any player (excluding keepers) picked from rounds nine through fifteen to be traded to them from the owner who accepted the consolation pick. This trade must be accepted as long as the player traded back is at the same position.</p>
    
    <h2 class="sectionHeading" bind:this={four}>Section 4: Scoring System</h2>
    
    <h3 bind:this={fourOne}>4.1 - Passing</h3>
    <ul>
        <li>25 Passing Yards = 1 points</li>
	<li>Passing Touchdown = 6 points</li>
        <li>Interception = -3 points</li>
	<li>Interception Returned for a Touchdown = -3 additional points</li>
	<li>Passing Play of 40+ yards = .5 bonus points</li>
	<li>Passing Touchdown 40+ yards = .5 bonus points</li>
    	<li>25 Completions = 1 bonus point</li>
    	<li>300-399 Passing Yards = 1 bonus point</li>
    	<li>400+ Passing Yards = 2 bonus points (Note: This bonus scoring replaces the previous bonus of 300-399 Passing Yards. The player will receive a total of 2 points not 3 points.)</li>
    </ul>
    
    <h3 bind:this={fourTwo}>4.2 - Rushing</h3>
    <ul>
        <li>10 Rushing Yards = 1 point</li>
	<li>Rushing 1st Down = .25 points (Note: This replaces our scoring last season for Rushing Attempts. Rushing attempts are no longer scored as .1 points.)</li>
        <li>Rushing Play of 40+ yards = .5 bonus points</li>
	<li>Rushing Touchdown of 40+ yards = .5 bonus points</li>
    	<li>20 Carries = 2 bonus points</li>
    	<li>100-199 Rushing Yards = 1 bonus point</li>
    	<li>200+ Rushing Yards = 2 bonus points (Note: This bonus scoring replaces the previous bonus of 100-199 Rushing Yards. The player will receive a total of 2 points not 3 points.)</li>
    	<li>200+ Rushing and Receiving Yards Combined = 1 bonus point</li>
    </ul>
	
    <h3 bind:this={fourThree}>4.3 - Receiving</h3>
    <ul>
        <li>Half PPR (half point-per-reception)</li>
	<li>Reception = .5 points</li>
        <li>Receiving Play of 40+ yards = .5 bonus points</li>
	<li>Receiving Touchdown of 40+ yards = .5 bonus points</li>
    	<li>100-199 Receiving Yards = 1 bonus point</li>
    	<li>200+ Receiving Yards = 2 bonus points (Note: This bonus scoring replaces the previous bonus of 100-199 Receiving Yards. The player will receive a total of 2 points not 3 points.)</li>
    	<li>200+ Rushing and Receiving Yards Combined = 1 bonus point</li>
    </ul>

    <h3 bind:this={fourFour}>4.4 - Kicking</h3>
    <ul>
        <li>PAT = 1 point</li>
	<li>FG Made (18-49 yards) = 3 points (Note: 40-49 Yard FG Made is no longer scored as 4 points.)</li>
        <li>FG Made (50+ yards) = 5 points</li>
    	<li>FG Miss = -1 point</li>
    </ul>

    <h3 bind:this={fourFive}>4.5 - Defensive</h3>
    <p>Our defensive scoring is unique and is based on the actual performance of the defense: sacks, tackles for loss, passes defended, forced punts, etc.</p>

    <ul>
        <li>Sacks = .5 points</li>
	<li>Tackles for Loss = .25 points</li>
        <li>Passes Defended = .25 points</li>
	<li>Forced Punts = .5 points</li>
    	<li>3 and Out = .5 points</li>
	<li>4th Down Stop = 1 point</li>
	<li>Forced Fumble = 1 point</li>
    	<li>Fumble Recovery = 1 point</li>
    	<li>Blocked Kick = 2 points</li>
    	<li>Interception = 2 points</li>
	<li>Special Teams Touchdown = 6 points</li>
	<li>Safety = 4 points</li>
	<li>Points Allowed (21-27) = -1 point</li>
	<li>Points Allowed (28-34) = -2 points</li>
    	<li>Points Allowed (35+) = -3 points</li>
	<li>300-399 Total Yards Allowed = -1 point</li>
	<li>400-499 Total Yards Allowed = -2 points</li>
    	<li>500+ Total Yards Allowed = -3 points</li>
    </ul>

    <!-- <ol>
        <li>Points For</li>
        <li>Head 2 Head Record</li>
        <li>Division Record</li>
        <li>Total Points Against</li>
        <li>Coin Flip</li>
        <li>Duel to the death</li>
    </ol> -->

    <h2 class="sectionHeading" bind:this={five}>Section 5: Transactions</h2>
    
    <h3 bind:this={fiveOne}>5.1 - Waivers</h3>
    	<p>Waivers function off a combination of modified continuous waivers and blind-bid/free agent acquisition budget (FAAB) system. For more information: <a href="https://www.thefantasyfootballers.com/articles/league-needs-change-waiver-system-asap/">What is a FAAB waiver system?</a></p>
	
	<h4 bind:this={fiveOneOne}>5.1.1 - FAAB (Free Agent Acquisition Budget)</h4>
    		<div class="subBlock">
        		<p>A $100 budget will be given to each team for the season. Each team will have the option to “bid” on players they want during the waiver period, which is from the time that player’s game starts through Wednesday morning at 5am cst. 
				The amount you bid on the player is the amount that will be deducted from your total waiver budget if your bid is the highest of all the teams.</p>
			<p>Note: Any player that is dropped will be subject to a waiver period of 24 hours. Any owner can bid on the player during that time.</p>
    		</div>
	
    	<h4 bind:this={fiveOneTwo}>5.1.2 - Waiver Schedule</h4>
		<div class="subBlock">
		<p>Waivers are processed Wednesday through Sunday at 6 a.m.</p>
		    <ul>
			<li>Sunday = Free Agency (waivers run at 6 a.m. central)</li>
			<li>Monday = Free Agency</li>
			<li>Tuesday = Locked</li>
			<li>Wednesday = Waivers run at 2 a.m. central</li>
			<li>Thursday = Waivers run at 6 a.m. central</li>
			<li>Friday = Waivers run at 6 a.m. central</li>
			<li>Saturday = Waivers run at 6 a.m. central</li>
		    </ul>
    		</div>

	<h4 bind:this={fiveOneTwo}>5.1.3 - Help! I accidentally dropped the wrong player!</h4>
		<div class="subBlock">
		<p>There is not much the commissioner can do if waivers have already run. Your best bet to to place a bid on the player you mistakenly dropped. However, if this occurred during the free agency period (Sunday or Monday when you do not have to submit a waiver claim), immediately contact the commissioner. If the player is still available on waivers, the commissioner may choose to communicate the mistake to the league and reverse the transaction.</p>
    		</div>

    <h3 bind:this={fiveTwo}>5.2 - Trades</h3>
    	<p>Trades are processed immediately once agreed upon. A trade will only be reverted if collusion is determined. Just because a trade seems unfair doesn’t mean it shouldn’t be allowed. Bad trades happen all the time in the NFL. There is one exception, however. I will review any trade that involves draft picks, and discuss the fairness of the trade with both owners.
	    If the league collectively voices they are against a trade, I will create a poll and ask everyone to vote for or against the trade to make the final decision.</p>

    	<p>Multi-team trades are possible in Sleeper, so feel free to work with multiple teams.</p>

	<p>It is also possible to trade FAAB and draft picks.</p>

	<p>Draft pick trading is limited to the period between the draft pick lottery and the end of the draft. Draft pick trading is disabled during the season to prevent trading future draft picks. The draft picks involved must be for the draft that year.</p>

	<p>If you are trading draft picks, make sure the amount of draft picks traded away and received are equal. All teams must have fifteen draft picks on draft day.</p>
	
    <h2 class="sectionHeading" bind:this={six}>Section 6: Playoffs</h2>
    	<p>The playoffs begin Week 15 and end Week 17 (one week before the regular season ends). It is single-elimination.</p>
	
    <!-- <h3 bind:this={sixOne}>6.1 - Seeding</h3>
	<p>Every team advances to the playoffs. There is no first round "bye". Playoff seeding is based on record.</p> -->
	<h3 bind:this={sixOne}>6.1 - 8-team League</h3>
    		<div class="subBlock">
        		<p>Every team advances to the playoffs. There is no first round "bye". Playoff seeding is based on record.</p>
    		</div>
	
	<h3 bind:this={sixTwo}>6.2 - 10-team League</h3>
    		<div class="subBlock">
        		<p>Six teams advance to the playoffs. The winner of each division secures a playoff seed and a first round "bye" (1st and 2nd seed). The remaining teams are vying for the last four spots. The top three with the best records of the remaining teams will be the 3rd, 4th, and 5th seeds. 
			Finally, the team with the most "total points for" of the remaining 5 teams will be the 6th seed.</p>
    		</div>
	
	<h3 bind:this={sixThree}>6.3 - 12-team League</h3>
    		<div class="subBlock">
        		<p>Six teams advance to the playoffs. The winner of each division secures a playoff seed. The two teams with the best records secure a first round "bye" (1st and 2nd seed). The leader of the third division and the two teams with the best records of those remaining will be the 3rd, 4th, and 5th seed.
			(Note: The third division leader does not automatically become the 3rd seed. They are guaranteed a playoff berth of at least the 5th seed.) Finally, the team with the most "total points for" of the remaining 7 teams will be the 6th seed.</p>
    		</div>
	
	<h3 bind:this={sixFour}>6.4 - 14-team League</h3>
    		<div class="subBlock">
        		<p>Eight teams advance to the playoffs. The winner of each division secures a playoff seed (1st and 2nd seed). There is no first round "bye". The remaining teams are vying for the last six spots. The top five with the best records of the remaining teams will be the 3rd through 7th seeds. 
			Finally, the team with the most "total points for" of the remaining 5 teams will be the 8th seed.</p>
    		</div>
    

    <h2 class="sectionHeading" bind:this={seven}>Section 7: Keepers</h2>
    
    <h3 bind:this={sevenOne}>7.1 - Changes for 2024</h3>
    <ul>
        <li>Updates coming soon...</li>
    </ul>
    
    <h3 bind:this={sevenTwo}>7.2 - Drafted Players</h3>
    	<p>A player can be designated as a keeper for two years (tenure). This means the player was on a team for three seasons total. On a roster for the first season, then kept the next two seasons if so desired.</p>
    	<p>The cost of a keeper is the round they were drafted the previous year minus one. Example: A player was drafted in the 14th round - 1 round = Keeper in the 13th round</p>
    	<p>1st round picks CANNOT be designated as keepers. You can only keep one player at each position.</p>
    	<p>If you trade for a player, his tenure resets.</p>
    	<p>The deadline to make your keeper designations is three days before the draft. I will send out reminders and review the keepers. If a keeper claim is denied, I will let the owner know why and the owner may designate another keeper selection.</p>
    	<p>Note: You are not locked into your keeper selection. You can change your keepers up to the start of the draft. The deadline is to allow me to set the draft board. If you change your mind on players you are keeping or work out a trade with about owner, let me know.</p>

    <h3 bind:this={sevenThree}>7.3 - Undrafted Players (Free Agents)</h3>
	<p>The keeper cost for an undrafted player is an eighth round pick. Players who were drafted and later dropped retain their original draft round cost.</p>
	<p>Only one waiver or free agent pickup may be designated as a keeper.</p>
	
    <h3 bind:this={sevenFour}>7.4 - Trading Keepers</h3>
	<p>Players who are traded maintain the draft cost of the original team. Example: You trade with Owner A for Sammy Watkins. If selected as a keeper, Watkins will be drafted in the same round Owner A drafted him minus one round.</p>
	
    <h3 bind:this={sevenFive}>7.5 - Keeper Scenarios</h3>
    	<p>You trade for a player and decide to designate them as a keeper. They were selected in the 7th round. You also decide to designate a player you drafted in the 7th round as a keeper. In this situation, one of those picks would be your 5th round pick and the other would be your 6th round (remember last year’s draft position minus one round). You get to choose which round the players are selected.</p>
	<p>You select a waiver/free agent pickup to be one of your keepers. They will now be your 8th round pick. You also have a player you chose in the 9th round you would like as a keeper. One of those players will now be your 7th round pick and the other the 8th round (again you get to choose).</p>
	<p>You trade for someone who was an 8th round pick, already have someone on your team that was an 8th round pick, and have a waiver pickup that will all be designated as keepers. The waiver pickup will be your 8th round pick. You will be allowed to choose the order for the remaining two keepers in the 6th and 7th round.</p>
	<p>You choose your 2rd round pick from last year as a keeper. This is allowed, though it will be your 1st round pick in the upcoming draft. The following year you cannot designate that player as a keeper because he was your 1st round pick. (Remember: 1st round picks CANNOT be chosen as keepers)</p>
	<p>I trade for a player who only had one year left for the keeper designation. On my team his three year tenure status resets. I drop the player and the original team who had the player picks him back up, or I end up trading the player back to the original team later in the season. The player’s keeper tenure status would go back to what it originally was (one year left).</p>
	<p>An owner from the previous year declines to play. A new owner to the league will have the choice to keep players from the previous owner or start fresh. If two or more owners decline to play, the commissioner will perform a coin flip to determine which new owner will get to take over the team of their choice. Neither of the new owners are required to keep players from the roster they are taking over. If three or more owners decline the play, all of the players from the non-returning teams will be returned to the pool. In a similar vein, if the league expands, all of the players from the non-returning owners teams will be returned into the player pool.</p>

</div>
