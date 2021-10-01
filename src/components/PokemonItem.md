```jsx
const pokemons = [
   {_id: 1,
    name: 'Bulbasaur',
    image: 'https://pokemon-json.herokuapp.com/images/001Bulbasaur.png',
    description: "Bulbasaur is a small, quadruped Pokémon that has blue-green skin with darker patches. It has red eyes with white pupils, pointed, ear-like structures on top of its head, and a short, blunt snout with a wide mouth. A pair of small, pointed teeth are visible in the upper jaw when its mouth is open. Each of its thick legs ends with three sharp claws. On its back is a green plant bulb, which is grown from a seed planted there at birth. The bulb provides it with energy through photosynthesis as well as from the nutrient-rich seeds contained within."
   },
   {_id: 2,
    name: 'Ivysaur',
    image: 'https://pokemon-json.herokuapp.com/images/002Ivysaur.png',
    description: "Ivysaur is a quadruped Pokémon that has blue-green skin with darker patches. On top of its head are pointed ears with black insides and it has narrow red eyes. It has a short, rounded snout with a wide mouth and two pointed teeth in its upper jaw. Each of its feet has three claws on them. The bulb on its back has bloomed into a large pink bud. A short brown trunk surrounded by leafy green fronds supports the bud. The weight of the plant prevents Ivysaur from standing on its hind legs and forces its legs to grow sturdy. When its flower is ready to bloom, it gives off a distinct, strong sweet-smelling aroma and starts swelling. Ivysaur will also start spending more time in sunlight in preparation for its upcoming evolution. Exposure to sunlight adds to the strength of both Ivysaur and its plant. Ivysaur's natural habitat is plains."
   },
   {_id: 12,
    name: 'Butterfree',
    image: 'https://pokemon-json.herokuapp.com/images/012Butterfree.png',
    description: "Butterfree resembles a vaguely anthropomorphic butterfly with a purple body. Unlike true insects, it only has two body segments and four light blue legs. The upper pair of legs resembles small, three-fingered hands, while the lower pair resembles long, digit-less feet. Butterfree has two black antennae, a light blue snout with two fangs underneath, and large, red compound eyes. Its two pairs of wings are white with black venation. Two oval scales on a female Butterfree's lower wings are black, but they are white on a male."
   }
];




<div className='mb-8'>
    <ul className='grid grid-cols-1 gap-6 sm:grid-cols-2 md:grid-cols-3 lg:grid-cols-4' id='pokemon-list'>
        {pokemons.map(pokemon => (
            <PokemonItem
                key={pokemon._id}
                name={pokemon.name}
                image={pokemon.image}
                description={pokemon.description}
            />
        ))}
    </ul>
</div>
```
