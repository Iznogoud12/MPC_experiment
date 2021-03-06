Floating monetary anchoring and imbalances - the forgotten links to inflation *Proposal for strategy-proofness* 
============

The present note book is three-fold : the first part presents a model of the international monetary system encompassing both the safe asset shortage hypothesis and Borio's financial cycle buildup hypothesis *(Borio, 2019c)*, while the second and third parts explore the policy recommandations that can be derived from the aforementioned model (the second part goes through a game theoretical approach to design the optimal mechanism for anchoring, while the third part is more closely linked to implementation and immediate policy applications).

*Please allow Binder to be loaded (<1 min), then you can look at the code, change parameters and run cell by cell as in any Jupyter Notebook (Maj+Enter to run each cell once, or use menu shortcut to run all cells under Cell > "Run All").*


--
### Our contribution :

We present here a **dynamic and computational model** of the international monetary system **with a larger number of agents and time periods**, complementing that of for instance Farhi and Maggiori (2017), and He et al. (2015).

While our model confirms their "*rationalization [of] the Triffin dilemma, [...] the common prediction regarding the natural and beneficial emergence of a multipolar world, the Nurkse warning that a multipolar world is more unstable than a Hegemon world, and the Keynesian argument that a scarcity of reserve assets under a gold standard or at the zero lower bound is recessionary*", our framework further bridges these considerations to the secular trends followed by "natural real rates" and inflation for the past thirty years, **expliciting the causal links between forms of monetary anchoring and these secular trends.**

Our model thus enables **calibration on real world data** that reproduces these trends over a long time period, **simulations on alternative future scenarii** on a detailed, country by country and quarter by quarter basis, and a **flexible and modular framework that can provide design possibilities for a strategy-proof monetary anchoring** which would counter the negative incentives, imbalances and trends that are arising from the current design (or lack of design) of the international monetary system. 


--
### Part I's summary : The link between monetary anchoring (*is there a safe asset shortage ?*) and financial cycles (*is Borio's financial buildup hypothesis correct ?*), inflation and globalization, monetary anchoring and long-term trends

Through a model of monetary anchoring we aim to provide an unifying framework explaining how **it is in fact a safe asset shortage that *enabled* central banks such as the Fed (by creating an environment with less inflationary/deficit funding pressure) to "keep output high today", thus "weakening the financial sector and narrowing policy choices tomorrow" (Borio, 2019c)**. Hence lower interest rate today, first made possible in the US by the demand from the Rest of World for USD denominated safe assets, but which then raised the likelihood of a future burst, "whose materialisation justifies even lower interest rates" (still made possible by the still ongoing safe asset shortage). Hence lower and lower US rates, which spilled over the rest of the world's monetary policies, thus creating a secular decline in natural real rates. 

Furthermore, **our model also highlights how globalization would have been the main driver of lower inflation worldwide** - an hypothesis first formulated by Rogoff (2003). Indeed, if one views globalization as the connection of advanced countries' consumer markets to developing countries' industrializing labor forces, while the supply of USD (the global trading and reserve currency) is roughly stable (at least compared to the scale and the magnitude of the new production forces introduced to global markets), then following John Stuart Mill's demand and supply factors determining the value of money (ie what money can acquire ; "the supply of money being, in a nutshell, the totality of money is circulation at the present moment [...]. The demand of currency is composed, on the other hand, of all merchandises put to sale". John Stuart Mill, *Principles of Political Economy*, book III, chapter VIII, paragraph 2, Paris, 1861) **global disinflation occurs naturally as a consequence of globalization**. Even more, inflation in every country is then *at least partly* defined by a component resulting ***only*** from international trade and finance parameters beyond domestic parameters (let's call this global component common to all countries the "neutral" inflation rate). Interesting questions follow, and that we'll try to answer here, are then : "*how much does this "neutral" inflation rate account for in domestic inflation rates ?*" and "*how much influence do monetary policies have on inflation rates then* ?".

Indeed, let's imagine for a minute that monetary policies only have a limited action on this "neutral" inflation rate, such that **no matter how much monetary easings are allowed the inflation rate will never reach the target**.
An important consequence that then follows, if we write inflation $\pi_t$ as a combination of this "neutral" inflation rate $\widetilde{\pi_t}$ mainly determined by international trade and finance and only *partially* responsive to Taylor rules, and of a financial asset price index $a_t$ such as $\pi_t = \widetilde{\pi_t}+ a_t$ , then changing interest rates $i_t$ to change $\pi_t$ will affect domestic financial asset prices $a_t$ to **all the extent** in which the "neutral" inflation $\widetilde{\pi_t}$ does not react to the interest rate change. It can thus be worth studying what factors affect this "neutral" inflation rate and how much power each country has over it (to explain inflation rates that can still differ from one country to another). These are the objects of the study of our Part I.

If our model and hypothesis are confirmed, then the Fed and advanced economies' central banks' over-reliance on inflation targeting rules will lead them to double down on efforts to make this "neutral" inflation rate reach their domestic target, in the process compounding the "low rates beget lower rates" financial buildup aforementioned with *active* inflation of financial assets and bubbles, hence riskier and riskier, and more and more ample financial cycles (as in Borio 2019c). 

All in all, our Part I's model of the existing monetary system provides an explanation of the **"secular long term rate trends" as entirely a consequence of the current (lack of) monetary anchoring**, compounded by misconceived models of inflation and of monetary policies (Taylor rules as above, DGSE and New Keynesian models as criticized in Borio 2019c). 

Indeed, **in a world with a floating monetary anchor inflation can be seen as a corollary of the levels of stock view imbalances. And as a matter of fact, in a relationship between supply of money and supply of goods à la John Stuart Mill, an imbalance favoring one side can be also expressed as a *shortage* of the other.** We can then say that it is the excessive industrial production (compared to the production of "reserve assets", mainly the USD) resulting from the connection of new industrializing countries that produced disinflation, ie a shortage of money (especially of USD - the world's dominant currency) which is reflected by lowering interest rates (since there are less need to invest in future industrial production, which is already in excess), increased USD denominated debt (to make up for the safe asset shortage), and inflated financial prices (the disinflationary pressure on goods prices prop up by contrast non industrial prices, such as financial asset prices, further helped by accomodating policies). The fact that traders are mainly reasoning - unconsciously but *also consciously* - along short-termist, flow views of markets, make them blind to this risk's buildup - are only becomes visible during bursts). 

**Price stability is hence dependant on the stability of the anchoring, which then has to be a sustainable, strategy-proof scheme**. 


--
### Part II and III's summaries : Estimating counterfactuals ; privacy-preserving surveys to estimate fiscal latitude and yield curve control feasability ; optimal hybrid insurance/borrowing-lending contracts for a more sustainable and strategy-proof monetary anchoring

**A simple calibration of our model coded in this notebook will show how the evolution of the inflation rate, the financial cycles, and reserve composition of the main economies, from 1945 to now, can be obtained from just a few initial (and two discretionary) inputs**. This computational and game-theoretic model can also provide guidelines for policies such as yield curve control, and conditionality on their feasibility. 

In fact, given privacy-preserving surveys such as those described in Abbe, Khandani, Lo, AER 2012, institutions such as the BIS could **use aggregated data to estimate how much governmental bonds can be issued by each country without a downgrading of its financing conditions and a potential raise in inflation, *all other parameters held equal*.** In the "global game" literature (à la Carlsson and van Damme 1993, Morris and Shin 1998, He et al 2020) this would equate the case in which some previously unobservable parameter (for instance the "measure of relative strength between country 1 and country 2" in He et al. AER 2020) will be made public, and in which the previously "private signal each investor receives" is identic, ie the noise vanished as in Morris and Shin 2003 ("so fundamental uncertainty vanishes and only strategic uncertainty about each investors' relative rank remains" - uncertainty which can also be partially solved by knowing through privacy-preserving surveys the *aggregated* ranks and willingness to fund from all investors, and this for each country).

Finally, **better financial safety nets and "leaning against the wind" policies can be implemented if such an aggregated funding information is coordinated by the BIS**, as the basis of tighter currency coordination for central banks to distribute at best shocks among them according to a negotiation and resolution mechanism similar to that of the hybrid insurance/borrowing and lending contract derived in Townsend, 1982. **We believe such a stabilization scheme to be Pareto improving, especially on what concerns negative incentives to *manipulate* one's exchange rate and "game" the international monetary system.** 



# Part I

--

### Microfoundations, up to the central banks level

