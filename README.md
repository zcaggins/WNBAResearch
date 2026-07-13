# WNBA Expansion Database

Reference notes on the WNBA expansion process, historical teams, and candidate-city profiles.

- **Visual board (flowchart + editable tables):** https://miro.com/app/board/uXjVH88ACHY=/
- **Spreadsheet version:** `WNBA_Expansion_Database.xlsx` (see chat)
- **Raw data (CSV, one file per table):** [`/data`](./data)
- **Charts (PNG):** [`/charts`](./charts)

> Population figures are metro-area estimates and arena capacities are basketball
> configurations; both are approximate. Current as of mid-2026.

## Putting this on GitHub

This folder is already laid out as a repo — `README.md` at the root, data in `/data`,
images in `/charts`. From this folder:

```bash
git init
git add .
git commit -m "WNBA expansion research"
gh repo create wnba-expansion-database --public --source=. --push
# no GitHub CLI? create an empty repo on github.com first, then:
# git remote add origin https://github.com/<you>/wnba-expansion-database.git
# git branch -M main
# git push -u origin main
```

Once pushed, GitHub renders this README with working tables and inline images automatically —
no extra setup needed. To edit any table, open the `.md` or `.csv` files in VS Code; GitHub
diffs both cleanly. The Miro board is not a file, so it can't live in the repo — link to it
from the README instead (already done above), or export a board snapshot as an image if you
want a static copy checked into git.

## Charts

![Population vs arena capacity](./charts/candidate_cities_population_vs_arena.png)

![Expansion fee growth](./charts/expansion_fee_growth.png)

![Team count growth](./charts/team_count_growth.png)

---

## 1. Expansion Process (WNBA)

| Step | Stage | What Happens | Typical Timeframe |
|---|---|---|---|
| 1 | League signals openness | WNBA leadership/Board of Governors states it will consider new markets, tied to a target team count. | Years ahead of first tip-off |
| 2 | Bid window opens | League sets a deadline; ownership groups file applications covering financing, arena, market data. | Weeks to a few months |
| 3 | League evaluates bids | Scored on ownership strength, arena/practice facility readiness, corporate & media support, women's sports track record. | Several months |
| 4 | Board of Governors votes | NBA and WNBA owners jointly vote to approve specific cities and ownership groups. | One vote; 2-4 yrs lead time to debut |
| 5 | Expansion fee paid | New owners pay the league a lump fee. Risen from $50M (2025) to $250M (2028-30). | Paid on/after approval |
| 6 | Front office stands up | Team hires GM, coach, business ops staff; secures practice facility and arena lease. | 1-3 years before debut |
| 7 | Expansion draft | Existing teams protect a set number of players; new team(s) draft unprotected players. | Months before first season |
| 8 | WNBA Draft allocation | New team participates in the next college draft, typically without the very top pick. | Spring before first season |
| 9 | Inaugural season | Team debuts; league monitors attendance/ratings/revenue to inform future expansion. | Year 1 |

---

## 2. NBA vs WNBA Expansion Comparison

| Dimension | WNBA | NBA | Key Difference |
|---|---|---|---|
| Governing vote | Joint NBA+WNBA Board of Governors (NBA owns ~42% of WNBA) | NBA Board of Governors alone; 23 of 30 owners must approve | WNBA expansion is co-governed by the NBA, not fully independent |
| Recent expansion fees | $50M (2025) → $115-125M (2026) → $250M (2028-30) | Expected $7-10B per team (Seattle/Las Vegas, 2026) | NBA fees are ~30-40x larger; WNBA fees growing far faster percentage-wise |
| Arena bar | Originally 7,000 seats; now wants 10,000+ | Requires top-tier 17,000-20,000+ seat arena | WNBA more flexible on venue size, often shares an NBA arena |
| Ownership structure | Individuals, investor groups, or the local NBA owner | Controlling owner needs ≥15% stake; PE capped at 20%/team, 30% combined | NBA has more codified ownership rules given far larger deal sizes |
| Draft mechanism | Expansion draft: teams protect ~6 players | Expansion draft: teams historically protect up to 8 | Similar mechanism; NBA lets incumbents protect more |
| Sister-team pattern | Many teams share ownership/arena with an NBA team (Valkyries/Warriors, Fever/Pacers) | N/A - NBA is the anchor franchise | WNBA expansion often piggybacks on existing NBA infrastructure |
| Selection criteria emphasis | Market viability, ownership commitment, fan/corporate/media support, community commitment to women's sports | Market revenue potential, arena readiness, ownership financial strength | WNBA weighs community commitment explicitly; NBA criteria are almost purely financial |
| Typical lead time | 2-4 years between award and first tip-off | Historically 1-2 years; 2-3 yrs for 2028-29 target | Comparable lead times once a formal vote occurs |

