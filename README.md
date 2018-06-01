# dollar_value_add_attribution
Working document illustrating mechanics of performance attribution measured as dollar value add.  We may develop this in to more of a presentation later.

At ASRS we do performance attribution on a "dollar value add" basis.  This just means that rather than "Equities Selection Effect was X bp", we instead say that we added $Y million through equities selection.  

Of course, the dollar values added at the component level need to add up to the total fund.  This turns out to be a little tricky in a multi-period scenario, especially with imperfect real world data.  

In a scenario with perfect data (the weighted average of the component returns equals the total fund return), the trick turns out to be to reinvest the individual period values added in the total fund benchmark.  

Investment return data are rarely perfect, and this method illustrates how to handle a scenario where the weighted average composite returns don't sum to the total fund return.  To use this, change the muddydata variable to TRUE.  The residual gets pushed in to an "unknown" attribution category.  

