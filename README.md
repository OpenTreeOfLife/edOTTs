edOTTs
======

JSON edits usable as inputs to [otcetera](https://github.com/OpenTreeOfLife/otcetera)
otc-taxonomy-patcher tool for editing the Open Tree of Life
Taxonomy (ott).

Provenance will later be inlined. Currently:

  1. `edott-000001.json` - *Homo sapiens sapiens* should no longer be hidden. See https://github.com/OpenTreeOfLife/reference-taxonomy/pull/374

  2. `edott-000002.json` - flagging `extinct` and `extinct_inherited` as `incertae_sedis`, which is how the synthesis algorithm treats them.

  3. `edott-000003.json` - simple taxon additions taken from the commits between [12c810f5da4cc4c32ea2f6e3c6993eb18b0d2586](https://github.com/OpenTreeOfLife/amendments-1/commit/12c810f5da4cc4c32ea2f6e3c6993eb18b0d2586) and [77292e0e8f31ae3f4266531ee4ec14e1c5562a74](https://github.com/OpenTreeOfLife/amendments-1/commit/77292e0e8f31ae3f4266531ee4ec14e1c5562a74) in https://github.com/OpenTreeOfLife/amendments-1


The next 5 edits are from the taxon amendments that fall within the range included 
in `edott-000003.json`, but they required some hand editing.

  1. `edott-000004.json` - *Bucco noanamae* is the preferred name, but an unrecognized synonym of the genus name *Nystactes* caused this bird species to be in the *Heteroconger* eels in OTT 3.2

  2. `edott-000005.json` - *Cirrhilabrus briangreenei* was assigned 2 IDs because the taxon additions are not live in the TNRS.

  3. `edott-000006.json` - *Celeus ochraceus* was assigned 2 IDs because the taxon additions are not live in the TNRS.
  
  4. `edott-000007.json` - *Alopochen mauritiana* was assigned 2 IDs because the taxon additions are not live in the TNRS.

  5. `edott-000008.json` - *Poospiza nigrorufa* is not an synonym of *Sporophila nigrorufa*

