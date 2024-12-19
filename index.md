---
layout: home
title: Annabel's story
subtitle: The way of the data analyst
---

Annabel, a young data analyst, has just joined a major American film studio preparing to release a range of new movies in 2025. After several disappointing box-office results in recent years, the CEO wants to maximize the chances of success by identifying ideal release periods along with what kind of movies are the most popular, and therefore profitable. By analyzing historical trends and patterns, Annabel’s job is to advise on the best release timing for each upcoming movie while also pinpointing the key factors that make movies popular. Her findings ultimately reveal a deeper truth about how movies evolved over time.


**What Drives Movie Success: Genres, Themes, or Release Timing?**
To guide her analysis effectively, Annabel considers which factors contribute most to a movie’s success. Taking the perspective of a producer focused solely on maximizing revenue, she chooses to evaluate success based on profitability, measured as the ratio of box office revenue to production budget. This approach reflects financial success regardless of audience appreciation, which isn’t always a reliable indicator in today’s market (as seen with recent Star Wars episodes).


Note: We assume that the dataset is representative of the movie industry in terms of genre distribution, meaning no specific genre is disproportionately underrepresented in any given year. However, the overall number of movies in the dataset may not be evenly distributed across time, as older movies (e.g., from 100 years ago) are less likely to be included compared to more recent releases. This does not imply that fewer movies were produced in the past.


After merging data from multiple sources, cleaning and handling it, Annabel is left with movie records spanning over 100 years. She wonders whether including such old data is meaningful and won't harm her analysis, given how much society has evolved over time. Factors like movie runtimes, peak release months, popular genres, and dominant themes may have changed significantly. For example, early films often had shorter runtimes due to technological limitations, while genres like superhero movies only gained popularity in recent decades.


However, first, she asks herself if there is anything to analyze to draw conclusions on.


<figure class="plot1">
    <img src="assets/img/plot1.png" alt="My Plot 1">
    <figcaption>Figure 1: A visualization of my data number 1.</figcaption>
</figure>

Annabel then introduced Figure 2: Long-Term Trends in Median Profitability and Success Rate, placing it after the monthly and seasonal analyses. While the previous figures highlighted tactical considerations—such as which months or seasons might be more favorable—this plot provided a broader, long-term perspective.
<figure class="plot2">
    <img src="assets/img/plot2.png" alt="My Plot 2">
    <figcaption>Figure 2: Long-Term Trends in Median Profitability and Success Rate.</figcaption>
</figure>
By examining trends over the last century, the figure indicated that film profitability and success rates have generally declined compared to earlier eras. In other words, though certain months or seasons may still stand out, the overall environment has grown more challenging for producing profitable films. Within the most recent 20-year span, the data suggested a leveling-off of this decline, hinting that the industry may have reached a new baseline—less prosperous than the mid-20th century, but relatively stable.

This historical context helps interpret the earlier findings. The information on monthly and seasonal patterns must be understood within an industry framework where achieving profitability has become increasingly difficult. While timing can still influence a film’s financial outcome, the long-term trends make it clear that studios must consider not only the immediate patterns identified in previous figures but also the broader shifts in market conditions and profitability over time.


Annabel began her analysis by examining the fundamentals: how does profitability vary month by month, without yet accounting for historical shifts or seasonal groupings over time? To address this, she introduced Figure 1: Profitability Per Month in her report. This figure presents boxplots of profitability for each month, enabling readers to see the central tendencies, variability, and the presence of unusual values (outliers) in a straightforward, comparative manner.
<figure class="plot3">
    <img src="assets/img/plot3.png" alt="My Plot 3">
    <figcaption>Figure 3: Profitability Per Month.</figcaption>
</figure>
Looking closely at the figure, one can discern notable patterns. Some months, such as June or December, show a higher median profitability, represented by a taller box and median line situated at a relatively elevated position on the y-axis. This suggests that, on average, films released in these months tend to achieve better returns. However, these months also exhibit a larger spread of values and more outliers, implying a greater degree of unpredictability—while many films do well, a few may significantly overperform, skewing the distribution. Other months, like January or March, have slightly lower medians and more compact interquartile ranges. This tighter grouping indicates that while results may be more modest, they are also more consistent, with fewer extreme outcomes.

