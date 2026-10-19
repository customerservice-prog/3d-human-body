# Human Atlas 3D

An interactive, browser-based 3D human anatomy explorer.

## What the first version already does

- Interactive 3D whole-body anatomy
- Click structures directly in the 3D scene
- Search anatomy by name, Latin name, region, or system
- Toggle complete body systems on/off
- Adjust system opacity to peel through layers
- Isolate a selected structure
- Front / back / left / right anatomical views
- Educational panel with function, facts, connections, and study prompts
- Quiz mode
- Responsive desktop/mobile shell
- No build step required

## Included anatomy foundation

### Skeletal
Skull, vertebral column, rib cage, pelvis, humerus/forearm bones, femur/lower-leg bones.

### Nervous
Brain and spinal cord.

### Cardiovascular
Heart and simplified major vessels.

### Respiratory
Lungs, trachea, bronchi.

### Digestive
Liver, stomach, intestines.

### Urinary
Kidneys.

## Run it

Open `index.html` in a modern browser, or serve the repository with any static web server.

For example:

```bash
python -m http.server 8080
```

Then open `http://localhost:8080`.

## Where this should go next

This project is intentionally structured as an expandable anatomy atlas, not a one-off demo. The procedural geometry in version 1 proves the interaction system. The next major upgrade should replace simplified geometry with medically accurate, individually named GLB/GLTF meshes while keeping the same click/search/isolate/learn workflow.

Recommended expansion order:

1. **Head & brain** — skull bones, meninges, cerebrum, lobes, cerebellum, brainstem, ventricles, major nuclei, cranial nerves.
2. **Full skeleton** — every named bone with landmarks, sutures, foramina and joints.
3. **Muscular system** — superficial/deep layers with origin, insertion, action and innervation.
4. **Nervous system** — spinal nerves, plexuses, peripheral nerves, autonomic pathways.
5. **Cardiovascular** — chambers, valves, coronary circulation, arteries, veins and capillary concepts.
6. **Respiratory** — lobes, segments, bronchi, alveoli, diaphragm.
7. **Digestive / endocrine / urinary / reproductive / lymphatic / integumentary systems.**
8. **Microscopic zoom** — organ → tissue → cell → organelle.
9. **Learning modes** — guided lessons, labeling quizzes, flashcards, pathology comparison, spaced repetition.
10. **Accessibility** — keyboard navigation, reduced-motion mode, text-only anatomy tree, screen-reader structure descriptions.

## Accuracy note

The current 3D geometry is educational/procedural, not suitable for diagnosis, surgery planning, or clinical decision-making. Medical-grade anatomical meshes and expert-reviewed content should be used before describing the model as clinically accurate.
