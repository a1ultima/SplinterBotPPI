################
# SPLINTER BOT #
################

#Description:
	
Scrapes iPfam and for co-complex (structure solved) protein-protein interactions in Anopheles gambiae and Plasmodium falciparum, given UniProt protein PDB structure annotations. 

#Usage:
	
	bash ./generate_ppi.sh

#Dependencies (and how to install):

python 2.7.6: 			

	sudo apt-get install python27

splinter (python package): 	

	sudo pip install splinter

pickle (python package): 	

	sudo pip install pickle

#Input/config files:

	./uniProt_structures_anopheles_gambiae.tsv      <-- manually edit, or download from www.UniProt.org (e.g. search: "Anopheles gambiae").

	./uniProt_structures_plasmodium_falciparum.tsv 	<-- manually edit, or download from ww.UniProt.org (e.g. search: "Plasmodium falciparum")

#Outputs:

	./protein_to_protein_interactions.tsv 		<-- Predicted protein-protein interactions, each row contains a pair of 	co-complex interacting proteins.

	./protein_to_pdb.tsv 				<-- Protein IDs and their available PDB structures.

	./pdb_to_interactions.tsv 			<-- PDB structures involved in protein-interaction complexes.

	./interaction_to_url.tsv 			<-- iPfam URLs of co-complex interaction protein-structures involving proteins listed in ./uniProt_structures_*.tsv.

	./UniProt_to_VB_ids.tsv 			<-- Synonyms between "UniPRot" protein accession IDs "VectorBase" gene accession IDs. 