Additionally, the number of data points (indicated by "n=" above each box) varies, reflecting industry behaviors. Months with a higher volume of releases may show more dispersion, as a greater variety of films—from low-budget indies to tentpole blockbusters—enter the market. This influences not just central profit tendencies but the overall shape of the distribution

By analyzing these boxplots, Annabel can identify months that historically yield steadier results versus those offering the potential for higher peaks but also larger risks. This initial examination lays the groundwork for her subsequent figures and analyses, which delve into how these patterns evolve over decades or shift when aggregated into seasons. Understanding the month-by-month baseline is crucial before exploring longer-term trends and more complex scheduling considerations.


Annabel’s analysis reached a critical juncture once she compiled historical profitability data by month and grouped it by season over multiple decades. Up to this point, she had discussed the importance of timing in movie releases, examined correlations between genre and seasonal trends, and highlighted how cultural events influenced audience turnout. Now, she needed to present concrete evidence of how these patterns had evolved over time.

This is where Figure 4: Monthly Profitability Distribution by Season Across Decades is introduced, placed after the initial descriptive analysis of overall seasonal shifts. The figure consists of four panels—one for each season—displaying how each month’s share of profitable outcomes has changed over successive decades. By examining these lines, one can observe long-term trends, such as the gradual strengthening of certain winter months or the periodic rises and falls in summer profitability.
<figure class="plot4">
    <img src="assets/img/plot4.png" alt="My Plot 4">
    <figcaption>Figure 4: Monthly Profitability Distribution by Season Across Decades.</figcaption>
</figure>
Annabel would present the figure immediately following her general overview of seasonal tendencies. Prior to showing it, she briefly discusses the methodological approach: how profitability percentages were calculated per decade, how months were assigned to seasons, and why focusing on aggregated historical data can provide a more stable reference point than short-term fluctuations.

When decision-makers review Figure 4, they can identify patterns, for example, the sustained growth in spring months or a mid-century decline in certain fall months. Each seasonal panel includes both individual months and the total seasonal trend, aiding in understanding not only the contribution of each month but also the collective seasonal profile.

After the figure, Annabel draws attention to key observations. For instance, she might note that the winter season consistently maintained a relatively stable share, while summer saw significant variability, influenced by evolving industry strategies for blockbuster releases. These insights equip the studio’s planning team with a data-driven foundation to fine-tune their scheduling decisions, ensuring that release dates align more closely with historically proven profitable periods.


After presenting Figure 4, Annabel directed attention to the shifts in profitability and representation across different film genres over time. Unlike the previous figures that focused on seasonal patterns, decades-long trends, or industry-wide profitability, Figure 5 offered a more granular view at the genre level. Each column represented a genre, with the top row illustrating changes in median profitability and the bottom row showing how frequently that genre appeared as a portion of the total film market.
<figure class="plot5">
    <img src="assets/img/plot5.png" alt="My Plot 5">
    <figcaption>Figure 5: Profitability Trends and Representation by Genre Over Time.</figcaption>
</figure>
From the data, Annabel noted several patterns. Family films, for instance, grew more common over the decades, but their average profitability declined, suggesting that while studios continued producing them, the financial returns gradually diminished. In contrast, war films lost both profitability and representation, indicating that they not only became less profitable over time but also less frequently produced, likely reflecting shifting audience interests and historical contexts.

Romantic films, once a staple, also saw a decrease in both frequency and profitability, pointing to waning audience demand. On the other hand, certain categories showed more positive trends. LGBT films, starting from a smaller base, increased in both representation and profitability, suggesting that as audience tastes and social attitudes evolved, these films found more consistent market success. Action films also expanded their share of the market without a corresponding drop in financial performance, indicating that they remained stable or even slightly improved in terms of returns as they became more common. Superhero films—while more variable—suggest a late emergence, peaking in profitability during certain periods and slowly building representation over time.

