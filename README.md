# chem.model
Model that displays ionic and formal charge interactions between ions/ligands and amino acid side chains. Python.



item= input("Enter Amino Acid: ")
charge= input("Enter Charge: ")

pcaa = ["arginine", "histidine", "lysine"]
ncaa= ["aspartic acid", "glutamic acid"]
ucaa= ["glycine", "alanine", "valine", "leucine", "isoleucine", "methionine", "proline", "tryptophan", "phenylalanine", "cysteine"]


#positively charged amino acids
if item in pcaa and charge== "positive":
        print("Reaction= Repulsive & Positively charged side chain")

elif item in pcaa and charge== "negative":
        print("Reaction= Attractive & Positively charged side chain")

#negatively charged amino acids
elif item in ncaa and charge== "negative":
        print("Reaction= Repulsive & Negatively charged side chain")

elif item in ncaa and charge== "positive":
        print("Reaction= Attractive & Negatively charged side chain")

#uncharged amino aciids
elif item in ucaa and charge== "negative" or charge== "positive":
        print("Reaction= None & Non-Polar side chain")

else: print("Error in Entry")

stop=input("Hit enter to close")
print(stop)
