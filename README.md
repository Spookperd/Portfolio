# Cambridge Crystallographic Structure Database (CCSD) Mining 

This section deals with the data mining and analysis of Gold structures obtained from the CCSD. The database was queried via a Python API and several structural parameters were extracted from each structure that matched the search criteria. This data were then processed using Pandas, and visualised with the Matplotlib and Seaborn packages.

**1.**

<img src="https://user-images.githubusercontent.com/107844512/217597625-580300b1-7df2-4d38-b9f2-58287e4a25c9.jpg" width="500" height="500">

This image shows a catagorized distributions of Gold-Q distances and L-Gold-Q angles. The plot shows that each Q-atom has a preferential distance, angle or both and turns out to have a fundamental reason why. Attracting charges dont have an orientational preference, but when Q is big, there is quantum interaction. 

**2. **

<img src="https://user-images.githubusercontent.com/107844512/217600729-bf0ece9c-30d5-46d5-abb6-99062b87097d.png" width="500" height="500">

This figure challenges the idea of chemical bonding of compounds containing Gold. These violin plots show a large variation in the distance for the N, O and F Q's, but a musch smaller variation for Q = S, Cl, Br and I, which means that they bond while N, O and F don't.  These plots also show that atoms are naturally occurring at preferred distances, although the current understanding is that there is no reason it should be, because they don't bond. This figure was used to challenge a long standing idea that Gold does not bond to other elements (a specific type of bond)

**3. **

<img src="https://user-images.githubusercontent.com/107844512/217618277-b03542be-8c96-40c0-a15e-1c021cd6d266.png" width="500" height="500">

The distributions shown in 1 and 2 can be further classified by the way the atoms interact with one another. A linear relationship emerged with the 1-4 intra class for example that limits the orientation of Q = F in Gold complexes. 

# Predictive regression model 

<img src="https://user-images.githubusercontent.com/107844512/217620428-9fc4a1bf-c41b-47e3-9518-a680644e5df1.png" width="500" height="500">

Some of the structures were further analysed using state of the art Quantum Mechanical software, and a bonding model for these compounds was extracted, including the exponential regression model shown above that was able to predict the strength of the bond between Gold and another atom, based on input parameters. 

# Buying a car
When I sold my last car, I think I got too little for it. Dealers use the "Book Value" to their advantage when buying and selling cars. I was interested in buying a car online, but I had no idea what a fair price would be, and I didn't trust their pricing. So I wrote a bot that scraped car sites for a specfic make, and mined all of the available data from the site, and put this into a Pandas Dataframe. I made a regression model, using the normalised milage, year, specs and condition to filter which cars were good value. 

<img src="https://user-images.githubusercontent.com/107844512/217647895-e73eef28-9c1b-49ea-aefc-d62ebc0399d7.png" width="550" height="500">

This shows the list price vs. milage for the car model I was looking at. There is a large variation in price for a given milage, since model year, location and condition is not shown in this Figure, but by doing a regression model, I could score vehicles by value, and take the url;s as output. The unfortunate thing is I still could not automate scams, so there were a few in my top 10 best value cars. I was able to also predict a value of a car, given it's specs, but this is a small sample size, so it was only reliable to convince a sneaky salesman.

I ran this script recently, and visually compare the results. Despite the massive rise in interest rate, and economic pressure, prices remain similar. This vehicle is often used commercially, so this may be why cars are not decreasing in price. 