By examining these genre-specific trajectories, Annabel established that no single pattern applies universally. Some genres fade, some find steady ground, and others expand into new opportunities. These insights, in combination with earlier findings about months, seasons, and overall profitability trends, provide a detailed map of how audience preferences, market conditions, and cultural factors influence the profitability and prevalence of certain types of films over the long term.


After discussing the long-term patterns shown in Figure 5, Annabel introduced a similar figure focusing on the last 20 years to see how these trends have evolved more recently. Whereas the century-spanning data showed slow, steady changes, this shorter timeframe revealed quicker adjustments and potential turnarounds in certain genres.
<figure class="plot6">
    <img src="assets/img/plot6.png" alt="My Plot 6">
    <figcaption>Figure 1: A visualization of my data number 6.</figcaption>
</figure>
For example, Family films, which had been steadily losing profitability over the long term despite increasing in prevalence, now show rising profits, suggesting that producers may have adapted to audience needs more effectively. War films, previously declining in both profitability and presence, appear relatively stable in representation now, though still less profitable than in earlier decades. Romantic films, once in continuous decline, now seem to have leveled off, indicating that their reduced appeal may have reached a plateau.

LGBT films, which showed promise over the full historical range, appear more variable in the last two decades, hinting that audience acceptance and market strategies are still settling. Action films, already on a stable upward path, continue to hold their ground and remain profitable. Superhero films, late bloomers in the long-term data, now display a clearer upward trend, reflecting better-defined franchises and marketing strategies.

By comparing these recent trends with the longer historical arcs, Annabel demonstrated that while past patterns provide context, contemporary shifts can differ meaningfully. Some genres are adapting and finding renewed profitability, others are stabilizing at lower levels, and a few continue to grow. This shorter-term perspective helps refine current strategic planning, complementing the broader insights gleaned from older historical trends.


As her analysis neared completion, Annabel introduced a new, interactive visualization to complement the static figures presented earlier. After showing long-term patterns, decade-specific shifts, and recent changes in profitability and representation by genre, she now offered an interactive bubble chart focusing on the last 20 years, broken down by release month and filtered by genre. By placing this tool after the previous figures, she allowed stakeholders to drill deeper into the specific conditions that contribute to a film’s financial outcome.
<div class="plot7">
    {% include plot_7.html %}
</div>
In this interactive chart, each bubble represents the median profitability of films released in a particular month for a given genre. Users can adjust the bubble size to reflect different metrics—such as median budget, runtime, or sample size. For instance, a large bubble with a modest median budget might indicate that profitable returns are achievable without massive financial investments, especially if it appears in months previously identified as stable or promising. Conversely, smaller bubbles or those corresponding to large budgets may prompt the viewer to question the return on high-cost productions in certain periods.

This dynamic element of the visualization allows decision-makers to explore multiple dimensions simultaneously. They can compare how Action films fare in early summer versus Family films at year’s end, or see whether a steady uptick in profitability aligns with an increase in sample size. The interactive nature means no single interpretation is fixed; instead, it encourages experimentation, letting users toggle between metrics and genres to find patterns that align with their strategic goals.

By incorporating this interactive bubble chart at this stage in the narrative, Annabel ensured that her readers weren’t just receiving a static overview of historical trends—they were equipped to engage with the data directly. This final step tied together the earlier findings, reinforcing the importance of month-by-month considerations, acknowledging the influence of budget and sample size, and showing how newly emergent patterns in recent decades could inform more nuanced, data-driven release strategies.


Following the introduction of interactive visuals and temporal breakdowns, Annabel next presented a heatmap that linked movie genres to thematic elements. Placed after the previous figures that focused on time-based trends and genre-level profitability, this heatmap offered a different angle: it highlighted how the combination of a film’s genre and underlying theme might influence its financial performance.
<figure class="plot8">
    <img src="assets/img/plot8.png" alt="My Plot 8">
    <figcaption>Figure 1: A visualization of my data number 8.</figcaption>
</figure>
In this visualization, each cell represented a unique genre-theme pairing, with color intensity indicating median profitability. Alongside the profitability values, sample counts were provided in parentheses, giving a sense of how frequently that combination appeared. By examining this matrix, Annabel could identify which themes seemed to resonate strongly with audiences within particular genres. For example, she might notice that “Family” themes performed well in the Family genre but less so in War films, or that “Friendship” consistently correlated with higher profitability across multiple genres—provided there were enough samples to support that observation.