For our model we will stay at a highly abstract, central bank level, game theoretic point of view. Indeed let's first note that **national debts and individual debts play along different rules**. Indeed, to adopt Graeber and Polanyi's language, insofar as individual debts are contracted along impersonal markets with "foreign" entities - people we don't know personally, with whom there is no preexisting history of trust nor incentive for future collaboration - so sets of rules and guarantees are needed to enforce the repayment by the borrower. 

**Countries among themselves are however known neighbors in the global village, condemned to interact with each other for eternity** (at least by the standards of our individual lives). Hence rules of debt closer to that of "human economies", in which neighbors are "always slightly in debt to one another [...] - a delicate web made up of obligations to return three egggs or a bag of okra, ties renewed and recreated, as any one of them could be canceled out at any time" (ibid, p.122), along with display of gifts, generosity and hierarchy following the much richer and more complex meanders of human psychology, which can not and could never be exactly quantified in monetary terms.

We are however only at the beginning of a phase of truly "globally" connected planet, so that **the rules of individual and impersonal markets are still the ones been used between nations (through the monetary anchor, which exactly quantifies and enforces what countries owe each other)**.

***However what happens when a country defaults ?*** It can't be imprisoned, beaten to death to serve as example to others, etc. There is then **a friction there not existing in individual markets**, since countries have more "relaxed" rules of default, **that distort risk pricing and establish a "hard" separation between what are considered safe assets (they are then really safe), and not as safe assets (pretty much the vast majority of countries' debts)**.

This is what we referred to as  "top-down vs bottom-up modeling in international economics": indeed, while Borio argues that "in sharp contrast to the current standard New Keynesian frameworks, the friction underlying deviations of market from natural interest rates is a capital market failure rather than price (and possibly wage) stickiness", we would like to add that **this "capital market failure" is in turn a result of bad incentives created by a even broader game, that of fiat monetary anchoring**.  Especially, different countries and cultures might have different preferences and definitions of utilities, which have to be accounted for in any macro framework derived from micro foundations (or, as in our case, be left as exogeneous parameters that can be adjusted on a country by country basis). Then the village economy analogy we used in the previous part naturally calls for game theory models, such as those underpinning the borrowing and lending, and insurance literature as in Townend 1982, 1982a, 1989, and as in the "global game" literature.


### There are thus only countries in our model, let's say N countries, and each one with their national currencies (no goods for now!)

We will start first with **a most basic multiagent asset allocation scheme**, that of Bogolmonaia and Moulin (2001)'s cake-eating game, which we will progressively complexify and merge with standard open macroeconomy models. 

Indeed we believe that **this model provides a close analogy to real life operations** by central bank officers, and can complement existing models such as Mundell-Fleming **on how safety considerations are being carried out dynamically in time, along with risk vs returns logics**. Furthermore, this highly abstract model can merge well with existing macroeconomy models, **by enabling calibration of practical values in highly stylized model such as the Safe Asset Scarcity and Aggregate Demand version of IS/LM developed by Caballero, Farhi and Gourinchas (AER, 2016)**. Indeed, the slope of the AS curve gives a sense of what inflationary pressure a country faces.  

Indeed, we believe that the superposition of games with incentives on top of existing models are **not competing but complementary views**, just as Roth's suspension bridge building analogy illustrates how in addition of "simple, beautiful and indispensable physics", "bridge design also concerns metal fatigue, soil mechanics, and the sideways forces of waves and wind". **International macroeconomics thus also unfolds within a game of economic competition and collaboration, whose rules - even if they "might be impossible to be answered analytically"** - must still be explored (and maybe computed), to allow "bridges designed on the same basic model to be built longer and stronger over time, as the complexities and how to deal with them become better understood" (Roth, 2002).

--
### Our model

Because we are in a fiat monetary anchoring, we postulate here that **each national currency's "purchasing power is limited to the amount which trading partners accepts to receive"** (here we can recall Schacht's analysis of "the war of 1914, which provided telling proof of the fact that state-guaranteed paper money, unlike gold and silver coins, does not represent any substantial value [...]. The war of 1914 isolated Germany from the greater part of the world market.  The Mark had become unusable on enemy markets. It has lost its purchasing power". (Schacht, *The Magic of Money*, p94).

