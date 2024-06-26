---
type: "page"
showTableOfContents: true
---
# The One–Dimensional Heisenberg Model, RG Methods and Numerical Simulation of the SDRG Process

You can find the thesis [here](/pdfs/bthesis.pdf) and the code [here](https://github.com/aethrvmn/1d-RandAFHeisenberg-SDRG)

## Abstract

The Strong Disorder Renormalisation Group (SDRG) method, first introduced by Dasgupta, Ma and Hu, and later greatly expanded by Fisher, yields asymptotically exact results in distributions where the disorder grows without limit in large scales, whilst Fisher also calculated limit values as well as scaling factors for random spin chains.

These results where the first of many, yielded through the intense research that followed afterwards, firstly in random quantum systems, and later expanded in classically disordered systems as well. The previous Real Space RG methods that were used treated the whole space as homogenous, allowing the grouping of spins into super-spins, and although in systems absent of randomness this homogenity is physically verifiable, it comes into question in the presence of disordered systems. The SDRG method has the property of renormalising space in a non-homogenous way so it can better handle local disorders.
 
More specifically, the XX chain, presented by Fisher, can be used to obtain exact results for the behaviour of phases dominated by randomness, as well as the critical behaviour near the various zero temperature phase transitions that occur. Studying the properties of antiferromagnetic Heisenberg spin-1/2 chains with random bonds, we analyse the low-energy behaviour, by decimating the strongest bond, replacing it with a new effective bond between the nearest neighbours. Repeating the procedure, the distribution becomes extremely broad improving the accuracy of the approximation. 

The structure of the thesis is this. First we introduce the Heisenberg model, it's relation to the Ising and Free Fermion models, solve it exactly for the ferromagnetic case using the Bethe Ansatz and introduce the Block RG method for the antiferromagnetic case. Afterwards we present the Strong Disorder RG method, using a modernised version of Fisher's process to solve the random AF XX chain. Finally, we present the methods we created to simulate the process.
