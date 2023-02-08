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

# 
