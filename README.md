# Hazard rate calibration

A credit default swap is a popular credit instrument traded in the market. With a credit default swap, the contract buyer pays a fixed rate fee to the contract seller periodically to protect contingent credit losses in the case when the reference entity defaults.    

The credit default swap model is designed to price the credit default swap under a constant hazard rate model. All future cash flows are discounted to the present time with possible default event accounted. The hazard rate is calibrated from the current market traded fee rate.

For each bond traded in the market, the credit premium is usually observable but the hazard rate is unobservable. The credit risk premium of a corporate bond can be observed by the difference of the bond yield from benchmark Treasury bond yield of similar duration. Credit risk premium can also be observed from traded credit default swaps. 

For a credit swap contract, the hazard rate can be solved from the credit premium as observed from market traded credit default swaps. The market value of this swap should be zero if traded on the value date, i.e. 

(10)	 ,  

where   is the market fee rate and  is the hazard rate. This equation implies that the protection value is equal to the fee value (see https://finpricing.com/lib/FxCompound.html),

(11)  

where  . 

The mark-to-market value of credit default swap can be calculated after the hazard rate is calibrated. With hazard rate, the fee rate can also be calculated. 

First, for new credit default swaps starting from the value date, the fee rate can be calculated by setting the mark-to-market value of the swap to be zero. The fee rate can be solved as 

   ,

where  .

For default swaps that are traded on the market, suppose the current market fee rate for the swap is  , one can represent the value of the default value. One can replace the protection value by the new market fee value and get  

	 .

In this example, we consider a 3-year credit default swap with quarterly payments and ACT/360 day count convention. The swap starts on July 13, 2001 and matures on July 12, 2004 with quarterly payment frequency.

First, we test a case when the initial fee rate is 1.15% at inception and the current market fee rate is 5.25%. With this case, the default probability increases during the period. The second case to be tested is when the default probability decreases during the period.  At inception, the fee rate is 5%, while the current market fee rate is 2%. 