---

## 3. Historical WNBA Expansion Teams (1997-2025, Pre-2026 Wave)

| Year | Team | City | Outcome to Date | Expansion Fee |
|---|---|---|---|---|
| 1997 | Original 8 franchises | Multiple | 3 remain (Liberty, Sparks, Mercury) as of 2026 | N/A - league founding |
| 1998 | Detroit Shock / Washington Mystics | Detroit, MI / Washington, DC | Shock relocated twice, now Dallas Wings; Mystics still active | N/A |
| 1999 | Minnesota Lynx / Orlando Miracle | Minneapolis, MN / Orlando, FL | Lynx still active; Miracle → Connecticut Sun (2003) → Houston (2027) | N/A |
| 2000 | Fever / Sol / Fire (orig.) / Storm | Indianapolis / Miami / Portland / Seattle | Fever & Storm active; Sol and original Fire folded (2002/2003) | N/A |
| 2006 | Chicago Sky | Chicago, IL | Still active | N/A |
| 2008 | Atlanta Dream | Atlanta, GA | Still active | N/A |
| 2024 | Golden State Valkyries | San Francisco Bay Area, CA | Active, debuted 2025; league's most valuable franchise within a year | $50 million |

---

## 4. Secured 2025-2030 Teams

| Debut Year | Team/City | Ownership | Expansion Fee | Arena | Notes |
|---|---|---|---|---|---|
| 2025 | Golden State Valkyries - Bay Area, CA | Joe Lacob, Peter Guber, Warriors ownership | $50 million | Chase Center | 13th franchise; most valuable team within a year |
| 2026 | Toronto Tempo - Toronto, ON | Kilmer Sports Ventures (Larry Tanenbaum) | $115 million | Coca-Cola Coliseum + 3 other venues | First WNBA team outside the U.S. |
| 2026 | Portland Fire - Portland, OR | Bhathal family (RAJ Sports) | $125 million | Moda Center | Revives Fire name from folded 2000-02 franchise |
| 2027 | Houston (relocated from CT Sun) | Fertitta family (Rockets ownership) | $300 million (purchase) | Toyota Center (TBD) | Relocation, not new expansion; revives former Comets market |
| 2028 | Cleveland (Rockers trademarked) | Dan Gilbert (Cavaliers) | $250 million | Rocket Arena | Revives 1997-2003 Cleveland Rockers market |
| 2029 | Detroit (Shock trademarked) | Tom Gores (Pistons) | $250 million | Little Caesars Arena | Revives 1998-2009 Detroit Shock market |
| 2030 | Philadelphia (name pending) | Harris, Blitzer, Adelman, Roberts (76ers/HBSE + Comcast) | $250 million | New South Philadelphia arena | Philadelphia's first-ever WNBA franchise |

---

## 5. Candidate Cities for Future WNBA Expansion

Rows 1-9 formally bid in the Jan. 2025 window but were not awarded a team; per the WNBA,
these markets retain priority over cities that did not bid (e.g. Boston). Row 10 (Louisville)
and Row 11 (Mexico City) did not file formal bids but are frequently discussed as future
markets - Louisville via local advocacy, Mexico City as a speculative international market.

