# norns-shnth-patches
A collection of [shnth](https://github.com/pblasser/shbobo) patches collected from the internet and modified to work with Cfdrake's [Norns + Synth Library and Mod](https://github.com/cfdrake/shnth). 

I found that many patches, while working with the latest version of fish were failing to load when attempted from the Norns mod menu. Errors for these patches were in three main categories: 1.) patches used an outdated opcode "slave" which had been changed to "gear" in later versions of shlisp, 2.) patches were named with spaces in the file name which interrupts the mod loaders loading process before it can read the file, and 3.) the version of shlisp used by the Norns mod requires opcodes to use a spaceless syntax so that patches reading, for example, "bar a", should read "bar" while "bar b" should read "barb". 

All the patches contained in this collection should now load via the Norns menu.
