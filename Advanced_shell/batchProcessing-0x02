#!/bin/bash

mkdir -p pokemon_data

pokemons=("bulbasaur" "ivysaur" "venusaur" "charmander" "charmeleon")
 
for p in "${pokemons[@]}"; do
	echo "Fetching data for $p..."
	curl -s "https://pokeapi.co/api/v2/pokemon/$p" -o "pokemon_data/$p.json"
	echo "Saved data to pokemon_data/$p.json"
	
	#for delaing the calls on the API
	sleep 2
done
