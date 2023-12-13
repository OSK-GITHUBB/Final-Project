Risein Final Project:

>>Part 1 - Information<<

Star System Collection: NFT mints of our Solar System objects (and possible beyond) with the following data:

Solar_System_Object_Type: Star, Planet, Moon, Astereoids

Name: 
Sun, 
Mercury, Venus, Earth, Mars, Jupiter, Saturn, Uranus, Neptune, 
Moon, Phobos, Deimos, Io, Europa, Ganymede, Callisto, Mimas, Enceladus, Tethys, Dione, Rhea, Titan, Iapetus
4979 Otawara, 140 Siwa

Rarity: Common (Astereoids), Rare (Planets and Sun), Legendary (Earth)

Short_description: Description about each object.

>>Part 2 - Codigo<<

Codigo CIDL (Código Interface Description Language) is used to create this project on solana.

Open codigo and create nft.yaml as shown.

Run "codigo solana generate nft.yaml"

We will write logic to 3 files as shown ................

Go to the folder with "Cargo.toml" (cd program should work) and run "cargo build-sbf".

>>Part 3 - Solana<<

Run "solana config set --url devnet"

Get as many solana coins as you need with command: "solana airdrop 1"

solana program deploy target/deploy/nft.so

Copy and save program id for testing in Part 4.

>>Part 4 - Test<<

Time to test to code we have just written:

navigate to the program_client directory and run: "yarn install"

"yarn add @solana/spl-token"

in program_client directory; create an app.ts file as shown.

npx ts-node app.ts <YOUR_PROGRAM_ID>

Observe output, you are done!
