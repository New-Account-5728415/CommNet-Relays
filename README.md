# CommNet Relays

Ever wanted to get money for setting up CommNet network relays? Your dreams can come true with the **CommNet Relays** contract pack!

## Features

**CommNet Relays** is a contract pack for Contract Configurator which gives you contracts for each body in the solar system (besides the homeworld, of course). The contract is to send a satellite with an appropriate dish or combination of dishes into an orbit low enough that surface missions can use the whip antenna instead of having to pack a big dish (so long as a relay is overhead, of course). Missions to your homeworld's moons are required to use an HG-5 or equivalent, missions to the inner planets (Duna/Mars and inward) are required to use an RA-15 or equivalent, while missions to outer planets or moons will need an RA-100 or equivalent. You also have to have your tracking station upgraded to the appropriate level.

The contracts are generated based on the lists of planets and moons in your solar system, so you can install Outer Planets or Real Solar System or whatever you want, and the contracts will automatically adjust themselves accordingly. Additionally, the antenna requirement does not depend on specific parts, but on the combined antenna power of the relay, so it's compatible with all modded antennas automatically. If you really wanted to (and had a computer that could handle it), you could build a relay with 20,000 HG-5 antennas for Jool missions.

(That said, be aware that the contract range requirements are based on stock CommNet ranges, which are in turn based on the stock solar system. I've got some patches that will modify ranges to adapt to Outer Planets and Real Solar System, but those patches assume particular balance choices for antennas and the solar system. At the end of the day, the contract requirement is just a lower bound -- check your link budgets before launch.)

In addition to the basic "relay around body X" contracts, there are a few extra contracts to help improve uptime around the network. You may receive contracts to place relays in highly-inclined, highly-elliptical orbits around the gas giants, so that missions to their moons or in low orbits can stay in contact around them, as well as contracts to place relays in solar orbits to keep contact with probes going behind the Sun (and also the homeworld's parent body, if you're using an alternate solar system in which the homeworld is a moon).

## Dependencies

* CommNet Relays depends on [**Contract Configurator**](http://forum.kerbalspaceprogram.com/threads/101604-1-0-2-Contract-Configurator-v1-0-4-2015-05-08), version **1.22.0** or later.
* You will need [**Module Manager**](http://forum.kerbalspaceprogram.com/index.php?/topic/50533-105-module-manager-2613-november-9th/) to patch the contracts for compatibility with other addons.

## Download and install

* under "Code" download zip

From there, just unzip the "ContractPacks/CommNetRelays" folder into your GameData directory.

## Known issues and limitations

It might be cool if nightingale implemented a coverage-checking feature like there is for RemoteTech, but as things are, I use the number of relays or relay-like vessels in orbit as a proxy -- four is the minimum to get full coverage (though that could be as low as two depending on how forgiving you've set the line-of-sight "fudge factor" to be), so if you've got five ships with enough relay antennas in low-enough orbit around a body, I figure you have coverage that's good enough and the config won't generate contracts for that body. In general, I've left most of the details of your network unconstrained -- the minimum and/or maximum values in the requirements will keep your satellites within range of the ground, but it's up to you to put your satellites in orbits that are useful for your particular situation.

If you find any other issues, please let me know in the [**KSP forum thread**](http://forum.kerbalspaceprogram.com/threads/129704-1-0-2-4-Contract-Pack-CommNet-Relays-1-0-0-%282015-Jul-24%29) or on the GitHub repo's [**issue tracker**](https://github.com/Kerbas-ad-astra/CommNet-Relays/issues)!

## Version history and changelog

* 2025 05 28 ():
	* Added initial JNSQ patch

## Roadmap

If you have suggestions, please post an [**issue**](https://github.com/Kerbas-ad-astra/CommNet-Relays/issues) on the GitHub repo.

## Credits

Many thanks to nightingale for Contract Configurator (and for implementing the SemiMajorAxis() method at my request, and accepting my HasAntenna parameter), toadicus for AntennaRange (which inspired the initial revision of this contract pack), and Squad for implementing CommNet!

## License

CommNet Relays is copyright 2015-2019 Kerbas_ad_astra. Contract configuration files are released under the [**GPL v3 license**](https://www.gnu.org/licenses/gpl-3.0) (or any later version). Any redistributions must use a different name and folder (per section 7c). All other rights (e.g. the CommNet Relays logo and agency definition files) reserved.
