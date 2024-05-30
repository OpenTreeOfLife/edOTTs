edOTTs
======

JSON edits usable as inputs to [otcetera](https://github.com/OpenTreeOfLife/otcetera)
otc-taxonomy-patcher tool (currently on the taxonomy-diff-maker branch)
for editing the Open Tree of Life Taxonomy (ott).

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

  6. `edott-000009.json` No hand edits recorded

  7. `edott-000010.json` No hand edits recorded


More automatic updates:

  1. `edott-000011.json` amendment-1 sha = [5f4764d6f0f4b2908465100fae724640b6306153](https://github.com/OpenTreeOfLife/amendments-1/commit/5f4764d6f0f4b2908465100fae724640b6306153)

  2. `semanticize_amendments.py amendments-1 5f4764d6f0f4b2908465100fae724640b6306153 > edott-000012.json` while amendments-1 was at [2faeefa1549ad7c231533528d1ec1dc1420060bd](https://github.com/OpenTreeOfLife/amendments-1/commit/2faeefa1549ad7c231533528d1ec1dc1420060bd)

 3. edott-000013 is still in progress, but started via running  `semanticize_amendments.py amendments-1 2faeefa1549ad7c231533528d1ec1dc1420060bd > edott-000013.json` while amendments-1 was at [09800651d3bef9f335fe663951cdc9d857ffa084](https://github.com/OpenTreeOfLife/amendments-1/commit/09800651d3bef9f335fe663951cdc9d857ffa084) see [notes/edott-000013-notes.md](https://github.com/OpenTreeOfLife/edOTTs/blob/main/notes/edott-000013-notes.md) for some notes.

