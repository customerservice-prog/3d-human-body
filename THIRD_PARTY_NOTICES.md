# Human Atlas 3D — Third-Party Anatomy Notices

Human Atlas 3D includes adapted open anatomical mesh data. These notices apply to the identified mesh assets and their adaptations; they do not relicense unrelated Human Atlas application code.

## BodyParts3D skin and organ meshes

- Bundled files: `assets/bodyparts3d-skin.js` and `assets/bodyparts3d-organs.js` (base64-encoded GLB data used by the browser viewer).
- Work/source: BodyParts3D version 3.0, © The Database Center for Life Science.
- Source mirror: https://github.com/Kevin-Mattheus-Moerman/BodyParts3D
- Original archive: https://doi.org/10.18908/lsdba.nbdc00837-000
- License: Creative Commons Attribution-ShareAlike 2.1 Japan.
- Official legalcode: https://creativecommons.org/licenses/by-sa/2.1/jp/legalcode
- Adaptations in Human Atlas 3D: browser bundling/encoding, scene registration, materials, opacity, semantic grouping, click interaction, system filtering and physiology animation.
- These mesh adaptations remain subject to the same CC BY-SA 2.1 Japan license.

## Open3Dmodel / Open Anatomy skeleton mesh

- Bundled files: `assets/open3d-skeleton-1.js`, `assets/open3d-skeleton-2.js`, and `assets/open3d-skeleton-3.js` (parts of one base64-encoded GLB used by the browser viewer).
- Work/source: Open3Dmodel Create / Open Anatomy lineage.
- Source information: https://anatomytool.org/open3dmodel-create
- Viewer/source repository used for the reviewed demo asset: https://github.com/djansma/open3dviewer
- License: Creative Commons Attribution-ShareAlike 4.0 International.
- Official legalcode: https://creativecommons.org/licenses/by-sa/4.0/legalcode
- Adaptations in Human Atlas 3D: browser bundling/encoding, selection of bone nodes, coordinate fitting, runtime mirroring of right-side paired bones, materials and click/system interactions.
- These skeleton adaptations remain subject to CC BY-SA 4.0.

## Three.js

- Source: https://github.com/mrdoob/three.js
- Copyright: three.js authors.
- License: MIT.
- Human Atlas 3D loads Three.js and its GLTF/DRACO loaders at runtime.

## Draco decoder

- Source: https://github.com/google/draco
- Copyright: The Draco Authors.
- License: Apache License 2.0.
- Used at runtime to decode compressed anatomy GLB meshes.

## Medical-use note

The atlas is educational. Meshes and simulated physiology are not validated for diagnosis, surgery planning, treatment decisions, or other clinical use.