Hence our model of the international monetary system, which consists in just countries. Each of these countries print fiat money, which has to be accepted by others in order for it to have any purchasing power. Hence **each country can be represented by a "mice"** (the country's aggregated investors - central bank managers and asset managers), **which absorbs the "cakes" (the fiat liabilities) generated by himself and by other countries**. 

The liability side can also more simply be viewed as bonds, link to the He et al. (2015) model of safe asset pricing. But multi round, multi players.

**Time is discreet, in rounds**, to represent the discretionary decision process of investors such as central banks and asset managers. To represent **private information and secrecy of the decision process**, all parameters involved in the decision process (each "mice"'s preference ordering of the "cakes", each "mice"'s absorption capacity at this round) are decided before the start of each round, and can't be modified once the round starts.

During the round (let's call it round T for instance), **the allocation algorithm follows that of Bogolmonaia and Moulin (2001)**. Each country i (out of N) - the "mouse i" simultaneously absorb each others' cakes $\zeta_j,_T$, with j$\in$T (the trade process, à la Wicksell triangle) at different absorption speed ($\omega_i,_T$ for country i - if one views a round as a new Treasury bills emission auction, some reserve managers have bigger budget and bidding capacities, here reflected by the different absorption speed), and each one following its own preference ranking $P_i,_T$. While $\zeta_j,_T$ $\in$ $\Bbb R_{>=0}$ and $\omega_i,_T$ $\in$ $\Bbb R_{>=0}$, $P_i,_T$ is a 1xN matrix  which contains a single time every integer between [1,..N]. **When a cake by one country is finished the countries j that were eating it move to the item below in their rankings matrices $P_j,_T$** (end of the Bogolmonia and Moulin 2001 algorithm. We chose it because of its versatility, its natural illustration of the safe asset shortage - see just below as to ***what happens if specific cakes are left unfinished at the end of a round*** - and to prepare for the axiomatic analysis we will conduct in Part II to make the anchoring game sustainable and strategy-proof). 

Each country's aggregated investors (central bank reserve managers and asset managers) stores what they absorbed in the country's aggregated reserves (central bank reserves and asset managers funds). **The state of the world at round T can thus be represented by one NxN endowment matrix $E_T$**, which records how much cakes in total each country has generated up to round T, and which countries are holding which proportion of these cakes. For convention we can fix column j of this matrix as all the cakes issued by country j, and line i of this matrix the cakes absorbed by country i. Cell (i,j) hence denotes the size of the cake issued by country j that country i absorbed into its own reserve.

Hence $E_T$ = 

$\begin{bmatrix} 
c_1,_1,_T  c_1,_2,_T  ... c_1,_j,_T ... c_1,_N,_T \\
c_2,_1,_T  c_2,_2,_T  ... c_2,_j,_T ... c_2,_N,_T \\
... \\
c_i,_1,_T  c_i,_2,_T  ... c_i,_j,_T ... c_i,_N,_T \\
... \\
c_N,_1,_T  c_N,_2,_T  ... c_N,_j,_T ... c_N,_N,_T \\
\end{bmatrix}$

And we have the relation, to denote the fact that column j of $E_T$ represents all the different shares of the cake $\zeta_j,_T$ issued by country j at round T, absorbed by all countries i (if $\zeta_j,_T$ has been totally absorbed during round T) : $\zeta_j,_T = \sum\limits_{i=1}^N (c_i,_j,_T - c_i,_j,_{T-1} )$

Note that what the "mice" has absorbed can be seen as the "asset" side of a country, whereas all the pieces of "cakes" that it generated can be seen as the "liability" side of that country (to relate to the view of the US as "the world's banker", cf Despres, Kindleberger and Salant 1966).

**At the end of each round (each round has a pre-fixed duration) a country's cake that hasn't been totally absorbed will face a devaluation** (since the rest of the world is denying it its current purchasing power), which is reflected in the endowment matrix as a decrease in value of the parts of all reserves that contained pieces of cakes (from all previous rounds, not just this round) from that country (so the endowment matrix is normalized to an unique unit of account !). This can be seen as decreasing the values of an entire column j in the endowment matrix, if country j's cake hasn't been totally absorbed by himself or others at the end of the round.

**Link to rollover debt and default à la Calvo (1988)** and Cole and Kehoe (2000), as described in He et al. 2015, but could also be a **link to the role of limited financial risk bearing by financial intermediaries in the exchange rate determination theory of Gabaix, Maggiori (JPE 2015)** - when aggregated investors have less appetite for a country's cake its price decrease, so devaluation. But when excess demand its price increase, so decreased rate (?). 

This link to Gabaix, Maggiori (JPE 2015) will be important in the policy implications of our model,  and the attempt of designing strategy-proofness of part III. 





--
### Discussion on investors' behaviour - what are part of 'global game'  considerations, and what are individual rational true preferences ?

Countries' preferences ordering can be for instance a function of their trading preferences, their trading partners' cakes' "safety", interest rate, sizes, strategic alliances.... See in more details in code cells below how rankings and cakes are generated by each country at each round, and on how endowments change according to countries' behaviours. 

**For now let's assume that each ranking is done according to true preferences, and that there is no attempt 'to manipulate' the game**. Indeed here we first want to see **what long-term 'natural' tendencies come out of this game** (and we postulate that in real life most private investors like asset managers don't think about the 'global game' consequences à la He et al., AER 2020, except in an Instability zone à la Farhi, Maggiori, QJE 2018. Hence preference ranking that are parametrized computationally by weights on safety, interest rates and inflation, and considerations around the sizes of each economies, etc listed in the code lines at the end of this paragraph). 
*Part II and strategic proofness will examine this postulate more in details, and define more precisely **how gaming the system actually happens (manipulating the exchange rates instead of manipulating the safety of other countries' bonds)** and how to prevent this*.

Countries can adjust the interest rates they pay on their "cakes" to make it more attractive. 

Inflation in our model can first be seen as just the corollary of devaluations (a country that devalues see the prices of goods imported increase - hence inflation). For now because we don't take goods into account **we can just assume that all goods are imported, from a fictional third party supplier of goods not playing the game** - which is made possible by the normalization of our game to an unique unit of account). A more sophisticated view of inflation in our model would be related to purchasing power ; indeed, **if other countries *accept* an expanded purchasing power by a country by including more of its issued pieces of cake in their reserve, than the inflationary pressure for this country would be lesser** (and the lesser the inflationary pressure the less effective lowering interest rates will be at pushing inflation up). 

So our framework would also allow to compute for every country the elasticities of their inflationary pressure and the counterfactuals should parameters for some other countries be modified.

*For instance the relevant lines of code concerning countries' trading preferences are, in the cell in annex below (two versions of how trade preferences are weighted) : 
- [~,trading_order]=sort(trading_preferences(k,:).*(ones(1,number_of_countries)+endowments(k,:)),'descend'); %the simplest version
and
- [~,trading_order]=sort(trading_preferences(k,:).*(ones(1,number_of_countries)+max(0,successfully_loaded_cake_last_round(k,1).*(history_counter(k,1)-deval_history(k,1)).*endowments(k,:)*(interest_rate(k,1)))),'descend'); %a slightly more complicated one 
    
*The reserves accumulated by a country i - read as the lines i of the endowments matrix - are used as proxy of the size of its economy in our model. The columns j of the endowments matrix are read as the cakes generated by country j. So the endowments matrix is really just keeping in time record of how much each country i is holding debts from each other country j. 

Let's also note that to reintroduce goods in our model, Schacht's 1914's wartime observation that "even at points where Germany bordered on neutral neighbours, the purchasing power of the Mark was limited to the amount which these countries were able to employ to purchase German goods" will allow in a trade model coupled with our monetary model, in which different quantities and shares of imports and exports are built in for each country.

But let's not complexify our model yet. 


```python
# Exogeneous parameters of the simulation to be played with in the rest of this notebook

number_of_countries = 6 %total number of countries in the simulation
number_of_rounds = 7 %total number of "cake eating rounds" 

interest_rate = (0.03).*ones(number_of_countries,1); %initial interest rates - more below on how interest rates change according to how successfully debt is absorbeb at each round.
interest_rate_history = zeros(number_of_countries,number_of_rounds);

uni=0.7; %uni is used in the random generation of the trade preference matrix - a number_of_countries x number_of_countries matrix in which the number line i, column j indicates how interconnected the economies of countries i and j are. This random generation is done with the function R = sprandsym(n,density) - in our case n=number_of_countries and density = uni, which returns a symmetric random, n-by-n, sparse matrix with approximately density*n*n nonzeros; each entry is the sum of one or more normally distributed random samples, and (0 <= density <= 1) .For calibration uni=0.3 creates with good probability if there are 6 countries in total 3 trade coalitions, one with 3 countries, one with 2, and 1 in autarky.

%If we were in Matlab we would have added the parameter rc=0.02, still for this sprandsym function, which denotes how inequal trade between countries can be (the smaller the more). Indeed,  R = sprandsym(n,density,rc) returns a matrix with a reciprocal condition number equal to rc. The distribution of entries is nonuniform; it is roughly symmetric about 0; all are in [−1,1]. If rc is a vector of length n, then R has eigenvalues rc. Thus, if rc is a positive (nonnegative) vector then R is a positive (nonnegative) definite matrix. In either case, R is generated by random Jacobi rotations applied to a diagonal matrix with the given eigenvalues or condition number. 
```


--
### The code cells below are used to produce simulations of the game we just described, to illustrate the incentives and trends it produces

We have described above the demand side. **For now the supply side is coded according to deterministic rules** (see the exact coding below, which you can change and relaunch yourself using the "Cell" button at the top of this interactive notebook. Basically the supply side starts by some random initialization, then **whenever a country does not suffers a devaluation then it will try to increase the size of the cake it will generate at the following round, and if there is a devaluation it will reduce the size of the cake it will generate at the following round**. The absorption speed for each country at each round is a function of the size of its total reserves, as a proxy of its GDP for instance).

One could encode in the supply side more sophisticated monetary rules such as the Taylor one, or some cyclical aspect like the domestic financial cycles described by Borio et al (2020). 

But for now our simple simulations (that you can reproduce yourself with the code provided below, and that you can run directly in this interactive notebook) already shows the following figures and results :

- **let's first observe generally, before we even enter in the details of how debt sizes, eating speeds, and preference rankings are endogenized, how **repeating such a game with a large number of countries integrate the notion of "safety", which brings here a positive feedback loop**. Indeed a country that doesn't default in the past will be perceived as safer, so would be ranked higher, hence will indeed become safer (and thus could issue bigger debts at each round). Then if we let $D^i_t$ be the debt size of country i at t and $\bar{D}_t$ the average debt size at t, and define $S^i_t$ =  $D^i_t/\bar{D}_t$, with the growth equation $S^i_{t+1}$ = $\gamma^i_{t+1}.S^i_t$ **one would only need to assume that the growth rates $\gamma^i_t$ are i.i.d. random variables to Gabaix (2009)'s proof of a resulting power law distribution** (with the existance of the steady-state distribution guaranteed by frictions that both prevents small countries from becoming too small and a lower bound for sizes enforced by a reflecting barrier - for instance a fixed cost that prevents anyone to start a very small country). This is **to give an intuition of how a winner-takes-all reserve currency can account for a larger and larger share of the global economy's reserve, due to its "safety" advantage**. 

Then some more detailed simulations and observations :
**First a 6 countries in 3 trade groups, 7 rounds simulation (just 7 rounds are enough to see trends !)**

- in our simulations the interest rates are computed deterministically - after a random initialization, after every round during which a country successfully (unsuccessfully) unloaded the piece of "cake" it generated during that round its interest rate will be decreased (increase). It is for us a very visual way to **see how much inflationary pressure there is on a country round after round** (so how flat its AS curve is - the higher that "interest rate" the steeper it will be).

- the size of cakes, aborption speed... all tend to powers law i.e. one country (here country 1) gains much more than any more in that trading group (mathematical proof in paper). Intuition is that as it is perceived "safer" by other countries (because it devalues less) the "cakes" it generates are always eaten first by other countries, and thus this "popularity margin" / "monetary latitude" allows country 1 to emit bigger cake later, invest more in its cake absorption speed (proxy of GDP), absorb more in other countries' cakes as well, etc.

**This already highlights how the USD's position as the dominant reserve currency is easily self sustaining, and allows its monetary policies to reach for lower rates without funding or inflationary pressure** (simulations and calibrations in Part II will explore more closely the limits of even a dominant reserve currency, and the conditions in which Triffin events might arise). 

Additional observations :

- the country that would gain the most is **determined by initial conditions** (in this very easy example everything is initialized at random, but looking at the initial ranking - the higher the score the most sought after a ranking is - and the initial interest rate we can already tell that country 1 will be winning !)

- the country that would gain the most in a trade group is **not necessarily the one determined by fundamentals** - i.e. not the most connected one or the most prudent one *(in the trade group between country 1, 4 and 6 country 1 is neither the most connected - since country 6 has more connections than it does - nor the most self preserving - since country 4 ranks its own debts to others' higher first)*

<img src="Screen%20Shot%202020-04-02%20at%2010.14.45%20AM.png" /> 


**A second 6 countries in 3 trade groups, 7 rounds simulation**

- Here the winner is country 3 - which is less connected (only to country 5) than the cluster with countries 1, 2 and 4

- The worse off country in the group (1, 2 and 4) is doing even worse than country 6 in autarky (extreme case of the model, because country 4 started (randomly) at the least preferred country in country rankings, and failed to get its cakes eaten at the end of round 1, thus devalues round 2, its interest rate surge, and it gets stuck in a devaluation sprial from round 1 to 4.

- Note that here **country 1 had better initial conditions to be the be winner of the simulations (best ranked country at the start, lowest interest rate at the start). But its trading partners - country 2 and 4, are the ones devaluing the most** 

<img src="Screen%20Shot%202020-04-02%20at%2010.44.32%20AM.png" /> 


**Finally a 9 countries, 1000 rounds simulation**

The figures below illustrate the long rung trends in this model :

- **Reduction of average global rates / average global inflationary pressure can happen** (see rounds 120 to 220 on both the cumulated. This is when the total absorption speed is faster than a period's timer times the total generated cakes in each of these rounds, hence the reduced number of devaluations rounds 120 to 220 

- **Triffin events exist** : the yellow country (country 3) started as the winner of this simulation, until around round 220 at which point it is overtaken by country 1 in deep blue and don't stop devaluing until the end of the 1000 rounds. This corresponds to fundamental analysis (country 3 is only trading with 2 countries whereas country 1 with 4. But countries 6 and 9 for instance are both connected to 4 trading partners, with stronger ties among some of them and with themselves. These two countries are respectly the 2nd and 3rd most sought after countries, both in rankings, in upward trends in rankings, and in how much of their cakes are absorbed by others as reserve).

*Note that these long term analysis will be nuanced by a more calibrated simulation in the notebooks on 1945-now and after Covid-19, available here and here, in which the cake absorption speed and cake generation speed are governed by more complicated but more realistic laws* 

<img src="Screen%20Shot%202020-04-02%20at%2011.07.19%20AM.png" /> 

<img src="Screen%20Shot%202020-04-02%20at%2010.55.01%20AM.png" /> 

# Part II :

--
### Estimating counterfactuals, fiscal latitude and yield curve control feasability 

Our computational and game-theoretic model can also provide guidelines for policies such as yield curve control, and conditionality on their feasibility. In fact, given privacy-preserving surveys such as those described in Abbe, Khandani, Lo, AER 2012, institutions such as the BIS could use aggregated data to estimate how much governmental bonds can be issued by each country without a downgrading of its financing conditions and a potential raise in inflation, *all other parameters held equal*. 


### Calibration of our model on 1945-now, to illustrate how for a few inputs it can reproduce the evolution of interest rates, inflation and reserve composition

We present here the detailed code used for the simulations. For that we first calibrate, by **just initializing with data from 1945, and changing three times some preferences** (the Marshall plan between 1948 and 1951, US investments in Japan between 1953 and 1955, and China's opening since 1978), **to reproduce by letting the game play by itself the main trends observed from 1945 to now (2020), and to obtain after 75 rounds today's reserve composition**. Being able to capture these features of past history will provide confidence and intuition in the model's inner workings. 

That also lead us to provide several scenarii in how the models' parameters will change following Covid-19's increase in debts *(these parameters from the model being for instance the change in debt levels, while debt absorption speed are maintained roughly constant. Different degrees in shifts in trade and supply chain preferences are also considered)*. We thus generate 50 more rounds after a common departing point, and report here the different outcomes, and the different probabilities of each outcome (since they are intervention of random perturbations in the model the probabilities of each outcome is calculated based on how many of different random sequence generate this specific outcome).

### And estimating covid debt shocks' impact on countries debt sustainability, reserve composition

The simulations of extra Covid debts show that :

- **in the case of everything constant (pre Trump US and China trade relations)** debts are overall sustainable, with adjustements in reserve levels and contraction of countries' economies depending on how affected by the crisis they were.

<img src="Screen%20Shot%202020-04-06%20at%2010.05.35%20AM.png" /> 

- **similar results in the case of everything constant, with just additional reliance on trade with China** (for instance for masks, medical supplies etc). The economic contraction is smaller, and the global reserve contraction as well. This could be interpreted by the fact that the additional trade with China is flushed in its reserve (the increase can be seen in the graph below), used to acquire other countries' debt (inferred from the lowering of global interest rates) and thus sustaining economic activity 

<img src="Screen%20Shot%202020-04-06%20at%2011.13.15%20AM.png" /> 

- **in the case of everything constant among all countries except China and US, who in that scenario stop trading with each other**, they are small probabilities of a global contraction (less reserves, less debts, less GDP growth) that preserves the overall shares of each country in the global economy - except for China in the global economy which suffers more. However in these small probability event the US go through an initial bubble fueled by the decrease of China, that then collapses back to the initial level (and note that after this collapse China's share is also back to the initial level - but with the cost of a global contraction, especially for all EM markets). **And with the caveat provided just above that this debt model doesn't take into account other incentives and consequences created by such dynamics - small probabilities in economic contraction in one country might leading to escalating tensions on other dimensions as well*

<img src="Screen%20Shot%202020-04-04%20at%209.50.20%20PM.png" /> 

- **in the case of stopping trade between China and the US AND additional reliance by other countries on China**, there is high probability for a sudden takeover of the role of the US as reserve currency China, accompanied by strong contraction for every other country. **Again, with the previous caveat of unaccounted destabilizing geopolitical consequences**

<img src="Screen%20Shot%202020-04-04%20at%209.57.55%20PM.png" /> 


- **finally, in the case of our proposed stabilization scheme** *(details in the paper - in the model it is just reflected as more willingness from participating countries to accept others' devaluation - see the commented code in the last cells of this notebook. Un-implemented here is also the extra information each country will have on how much latitude they will have at each round on their debt, which should also help in addition of the effects produced here to stabilize debts, interest rates and balance global reserve currencies)* the effects of all above scenarii are smoothen, with much more balanced reserve currencies (at least 3 currencies accounting each more than 20% of the global share of reserves, with the exact currencies - most often Germany ie the Euro, or the JPY - switching depending on the random shocks, but without adverse effects on all countries - including on the US even though the dollar loses its monopoly as reserve currency)

Examples from one representative random initialization 
<img src="Screen%20Shot%202020-04-04%20at%2010.12.50%20PM.png" /> 

Examples from another representative random initilization
<img src="Screen%20Shot%202020-04-04%20at%2010.13.52%20PM.png" /> 


# Part III

--

### Introducing our model of monetary anchoring, secular trends, and the incentives to "cheat" such an anchoring game creates

Mundell’s redundancy (or "n-1") problem illustrates how international finance can be interpreted by some as a zero-sum game, with many prisoners dilemma problems. Such a view logically leads some countries to **try to "game" the international monetary system**, first and foremost through their managed floating currencies (hence the vocabulary around "manipulation" on what concerns exchange rate levels).  

In fact, since the dollar unpegged from gold and some currencies started to float, exchange rate manipulation has been tolerated up to some point - principally because of the increased difficulty in pinpointing exactly what the "fair" parity between the two legs of a currency pair would be, which itself would influence in return all other currency pairs these two legs are involved in.

The term "fair exchange rate levels" itself changed meaning, between a Gold Standard world in which the anchor aimed at adjusting (im-)balances of payments, and a free floating world "in a global liquidity trap, in which the exchange rate affects the *distribution* of recessions across countries" (Caballero, Farhi, Gourinchas, 2017).

Here we provide a model and simulations in an interactive Notebook format to load and play directly with the Matlab code **to examine how international monetary systems relying on specified nominal anchors (silver and gold, sterling then USD, bancor sometimes maybe)** - though the most "natural" form of anchoring, as it provides a solution to commitment and reneging issues - **create incentives that might be correlated with hegemonic wars** *(political scientists - Wallerstein, Modelski, Organski or more recently Goldstein - have long explored these cycles, but economists also advanced some causal hypothesis. Vilfredo Pareto in his "Forme di fenomeni economici e previsioni" for instance postulated that ascending and descending phases in international trade are linked to more or less available saving levels, and that period of social unrest and cross-country wars occur in such descending phases)*.

Notably, our model's extension with goods, in a separate paper, will lead to a reinterpretation of Ibn Khaldun's imperial cycles (the intuition being that of Paul Kennedy's emphasis on productive capacities in determining winners of wars, as laid out in *Rise and Fall of the Great Powers: Economic Change and Military Conflict from 1500 to 2000 (1987)*, which determines the cycle of dominant elites - the ones most able to channel and retain - capture! - the productive resources and capacities produced by the Rest of World. For instance the Victorian age UK, the gilded age US, and now the post-economic opening China. And, within a cycle, the eroding of the elite's "productivity capture" due to rising inequaity, rising intra-elite competition, etc has put down in complex dynamic systems format by Peter Turchin. We will aim to bridge these three frameworks.)

Here, let's just **recognize (through our Part I) that the current international monetary systems provides incentives / insidious pressure** (through inflationary pressure) to **hijack countries' *sustainable level of consumption* to an overvalued purchasing power that satisfies the safe asset shortage** (but which also leads to a decline in long-term interest rates, lowering the potency of monetary tools, while building up financial risk, as a side effect). 

So **an optimal scheme need to both *counter* (for safer countries) this incentive to over-issue debt, while *prevent* (for not as safe countries) the possibility of manipulating its currency for faster growth and development** (which come at the cost of increasing the safe asset shortage, hence adding pressure for safer countries to over-issue).


### A role for mechanism design 

Central banks' reserve management operations and the decision process revolving around them naturally call for game theory models, such as those underpinning the contract theory, borrowing and lending and to some extent medieval village economy literature. 

Exchange rate levels as a start ("the trade-off of internal purchasing power / external competitivity ones wants to retain for it countries, that has to agreed to by other countries")

So it is linked to exchange rate determination theory.
But exchange rate determination in practice is through multinational bank. Indeed, the theoretical advancements on exchange rate determination now put the emphasis on market frictions caused by the few risk-bearing financial intermediaries' shifting perceptions and acceptance of currency risks, whose multi-currency balance sheets readjustments thus constitutes "first-order determinants of exchange rates and their volatility" (Gabaix, Maggiori 2014).

However, if Gabaix and Maggiori (2014)'s main bearers of the risks resulting from international imbalances are the "highly concentrated, few large financial players ranging from the [former] proprietary desks and investment management arms of global investment banks to macro and currency hedge funds, active investment managers and pension funds", empirical data show evidence that these actors are only bearing the *marginal* currency risks, while central banks are bearer "to the first order of approximation of all net foreign demand for 'safe' US assets from 1990 to 2014" - (see figure 1 below from cfr, February 16, 2018, echoed by Alessandro Dovis discussing GaMa models at the NBER Monetary Economics Meeting of March 7, 2014).

<img src="dollar-fx-v-cumul-purch.png" /> 

This observation is then prompting us to reconsider whether the aforementioned policy trade-off (between absorbing shock into reserves or letting it increase the exchange rate volatility) is veritably a trade-off, or in reality an unilateral policy forfeiture - since it seems that *excessive* volatility is the result of *excessive* concessions made to private agents that are, after all, only marginally concerned with the underlying risks. With consequences such as flash crashes - resulting first from very short span imbalances in order books (see figure 2 below from the Bank Of England's Staff Working Paper No. 687, October 2017). 

Let's also note that *most* central banks actually are aware of this fact, and actually work against such privately created volatility. Frankel (2019) illustrates for instance how most central banks are guided by internal *systematic* (systematic floating, or "dirty" floating) rules concerning such trade-offs, and how reserve management objectives can be an important term in the equation. The level of exchange rate volatility can then be viewed as determined by the policy trade off of how much of these shocks are to be absorbed into central banks reserves, and how much are let into exchange rate fluctuations.

**We thus see here how the proper exchange rate level determination and exchange rate volatility are part of the same problem here**. 

So one needs an unifying framework around exchange rate levels, exchange rate volatility, financial safety net, policy debate on dilemma vs trilemma, leaning...(cf Domestic financial cycle, vs global financial cycle)

The unifying framework : let countries take back control COLLECTIVELY on BOTH exchange rate level determination and exchange rate volatility (which some are already doing anyway, cf Frankel's systematic managed float)

How to do the COLLECTIVE part ? 
Negotiation part linked to the "global game" aforementioned
provide common values in signal ?




--
### Mechanism design concerns :

Let's first observe that the original Bogolmonaia and Moulin's good assignment game mainly concerns itself mainly with **what axiomatic properties such a game has**. Notably that it is **ordinally efficient, fair** (i.e. if everyone prefers his or her assignment to the assignment of anyone else with respect to the reported preferences) ***equal treatment of equals*, but not strategy proof** (i.e. agents might try to manipulate the game - for instance if too many people like the second choice of an agent as their first choice, then this agent may be better off if he starts eating from his second choice instead of his first choice). Furthermore, they proved that **there is no mechanism that satisfies ordinal efficiency, strategy-proofness and equal treatment of equals**. 

**What do these imply for our adaptation in monetary anchoring ?** Let's first note how the entire language around ***"manipulating one's exchange rate"*** hints at such market design considerations. Indeed, if one combines a non strategy proof mechanism with the long-term incentives of a repeated game based on this mechanism leading to a "winner takes all" reserve currency (and economy), then any agent will have incentives to try to manipulate the game to try to be better off in the resulting distribution (and become closer for instance to being a "world's banker", cf Despres, Kindleberger and Salant 1966).

Also, NB : Bogolmonaia and Moulin's scheme's ordinal efficiency is not that important in our case, since there are secondary markets on which countries' debts can be acquired at any points in time - even though potentially at a higher price. What Bogolmonaia and Moulin's model was used to highlight was indeed rather to decide which countries' debts will NOT be fully endorsed by the end of a round. And since this is the only case incurring a "penalty" to countries in our model, let's examine what factor can play there (hence which levers of "manipulation" countries have).


--
### Collectively preparing a new Bretton Woods :

Let's also note here that it is the approach we are following so far that is of interest - the specific model and incentives analysis indeed might change in the future, but hopefully many bright minds from market design and contract theory will contribute in examining the monetary anchoring supergame, so that the world comes ready when a new Bretton Woods will be called, and that the contingencies at that time do not dictate its outcomes. After all, **“there is, in particular, all the difference between deliberately creating a system within which competition will work as beneficially as possible and passively accepting institutions as they are”** (Hayek, The Road to Serfdom)
So where are the "tension points" in our game ? Let's first note where a country can intervene (the size of the cake it issues at the beginning of each round, its interest rates, its eating speed during each round, and its preference ranking), and where it can not (the same parameters for every other countries, plus inflation rates for all countries). Then where privacy intervenes - the cake sizes and eating speeds are known by all at the start of a round, but each country's ranking lists remains in practice private (so in our game the sizes of the cakes issued at the beginning of each round do not factor in the potential rankings). Let's recall there the application of the literature on optimal borrowing lending - and how privacy-preserving technologies can now allow implementations of some schemes designed in the 80s (Townsend 1982, and how technology lowered the cost so became interesting enough to use these more complicated form of contracts).

Then how do countries potentially improve their lot through interactions with other countries (one could call that manipulating the game - though what I mean here is more on how to interact with other countries so that in the same rules of the same game your outcome improves) ? It has to deal with the private information part of the game, since if known then a country could just adapt its own parameters accordingly (for instance if known all what other countries will eat, with what speed and in what time, one could know until what cake size he'll be able to issue successfully this round). 

Also looking in more details in how these eating order ranking done by each country is made - we can note that trade partnerships at least intervenes in most of the different modeling of how the ranking is done (one could also imagine military alliances, size of countries' economies...). And what is the best way to gain more trading partners ? By producing more goods, of better quality, or cheaper. So we can relate here this fact from the "exchange rate manipulation" language noted earlier. 

Hence, a better monetary anchoring game for us will consist in both giving better information to each country about the aggregate other countries' private rankings, so that it can better decide on the size of the cake/debt it issues at a given round/quarter, all the while ensuring that competitive devaluations are avoided. So any optimal monetary anchoring scheme has then to be both an exchange rate stabilization scheme (that still allows to allow for exchange rates to help mitigate unforecasted shocks, and to account for cultural differences among countries - as some exporting countries might agree to finance more importing countries) and a privacy-preserving demand aggregation scheme. And this on a multilateral scheme rather than on networks of bilateral trading partners - as for us only a truly flexible reserve composition and global governance and negotiation platform can lead countries to compete fully on economic terms with less incentive to wage war.



--
###  Optimal hybrid insurance/borrowing-lending contracts, for a more sustainable anchoring


**Let's see in the model what would happen if each agent could see before the start of the round some aggregated information about others' preference ranking, and/or others' total cake emission, and/or others' total absorption speed.**
Solving the commitment issue through the use of options ? (see below)

### Privacy-preserving technologies to implement mechanism design's planner

Aggregation of private information, we have seen above, could provide a valuable insights to countries to see how much margin they have in issuing their debts, for them to be securely endorsed by others. We present here an existing and maturing privacy-preserving technology, that could perform such privacy-preserving aggregation of countries' rankings.

Let's note that this can be organize with or without a trusted third party (such as BIS - that would just perform a "computational" role without ever seeing any inputs). First each country "pings" each other (like knocking on each other's door), so that they together generate a shared encryption key (we'll discuss this more in the appendix). That's step 1 in the image below.

Then they both input their message (step 2a below), and encrypt it on their computer (step 2b).  Then they send these encrypted values to each other (the best setting, in which the "dealer" or "central server" handling the computation is replaced by both agents interacting to perform the computations themselves - cf the detailed cryptographic appendix. 

In less sophisticated settings that can be replaced by a server - which is what is mentioned on the image below, step 3. 

If the encryption is done properly (which we can assume it is, if implemented correctly) none of the agent should be able to decrypt the other agent's value - whether this value being handled by a central server or by the players themselves (to answer your concerns in the first email of the day:) 

Then the computation (so the function that performs the aggregation - it can be a sum, an average, or any other collection of linear operations) is done (either by the central server, or by agents' themselves), and the results - still encrypted, comes back to each agent

Both agents need to agree to decode for the results to be decrypted - by both of them so both have a copy of the same result.  (step 4 and 5 in the image below).


--
###  The optimal hybrid insurance/borrowing-lending contract, adapted to central banks and exchange rate determination

The seminal result by Kareken and Wallace (1981) that the nominal exchange rate is indeterminate in
a world with pure interest rate targets also applies when the economy is in a global
liquidity trap, since both countries are permanently at the ZLB. However, in our framework and
in contrast to the environments envisioned by Kareken and Wallace (1981), this indeterminacy has
substantive real implications. Different values of the nominal exchange rate correspond to different values of the real exchange rate, and therefore to different levels of output and the current account across countries. This mechanism means that, via expenditure switching effects, the exchange rate affects the distribution of recessions across countries in a global liquidity trap. This creates fertile grounds for zerosum beggar-thy-neighbor devaluations achieved by direct interventions in exchange rate markets, stimulating output and improving the current account in one country at the expense of the others.

So to stabilise the exchange rates, in our game theoretic cake-eating model, at the core of our proposal resides the *multi-currency* nature of the market making activity of international banks, which we aim at replicating at a central bank level. A first underlying reason would be that of *collection of risk* - in the line of bigger risks for higher returns. Additionally (and that is a second reason for emphasizing the multi-currency aspect) in our case the additional risk is that of adding on more exotic currencies such as the South East Asian ones in a reserve basket previously not containing them - that could thus act as an additional cushion to mitigate external shock on them.

It is then possible to see that for such a **multi-currency reserve balance sheet** the profit objective of traditional private market maker is here also aligned with the volatility stabilization objective of the central banks involved, and that the mechanisms underlying these forms of interventions would be conceptually the same as the ones through which financiers' alterations to their balance sheets affect both the level and volatility of exchange rates.

The design question then, critical to the feasibility of such a multi-currencies account for instance, is on **how to create and foster this form of collaboration among different central banks**.

--
### Computing these multilateral balance sheets, through privacy-preserving methods

Privacy-preserving methods like multiparty computation *(referring to the financial adaptation of Abbe, Khandani, Lo, 2012, which build on Yao 1982; Goldreich, Micali, and Wigderson 1987; Ben-Or, Goldwasser, and Wigderson 1988; Chaum, Crépeau, and Damgard 1988; Beaver, Micali, and Rogaway
1990; Cramer et al. 1999)* provide a clear and useful framework on which to **reach agreement on the different exchange and interest rate objectives pursued by respective central banks**. This is why this section will build on the language and framework of these privacy-preserving methods - which again don't have to be *actually* implemented for the interventions to be conducted.

1. Thus central banks would first each allocate some funds denominated in their national currencies, plus portions of their reserves in each of the currencies they would like to stabilize their exchange rates with. 
2. They would then set-up the daily volatility bands they want their national currencies to stay in, which proportion of reserves they are ready to commit to the operation, and what amount of risk or leverage they are ready to bear on any derivative instrument used in the process (for convenience let's imagine the updates are only feasible at a regular interval - for instance once a day or once a week. We are then in a discreet time setting). These three points are where privacy-preserving methods might be applied, since participant central banks wouldn't want for instance *the entirety* of the reserves they engaged in that fund to be potentially used to defend the currency of another participating country)
3. Thus a daily total amount of reserves committed to each currency could be computed using the aforementioned methods, without individual inputs from each central bank being revealed). Note that the viewing of the results of these computations can also be restrained so that each central bank only sees the pooling of reserves allocated to him - and not that allocated to others. In this fashion, both inputs and outputs of these forms of computations have modular privacy settings, that can be deployed according to participants preferences.

The previous paragraph described mostly a pooling of reserves, quite similar to what already exists in the Chiang Mai Initiative, but **applied on a continuous and systematic basis rather than just during times of extreme stress** (in fact one of the goals of this automatic and systematic market smoothing is to potentially provide in-commensurable psychological relief and precious time for governments to *avoid* times of extreme stress). 

There are also **other benefits to having a common multicurrency account: first, the mechanisms derived to stabilize a currency vs the international currencies part of the reserves portfolio can now also be used to also stabilize more exotic currency pairs** (but among natural trading partners) such as the MYR/IDR. 

Furthermore, **our scheme would constitute an implementation of the "optimal capital controls**, that should lean against the wind by requiring a temporary tax on inflows and a subsidy on outflows (if dealing with sudden inflows, the opposite if dealing with a sudden stop)" from Farhi and Werning (2013).

Finally, it would **help by design including more currencies in the global reserve distribution and alleviating the "safe asset shortage"** (Caballero, Farhi, Gourinchas, 2017).


```python
# We initialize here the recording vectors that will collect the history of the simulation, to plot the graphs at the end of this notebook

endowments_reserves_history = zeros(number_of_countries,number_of_rounds); %The records of how much cakes in total each country has accumulated at each round (see cell just below for the definition of a cake)
endowments_debts_history = zeros(number_of_countries,number_of_rounds); %The records of how much cakes (ie debts) in total each country has generated up to round t (see cell just below for the definition of a cake)
sum_cakes_history = zeros(1,number_of_rounds); %The records of each country's cake size for each round (see cell just below for the definition of a cake)
sum_of_generated_cakes = 0; %for cumulated

abso_speed_history = zeros(number_of_countries,number_of_rounds); %The records of the eating speed of each country for each round (see cell just below for the definition of the eating speed)
abso_history = zeros(1,number_of_rounds); 
sum_of_abso_speed = 0; %for cumulated

devaluation_history = zeros(number_of_countries,number_of_rounds); %The records of the cumulated number of times which each country devalued up to round i
ranking_history = zeros(number_of_countries,number_of_countries); %The records of the order in which each country ranked other countries' cake to be eaten at each round(see cell just below for the definition of a cake)
history_counter = ones(number_of_countries,1); %used in which round to determine sizes of generated cakes and cake eating speeds (see within round cell below)
deval_history = zeros(number_of_countries,1); %idem

duration_T_updated_history = zeros(1,number_of_rounds); %The records of how long was the timer for each round (see cell just below for the definition of a timer)

```


# Annexes 

--
### First the code for the graphs in part I, then in cells below these first code cells the code for the graphis in part II, then the code for the counterfactuals and simulations 1945-now



```python
# We initialize here the intermediary parameters that will be used within each round

endowments = zeros(number_of_countries,number_of_countries); % Where countries store what "cakes" (debts) they ate during each round. At the end of each round a country's cake that hasn't been totally eaten will decrease the parts of all reserves that contained pieces of cakes (from all previous rounds, not just this round) from that country (it's a devaluation - and we record it in deval_history = deval_history + 1). Else if the cake has been totally it counts as a success and we record it in history_counter = history_counter + 1 
abso_speed = 100.*rand([number_of_countries,1]); % The eating speed of the countries - here initialized at random. During the rest of the game these speed will evolve depending on the history_counters and devaluation_counters of each country
abso_speed_init = abso_speed;

initial_pos = 100.*rand([number_of_countries,1]); % Cakes generated by each country, initialized at random. Then at the start of each round the size of cakes being generated by each country are function of how safe this country is (history_counter - deval_history) plus a random number different for each country (see further in the code)
initial_pos_init =initial_pos;
initial_pos_round = initial_pos;
cakes_from_previous_round = initial_pos; 

duration_T = 1; % There's a timer for each rouund. A round ends when this timer ends, or when countries ate all the cakes if faster than the timer (the timer changes at each round depending on the total cake sizes and total eating speed ratio, so that it increases rather steadily)
fraction_ranking = (1/3); % Used for calibration
duration_T_updated = duration_T;


successfully_loaded_cake_last_round = zeros(number_of_countries,1);
```


```python
# random initialization of ranking between countries, before it is impacted by trade preference and readjusted within each rounds
ranked_list = zeros(number_of_countries,number_of_countries);

for j=1:number_of_countries
    ranked_list(j,:) = randperm(number_of_countries);
end
```


```python
# Initialization of trade preference, and impact on ranking among countries just defined above.
% NOTE THAT THESE CAN BE PLAYED AROUND, AND CALIBRATED AS IN THE 1945-NOW Notebook !!! 

trading_preferences = ceil(abs(full(sprandsym(number_of_countries,uni)))); %NOTE THAT IN MATLAB FULL CODE IS 
%trading_preferences = ceil(abs(full(sprandsym(number_of_countries,uni,rc,2)))); with rc discussed in the intro, for unequality in initial distribution

for k=1:number_of_countries
% we first find a country's preferred trading partners and rank them among themselves

    [~,trading_order]=sort(trading_preferences(k,:).*(ones(1,number_of_countries)+endowments(k,:)),'descend'); %we rank by first trade preference, then by the size of trading partners. Note that this is modelled more finely in the 1945-now simulation notebook 
    % the 1945-now version : 
    %[~,trading_order]=sort(trading_preferences(k,:).*(ones(1,number_of_countries)+max(0,successfully_loaded_cake_last_round(k,1).*(history_counter(k,1)-deval_history(k,1)).*endowments(k,:)*(interest_rate(k,1)))),'descend');
        
    
    % then we adjust the country's rankings by moving these trading partners up the list
    res=sum(trading_preferences(k,:)~=0);
    
    if res>0
        for l=1:res
            ressort_count=find(ranked_list(k,:)==trading_order(l));
            if ressort_count>l
                for m=1:(ressort_count-l)
                    ranked_list(k,ressort_count+1-m)=ranked_list(k,ressort_count-m);
                end
                ranked_list(k,l)=trading_order(l);
            else
            end
        end
    end
    
end
ranked_list_true_init = ranked_list %print this ranking matrix so that you can see; each line i is the ranking list of a country i, from top priority left to last choice right. 
```


```python
# Now we go into rounds of cake eating, that are looped over. Everything important happens in this cell !


for i=1:number_of_rounds
    
    cakes = max(0,successfully_loaded_cake_last_round.*(history_counter-deval_history)+rand([number_of_countries,1]));
    abso_speed = max(0.1,(history_counter-deval_history)+rand([number_of_countries,1]));
    % At the start of the round cakes (ie debt) are generated by each country, and each country is assigned a new eating speed, both depending only on how successful it history is in getting its debt absorbed.
    % Plus we just add a bit of random perturbations to make it more realistic. But very simple model here, that is made more sophisticated in the other simulations (see the two other notebooks

    %we record all of this for graphs later
    cakes_from_previous_round = cakes; 
    sum_of_generated_cakes = sum_of_generated_cakes + cakes;
    sum_of_abso_speed = sum_of_abso_speed + abso_speed;
    abso_history(1,i)=sum(abso_speed);
    sum_cakes_history(1,i)=sum(cakes);
    initial_pos_round = cakes;
    
    % The counter of a round is set up as the max cake size generated at this round
    duration_T_updated = max(1,max(cakes));
    
    % We initialize the counting
    time_counter=0;
    cakes_counter=0;
    rank_counter = ones(number_of_countries,1);
    removed_cake_row = zeros(number_of_countries,1);
    k=1;
    latest_finished_cake = 0;
    will_be_totally_consumed = zeros(number_of_countries,1);
    
    % And the countries start eating ! Until all the cakes are eaten or the counter is down to zero.
    while (duration_T_updated>0 && cakes_counter<number_of_countries) 
    
        initial_pos_updated = cakes;
        diff_between_wished_and_offered = zeros(number_of_countries,1);
        
        % We go through the preference list of all the countries - if the cake item at the top of each country's remaining list is still there they'll eat it, else we move down an item in that country's list
        % For that we first figure out which cake pieces are sought after by the most countries x their eating speed
        for l=1:number_of_countries
            if removed_cake_row(ranked_list(l,1))>0
                o=1;
                u=1;
                if  removed_cake_row(ranked_list(l,o+1),1)>0
                    u=o+1;
                    while ((u<(number_of_countries-1)) && (removed_cake_row(ranked_list(l,u+1),1)>0))
                        u=u+1;
                    end
                    ranked_list(l,o)=ranked_list(l,u+1);
                else
                    ranked_list(l,o)=ranked_list(l,o+1);
                end
                rank_counter(j,1)=rank_counter(j,1)+1;
            end
        end
        
        for j=1:number_of_countries
            if removed_cake_row(j,1)>0
            else
                if sum(abso_speed(ranked_list(:,1)==j))>cakes(j,1)
                    will_be_totally_consumed(j,1)=will_be_totally_consumed(j,1)+1;
                    diff_between_wished_and_offered(j,1) = sum(abso_speed(ranked_list(:,1)==j))/initial_pos_updated(j,1);
                end
            end
        end
        
        if sum(diff_between_wished_and_offered)==0
            for j=1:number_of_countries
                if removed_cake_row(j,1)>0
                else
                    diff_between_wished_and_offered(j,1) = sum(abso_speed(ranked_list(:,1)==j))/initial_pos_updated(j,1);
                    will_be_totally_consumed(j,1)=will_be_totally_consumed(j,1)+1;
                end
            end
        else
        end
        
        % Now that we know which cake pieces are sought after by which countries x their eating speed we can sort them 
        [~,consumption_order]=sort(diff_between_wished_and_offered,'descend');
        
        % Just some safety checks 
        if sum(diff_between_wished_and_offered)==0
            [ii,jj]=find(~removed_cake_row);
            if size(ii)==1
                consumption_order(1)=ii;
            else
                for j=1:size(ii)
                    consumption_order(j)=ii(j);
                end
            end
        else
        end
        
       
       % Now we know which cake will be eaten ! 
       % Let's share it across countries according to their eating speed - we move these to the relevant slots in the endowments matrix.
        
       % With just a special attention if the cake piece being eaten won't be finished in time (the "else" to this "if" condition)
        if (duration_T_updated-cakes(consumption_order(1),1))>0
            duration_T_updated = duration_T_updated - cakes(consumption_order(1),1);
            for j=1:number_of_countries
                if ranked_list(j,1)==consumption_order(1)
                    endowments(j,consumption_order(1)) = endowments(j,consumption_order(1))+(abso_speed(j,1)./(sum(abso_speed(ranked_list(:,1)==consumption_order(1)))))*initial_pos_updated(consumption_order(1),1);
                elseif cakes(ranked_list(j,1),1)==0
                    removed_cake_row(ranked_list(j,1),1)=removed_cake_row(ranked_list(j,1),1)+1;
                else
                    endowments(j,ranked_list(j,1)) = endowments(j,ranked_list(j,1))+(abso_speed(j,1)*cakes(consumption_order(1),1))/(sum(abso_speed(ranked_list(:,1)==consumption_order(1))));
                    cakes(ranked_list(j,1),1)=initial_pos_updated(ranked_list(j,1),1)-(sum(abso_speed(ranked_list(:,1)==ranked_list(j,1)))*cakes(consumption_order(1),1))/(sum(abso_speed(ranked_list(:,1)==consumption_order(1))));
                end
            end
            time_counter = time_counter + cakes(consumption_order(1),1);
            cakes(consumption_order(1),1) = 0;
            removed_cake_row(consumption_order(1),1)=removed_cake_row(consumption_order(1),1)+1;
            
             % With just a special attention if the cake piece being eaten won't be finished in time (the "else" to this "if" condition)
        else
            cakes(consumption_order(1),1) = cakes(consumption_order(1),1) - duration_T_updated;
            time_counter = time_counter + duration_T_updated;
            for j=1:number_of_countries
                if ranked_list(j,1)==consumption_order(1)
                    endowments(j,consumption_order(1)) = endowments(j,consumption_order(1))+(abso_speed(j,1)./(sum(abso_speed(ranked_list(:,1)==consumption_order(1)))))*duration_T_updated;
                elseif cakes(ranked_list(j,1),1)==0
                    removed_cake_row(ranked_list(j,1),1)=removed_cake_row(ranked_list(j,1),1)+1;
                else
                    endowments(j,ranked_list(j,1)) = endowments(j,ranked_list(j,1))+(abso_speed(j,1)*duration_T_updated)/(sum(abso_speed(ranked_list(:,1)==consumption_order(1))));
                    cakes(ranked_list(j,1),1)=cakes(ranked_list(j,1),1)-(abso_speed(j,1)*duration_T_updated)/(sum(abso_speed(ranked_list(:,1)==consumption_order(1))));    
                end
            end
            duration_T_updated = 0; 
        end
        latest_finished_cake = consumption_order(1);
        
        cakes_counter = cakes_counter + 1;
        k=k+1;
        duration_T_updated_history(1,i)=duration_T_updated;
    end
    
    
    % At the end of a round we devalue all countries that didn't manage to get all its debt absorbed during this round, proportionally to how much of it is left at the end of the round
    for j=1:number_of_countries
        if (initial_pos_round(j,1)-cakes(j,1))>0
            endowments(:,j)=endowments(:,j)*((initial_pos_round(j,1)-cakes(j,1))/initial_pos_round(j,1));
        else
        end
        if cakes(j,1)==0
            history_counter(j,1) = history_counter(j,1) + 1;
            successfully_loaded_cake_last_round(j,1) = 1;
            interest_rate(j,1)=interest_rate(j,1)./(1+rand(1,1));
        else
            interest_rate(j,1)=min(1,max(interest_rate_history(j,1),interest_rate(j,1).*(1+rand(1,1))));
            deval_history(j,1) = deval_history(j,1)+1 ;
        end
    end
    
   
   % And we update the ranking list for each country after the events of this round, in a similar fashion as what happened initially on the cell just above on this notebook.
   [~,success_order]=sort(history_counter,'descend');
   ranked_list = repmat(success_order',number_of_countries,1);
   
   for k=1:number_of_countries    
       r1 = randperm(number_of_countries,2*round(number_of_countries*fraction_ranking));
       for j=1:round(number_of_countries*fraction_ranking)
           inter=ranked_list(k,r1(1,j));
           ranked_list(k,r1(1,j))=ranked_list(k,r1(1,2*j));
           ranked_list(k,r1(1,2*j))=inter;
       end
   end
   
   for k=1:number_of_countries
       [~,trading_order]=sort(trading_preferences(k,:).*(ones(1,number_of_countries)+max(0,successfully_loaded_cake_last_round(k,1).*(history_counter(k,1)-deval_history(k,1)).*endowments(k,:)*(interest_rate(k,1)))),'descend');
       res=sum(trading_preferences(k,:)~=0);
       if res>0
           for l=1:res
               ressort_count=find(ranked_list(k,:)==trading_order(l));
               if ressort_count>l
                   for m=1:(ressort_count-l)
                       ranked_list(k,ressort_count+1-m)=ranked_list(k,ressort_count-m);
                   end
                   ranked_list(k,l)=trading_order(l);
               else
               end
           end
       end
       interest_rate_history(k,i) = interest_rate(k,1);
   end
   ranked_list_init = ranked_list; 
   endowments_reserves_history(:,i) = sum(endowments,2);
   endowments_debts_history(:,i) = sum(endowments,1)';
   abso_speed_history(:,i) = abso_speed;
   devaluation_history(:,i) = deval_history;
   ranking_history(:,:,i) = ranked_list_init;
end
```

### That was the core of the simulation code ! Now one can just plot everything

So the graphs can either be all in one cell, or be plot individually one per cell. I'll let the reader copy paste the relevant pieces of code accordingly, that can be put in a following single cell as shown for example below.

*Also note that the digraph function used to plot the graph of the trade preferences among countries is not implemented yet in Octave. So the code is provided here but won't produce this specific graph.


```python
sum_ranking_history = zeros(number_of_countries,number_of_rounds);
i=1;
for j=1:number_of_countries
    tag{j}=strcat('country ',num2str(j));
    for k=1:number_of_countries
        [~,indexes]=sort(ranking_history(k,:,i));
        score_for_one_country = ((number_of_countries+1)*ones(1,1)-indexes);
        sum_ranking_history(j,1) = sum_ranking_history(j,1)+score_for_one_country(1,j);
    end
end
sum_ranking_history_b = sum_ranking_history;

for i=2:number_of_rounds
    for j=1:number_of_countries
        for k=1:number_of_countries
            [~,indexes]=sort(ranking_history(k,:,i));
            score_for_one_country = ((number_of_countries+1)*ones(1,1)-indexes);
            sum_ranking_history(j,i) = sum_ranking_history(j,i)+score_for_one_country(1,j);
        end
    end
    sum_ranking_history(:,i)=(sum_ranking_history(:,i)+sum_ranking_history(:,i-1));%./(mean(sum_ranking_history(:,i-1)));
    sum_ranking_history_b(:,i)=sum_ranking_history(:,i)-sum_ranking_history(:,i-1);%./(mean(sum_ranking_history(:,i-1)));
end

figure;
A=trading_preferences;
G = digraph(A);
LWidths = 5*G.Edges.Weight/max(G.Edges.Weight);

subplot(2,3,1);
plot(G,'LineWidth',LWidths)
title('Trade preferences among 6 (numbered) countries graph')


subplot(2,3,2);
plot(interest_rate_history')
title('Interest rate history')
%legend(tag)
    
subplot(2,3,3);
plot(abso_speed_history')
title('Cake eating speed history')
%legend(tag)

subplot(2,3,4);
plot(sum_ranking_history_b')
title('Ranking history by country')
legend(tag)

subplot(2,3,5);
plot(endowments_debts_history')
title('Cumulated debts generated by country history')
%legend(tag)

subplot(2,3,6);
plot(endowments_reserves_history')
title('Cumulated reserves by country history')
%legend(tag)
```


Draft that might be deleted
--
### Safe asset shortage or financial cycle buildup - the two sides of the same (anchor-) coin ?

**In fact, the global loosening of the monetary anchoring** (no rules determines how much USD can or should be printed to optimize the global economy) **might even be a driver of the secular decline in global real interest rates over much of the past 30 years**. However, while there are now several competing theories aiming at explaining this "secular stagnation", none of them explicitly examines how the anchoring of the international monetary system might (or might not) have played a role in causing this trend. 

**That is why we will try to provide here a framework based on modelling the anchoring as a mechanism design problem**, to explicit parameters that changed between now and the Gold Standard, before/after 1971, and which might provide a framework linking the safe asset shortage view of today's monetary anchoring, to Borio's financial cycle buildup warning (a possible consequence of the more flexible anchoring). **Such a framework would also allow to explore the different conditions under which yield curve control by the Fed would work without raising inflation, conditions which would lead to parallel financial systems to emerge, and conditions which might lead to Triffin events (and how they would unfold).**


--
### The link with the Safe Asset Shortage hypothesis, and Borio's financial cycle build up hypothesis 

From the parameters of the cake eating model below, and they interact with each other, we can attempt to draw a few parallels with the competing hypothesis of Caballero, Farhi and Gourinchas, and of Borio. 

In fact, let's first note how the cake-eating model itself **is based** off scarcity - indeed if central banks *could* absorb all imbalances and debt at each round then in our model there would no default, no devaluation, and all assets would be considered safe. However given the limited *duration* parameter *(see the parameter duration_T_updated_history introduced below, noting the records of how long was the timer for each round. A round ends when this timer ends, or when countries ate all the cakes if faster than the timer, with the timer changing at each round depending on the total cake sizes and total eating speed ratio, so that it increases rather steadily)*, only the countries that first manages to "offload" their debts avoid devaluation and maintain a "safe" reputation. 

Second, let's note how the two parameters of how much cakes (ie debts) each country is generating, and how much cakes each country can absorb, at each round, are proxies of how developed/stretched a country's financial system is. One can note how past history of safety in a country can lead to an expanding emission/absorption cycle, which might eventually burst à la Minsky, related to Borio's hypothesis.

Hence two scenarii : one in which a few safe countries' debts are pursued in higher demand than what they emit (safe asset shortage), which lowers the interest rate. But this scarcity only incentivizes them to stretch more their financial systems so that they both emit and absorb more pieces of cake. Up until a situation in which they emitted too much pieces of cake compared to the demand, in which case they suffer a devaluation requiring them to either emit less pieces of cake, absborb more of their own (through decreased interest rate as described by Borio), or convince more countries to absorb theirs first. 

*NB : explore how this could be linked back to Caballero, Farhi and Gourinchas' IS-LM equations*


```python

```