This perspective helped Annabel understand not only when or what type of movies performed well, but also why certain films might stand out. Identifying profitable theme-genre pairs allowed her to connect previous insights—like the decline in certain genres or the rise in others—to the narrative and emotional elements that drive audience engagement. If a particular theme thrived in a stable or upward-trending genre, it suggested opportunities for studios to develop content more aligned with those favored combinations.

In the context of her broader story, this heatmap represented another layer of detail, following the earlier analyses of timing, long-term trends, and genre-specific shifts. By adding thematic content into the equation, Annabel gave stakeholders a more comprehensive toolkit for decision-making: they now had insights into not just when to release a film or which genre might be profitable, but also which themes, paired with the right genre, had historically yielded strong financial results.


<!-- 
Annabel’s goal was to provide the studio’s leadership with data-driven guidance on movie release strategies, content choices, and long-term planning. She began her analysis with a foundational question: How does profitability vary on a month-to-month basis?

Figure 1: Profitability Per Month offered the first glimpse of these patterns. Through boxplots, Annabel demonstrated that certain months, like June and December, often yielded higher median profits, yet came with more volatility. Others, like January or March, were more modest but more predictable. This initial view helped establish a baseline: timing matters, but each month carries its own risk profile.

Building on this, Annabel moved beyond single-month snapshots. Figure 4: Monthly Profitability Distribution by Season Across Decades grouped months into seasons and traced their share of profitability over long periods. By examining how these distributions shifted, Annabel revealed that what might look promising in a single month could be part of a larger seasonal trend evolving over many decades. Some seasons remained stable, while others rose or fell in prominence. This placed the monthly observations in a broader temporal context.

Annabel then expanded the perspective further with Figure 2: Long-Term Trends in Median Profitability and Success Rate. Looking back over the last century, she found that overall profitability and success rates have declined. While earlier figures offered tactical insights (e.g., which month or season might be better), these century-long trends highlighted a more challenging industry environment. Even though certain times of year still provide advantages, the general conditions for achieving profitability have grown tougher, especially compared to the mid-20th century. Yet, the data also suggested a leveling-off in recent decades, possibly indicating a new baseline from which studios must operate.

Next, she introduced Figure 5: Profitability Trends and Representation by Genre Over Time to understand how different genres fit into this evolving landscape. This figure revealed that some genres, like Family films, grew more prevalent but less profitable, while others, like LGBT or Action films, managed to increase (or at least maintain) profitability as their representation rose. This linked the time-based shifts to creative and market-driven factors—certain audience tastes and content strategies fare better as the industry transforms.

To get a closer look at how recent changes differ from long-term trajectories, Annabel presented a similar figure focusing on the last 20 years. Here, some genres that had previously declined seemed to stabilize or even improve slightly, showing that recent industry conditions can differ from century-long patterns. Such a short-term lens helps studios stay agile and responsive to current market trends.

To make these insights more actionable, Annabel introduced an interactive bubble chart that combined month-by-month profitability with genre filters and allowed the viewer to adjust bubble sizes by budget, runtime, or sample size. This interactive tool encouraged stakeholders to experiment and identify conditions under which certain genres and months align to produce solid returns. By exploring multiple dimensions simultaneously, the team could move from passive observation to active scenario testing.

Finally, Annabel presented a heatmap linking genres to themes, revealing how narrative elements interact with genres to influence profitability. Identifying which themes perform best within certain genres—especially those trending positively—could guide content creators and producers in crafting stories more likely to resonate with audiences and yield better financial results.

Taken together, these visualizations tell a comprehensive story. Starting from basic monthly differences and building towards a multi-layered understanding involving seasons, decades, genres, and themes, Annabel’s analysis offers both short-term tactical insights and long-term strategic perspectives. The combination of static figures and interactive tools ensures that decision-makers can not only understand historical patterns but also engage with the data to inform future strategies. This integrated approach provides the studio with a richer, more nuanced blueprint for making data-driven decisions in a complex and evolving film landscape.

 -->