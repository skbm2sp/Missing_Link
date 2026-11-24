# Missing Link: Specimen Intake

A pixel-art browser game for Grade 9 Science, in the style of Papers, Please. Field paleontologists come to your intake window with specimen files. Date each fossil, identify it, stamp it and hand it back. The shift report at the end is the screenshot students submit. Works on laptops and iPads (landscape).

## Starting a game
1. **Title page:** choose SINGLE PLAYER or MULTIPLAYER · CO-OP (two inspectors).
2. **Application form:** type surname and first name (one row, or two for co-op), tap the photo to choose a preset portrait or add your own picture to *My Folder* (photos are saved only on that device), choose the section, difficulty and number of cases (3, 5, 8 or 10), and sign in the SIGN HERE box. The tutorial box is ticked by default.
3. **Tutorial:** Director Ramos hands over a practice trilobite and walks the student through each step. Wrong answers are rejected and explained. SKIP TUTORIAL is at the top right.

## Pause menu
The **❚❚ MENU** button on the shelf (or the Esc key on a laptop) pauses the game and stops the shift clock. From there: **Resume**, **Restart** (a new shift with new folders, or the tutorial from step 1) or **Main menu** (back to the title screen; the current shift is discarded). Restart and Main menu ask for confirmation.

## Difficulty
| Level | What changes | Pay per point |
|---|---|---|
| Normal | Full manual and complete files | ₱10 |
| Difficult | No half-life table: work out n with the calculator | ₱15 |
| Extreme | Difficult, plus damaged files: grams instead of %, no photo, missing date and size, two observations unreadable | ₱20 |
| Progamer | Extreme, and no manual at all | ₱30 |

The tutorial always uses Normal rules.

## How a case works
1. A reporter (a silhouette at the window) slides a folder onto the desk.
2. Click the folder to open it. It holds three papers: Lab report, Field report and Specimen ID form.
3. Pull the manual and calculator up from the shelf. Use the half-life table and calculator to write n and the age, the time scale for the period, the organism guide (choose a period) and name list to identify the organism, and choose the type of fossil.
4. Press the STAMPS tab on the right. Set each stamp with its ▼, slide the ID form so its box sits under the yellow arrow, and press the stamp.
5. Put all three papers back on the folder, click its inside cover to close it, and drag it up to the reporter.

Each file is worth 4 points (period, type of fossil, organism name, organism type). The age is checked but not scored. The results page shows the students' photos, names, section, difficulty, signature and a verification code.

## Organisms
35 cases: Anomalocaris, Trilobite, Hurdia, Cambroraster, Mosura, Kampecaris, Meganeura, Pederpes, Hylonomus, Brasilodon, Shonisaurus, Eudimorphodon, Eocursor, Archaeopteryx, Brachiosaurus, Brontosaurus, Stegosaurus, Allosaurus, Ichthyosaurus, Tyrannosaurus rex (coprolite), Velociraptor, Edmontosaurus, Archaeornithura, Eomaia, Pakicetus, Purgatorius, Obdurodon, Australopithecus, Leptobos, Diprotodon, Woolly mammoth, Homo habilis, Homo erectus, Homo neanderthalensis and Homo sapiens (Tabon Cave).

Organism-type stamps: Arthropod, Amphibian, Reptile (not a dinosaur), Ornithischian / Sauropod / Theropod dinosaur, Early mammal, Monotreme, Marsupial, Placental. Fish, cephalopods and synapsids from the lessons appear in the guide and name list as look-alikes, not as cases.

## Settings
In `index.html`, the `CFG` line near the top of the second script sets the case-count choices, perfect-shift bonus, duplicate chance (0.0128 per case, about a 5% chance of a repeated organism in a 5-case shift) and the section list. Pay per point is in `DIFFS` on the next lines.

## Credits
Inspection logic follows the Rule / Ruleset pattern from anakreon/PapersPlease (https://github.com/anakreon/PapersPlease, ISC licence). Fonts: VT323 and Silkscreen (Google Fonts, SIL Open Font Licence). Layout inspired by Papers, Please (Lucas Pope); all art is original and generated in code, including the random reporter portraits.