| City | Metro Pop. (approx.) | NBA Team? | Prior WNBA History | Ownership Backing | Arena | Capacity (approx.) | New Facility Needed? | Tourist Draws | Food & Dining | Women's Sports Fan Signal | Bid Status | Notes |
|---|---|---|---|---|---|---|---|---|---|---|---|---|
| Charlotte, NC | 2,800,000 | Yes | Charlotte Sting (1997-2006) | Hornets Sports & Entertainment (NBA-backed) | Spectrum Center | 19,000 | No | NASCAR Hall of Fame, US National Whitewater Center, Uptown | Strong Southern food/BBQ scene | Sting alumni fan base; NBA-owner backing | Formal bid, not chosen | One of only two rejected bids backed by an NBA owner |
| Denver, CO | 3,000,000 | Yes | No prior team | Local investors (not Nuggets ownership) | New arena proposed | 10,000 | Yes | Rocky Mountain access, Red Rocks, outdoor tourism | Nationally known craft beer scene | Strong Title IX/college sports culture | Formal bid, not chosen | Bid was independent of Nuggets ownership |
| Austin, TX | 2,500,000 | No | No prior team | Group incl. investors close to Kevin Durant | Moody Center (UT Austin) | 11,000 | No | SXSW, Live Music Capital, Barton Springs | Renowned food-truck/live-music dining culture | Large young population, strong UT culture | Formal bid, not chosen | Biggest handicap: no NBA team/ownership in-market |
| Nashville, TN | 2,100,000 | No | No prior team | Bill Haslam, Candace Parker, Peyton Manning | Bridgestone Arena / proposed venue | 10,000 | Possible | Music Row, Grand Ole Opry, honky-tonk district | Famous hot chicken/live-venue dining scene | Proposed name 'Summitt' honoring Pat Summitt | Formal bid, not chosen | Star power did not overcome lack of NBA tie-in |
| Kansas City, MO | 2,200,000 | No | No prior team | Group incl. Patrick Mahomes | T-Mobile Center | 18,500 | No | WWI Museum, BBQ culture, Union Station | Nationally known BBQ scene | Framed as 'no-brainer' given WNBA's success | Formal bid, not chosen | Lacks an NBA team in-market |
| St. Louis, MO | 2,800,000 | No | No prior team | Group incl. Jayson Tatum (St. Louis native) | Enterprise Center | 19,000 | No | Gateway Arch, City Museum | Strong Midwestern dining/BBQ scene | Hometown-star-driven bid | Formal bid, not chosen | No NBA team in-market is a structural disadvantage |
| Miami, FL | 6,300,000 | Yes | Miami Sol (2000-02, folded) | Independent group (not Heat ownership) | Kaseya Center | 19,600 | No | South Beach, Art Basel, cruise-port tourism | Internationally known dining/nightlife scene | Large Latin American fan base, no incumbent base since Sol folded | Formal bid, not chosen | Heat ownership was not involved in this bid |
| Jacksonville, FL | 1,700,000 | No | No prior team | Not widely publicized | VyStar Veterans Memorial Arena | 15,000 | Possible | Beaches, riverfront, NFL Jaguars fandom | Growing Southern food scene | Smaller media market than other bidders | Formal bid, not chosen | Least-publicized of the 9 bids |
| Milwaukee, WI | 1,600,000 | Yes | No prior team | Not widely publicized | Fiserv Forum | 17,500 | No | Harley-Davidson Museum, lakefront, brewing heritage | Strong beer/brewery, Midwestern food culture | Lower profile bid relative to others | Formal bid, not chosen | Smallest metro population among the 9 formal bidders |
| Louisville, KY | 1,400,000 | No | No prior team | No group secured; Mayor Craig Greenberg has lobbied the league | KFC Yum! Center | 22,000 | No | Kentucky Derby, Louisville Slugger Museum, bourbon trail | Nationally known bourbon/Southern dining scene | Top-5 nat'l women's college basketball attendance for over a decade; also home to Racing Louisville (NWSL) | No formal bid / advocacy only | Did not file a formal Jan. 2025 bid; smallest market/lowest per-capita income, but genuine arena and fan-base strengths |
| Mexico City, Mexico | 22,000,000 | No (G League Capitanes) | No prior team | No group publicly identified; not part of the Jan. 2025 round | Arena CDMX | 22,300 | No | Zocalo/historic center, Teotihuacan, Chapultepec Park | One of the world's top culinary capitals | Growing (Liga MX Femenil rising), but no dedicated WNBA/pro women's basketball base | No formal bid / advocacy only | Metro larger than any current NBA/WNBA market; NBA has hosted games there since 1992, G League team since 2020; cross-border travel/visa/broadcast logistics are the real hurdle - Toronto Tempo (2026) is the first non-U.S. test case |

---

## Sources

WNBA/NBA official announcements, Sports Business Journal, ESPN, ex-athletic reporting,
ProLeague coverage of the Jan. 2025 bidding round, and local coverage of Louisville's
advocacy efforts (BetKentucky, LEO Weekly). Current as of mid-2026 — re-verify before
using for decision-making.

