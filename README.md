# Human Atlas 3D

Human Atlas 3D is an interactive browser anatomy explorer designed to scale from the whole human body down to named anatomical structures and, later, microscopic anatomy.

## Current build

The project now has a functioning drill-down anatomy architecture rather than a single generic human model.

### Interaction
- Rotate, zoom and inspect the human body in 3D
- Click directly on visible structures
- Double-click to drill deeper
- Search by common name, Latin name, region or system
- Browse a hierarchical anatomy tree
- Filter by organ system
- Focus a structure in 3D
- Isolate a structure and its descendants
- Exploded anatomical view
- Front, back, left and right standard views
- Connected-anatomy navigation
- Quick identification quiz mode
- Responsive desktop/mobile interface

### Hierarchy already represented

**Head**
- Skull
  - Frontal bone
  - Parietal bones
  - Temporal bones
  - Occipital bone
  - Sphenoid
  - Mandible
- Brain
  - Frontal lobe
  - Parietal lobe
  - Temporal lobe
  - Occipital lobe
  - Cerebellum
  - Brainstem
  - Pituitary gland

**Spine and nervous system**
- Cervical spine
  - Atlas (C1)
  - Axis (C2)
- Thoracic spine
- Lumbar spine
- Sacrum
- Spinal cord
- Cervical spinal nerves
- Thoracic spinal nerves
- Lumbar spinal nerves

**Thorax**
- Rib cage
- Sternum
- Heart
  - Right atrium
  - Right ventricle
  - Left atrium
  - Left ventricle
  - Aorta
- Lungs
  - Right lung
  - Left lung
  - Trachea

**Abdomen / pelvis**
- Liver
- Gallbladder
- Stomach
- Intestines
- Kidneys
- Urinary bladder

**Long bones**
- Humerus
- Radius
- Ulna
- Femur
- Patella
- Tibia
- Fibula

**Endocrine**
- Pituitary
- Thyroid

## Files

- `index.html` — complete interactive Three.js viewer
- `anatomy-data.js` — hierarchical anatomy knowledge graph and educational content

There is no build step. Serve the directory from any static server:

```bash
python -m http.server 8080
```

Then open `http://localhost:8080`.

## Architecture

Every anatomical structure has:
- unique ID
- parent structure
- depth level
- system
- region
- English and Latin names
- summary
- function
- facts
- anatomical connections

This lets the atlas grow without redesigning the UI. A future medical-quality mesh can use the same structure ID and automatically inherit search, hierarchy, isolation, learning content and navigation.

## Target: full human atlas

The finished goal is much larger than the structures currently modeled.

### Skeleton
All 206 adult bones plus named landmarks, sutures, foramina, processes, joints, cartilage and ligaments.

### Muscular
Superficial and deep muscles with origin, insertion, action, innervation and blood supply.

### Nervous
Brain subdivisions, spinal cord tracts, 12 cranial nerve pairs, plexuses, peripheral nerves, autonomic pathways and sensory/motor maps.

### Cardiovascular
All four heart chambers and valves, coronary circulation, named arteries, named veins and major microcirculation concepts.

### Respiratory
Airway hierarchy from nose/larynx through bronchi, bronchioles and alveoli plus diaphragm and respiratory mechanics.

### Digestive
Oral cavity, teeth, tongue, salivary glands, pharynx, esophagus, stomach layers, liver, gallbladder, pancreas, small intestine subdivisions, colon, rectum and anal canal.

### Urinary
Kidney cortex/medulla, pyramids, calyces, pelvis, ureters, bladder and urethra.

### Endocrine
Hypothalamus, pituitary, pineal, thyroid, parathyroids, thymus, adrenals, pancreatic islets and gonads.

### Lymphatic / immune
Lymphatic vessels, lymph nodes, spleen, thymus, tonsils and marrow concepts.

### Reproductive
Complete male and female reproductive anatomy with age-appropriate educational controls.

### Integumentary
Skin layers, hair follicles, sweat/sebaceous glands, nails and receptors.

### Special senses
Eye layers and chambers, visual pathway, external/middle/inner ear, cochlea, vestibular system, olfactory pathway and taste structures.

### Microscopic mode
Organ → tissue → cell → organelle, including representative histology and functional diagrams.

## Medical accuracy

The current 3D geometry is procedural and educational. It is **not** a diagnostic, surgical-planning or clinical model. The application architecture is ready for medically reviewed GLB/GLTF meshes, but those assets must be sourced or created and reviewed before the model should be described as medically accurate.
