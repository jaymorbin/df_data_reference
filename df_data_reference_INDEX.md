# df_data_reference

Path maps and structure dumps captured from a **live Dwarf Fortress game**. These are ground truth for where data actually lives in the DF object tree, as opposed to what documentation says about it.

## How to use this

Each path map is a flattened trace of one object, every field recursively expanded, in the form `df.global.world.raws.<family>.<list>[i].<field> = <value>`. To find where something lives, grep for the field or value name across the repo. The hit gives you the full access path verbatim.

```
grep -rn 'reaction_class' 'Object Path Maps/' 'Path Maps/'
```

## Path maps (50 files)

Grouped by object family. 'Subject' is the object the map was taken from.

### buildings (1)

| File | Subject | Code | Size |
|---|---|---|---|
| `vanilla_collect_sand_job_path_map.txt` | `df.global.world.buildings.all[3].jobs[0]` |  | 267K |

### descriptors (1)

| File | Subject | Code | Size |
|---|---|---|---|
| `descriptors_colors_object_map.txt` | `df.global.world.raws.descriptors.colors[0]` | AMBER | 5K |

### entities (3)

| File | Subject | Code | Size |
|---|---|---|---|
| `entity_object_map.txt` | `df.global.world.raws.entities.all[5]` | MOUNTAIN | 5526K |
| `shortened_entity_object_map.txt` | `df.global.world.raws.entities.all[0]` | MOUNTAIN | 204K |
| `vanilla_global-world-entities_path_map.txt` | `df.global.world.entities.all[0]` | MYTHICAL_ENTITY_1 | 949K |

### inorganics (22)

| File | Subject | Code | Size |
|---|---|---|---|
| `inorganic_path_map.txt` | `df.global.world.raws.inorganics.all[0]` | IRON | 31K |
| `iron_inorganic_path_map.txt` | `df.global.world.raws.inorganics.all[0]` | IRON | 31K |
| `making_metal_ite_inorganic_path_map.txt` | `df.global.world.raws.inorganics.all[332]` | MAKING_METAL_ITE_ITE | 29K |
| `making_metal_orichalcum_dirty_object_path_map.txt` | `df.global.world.raws.inorganics.all[324]` | MAKING_METAL_ALLOY_ORICHALCUM | 32K |
| `metal_ore_map.txt` | `df.global.world.raws.inorganics.all[214]` | MAGNETITE | 33K |
| `modded_cobalt_glass_inorganic_path_map.txt` | `df.global.world.raws.inorganics.all[498]` | GLASS_COBALT | 31K |
| `plaster_inorganic_path_map.txt` | `df.global.world.raws.inorganics.all[26]` | PLASTER | 28K |
| `vanilla_clear_diamond_inorganic_path_map.txt` | `df.global.world.raws.inorganics.all[153]` | DIAMOND_CLEAR | 29K |
| `vanilla_diorite_inorganic_path_map.txt` | `df.global.world.raws.inorganics.all[173]` | DIORITE | 29K |
| `vanilla_divine_inorganic_path_map.txt` | `df.global.world.raws.inorganics.all[265]` | DIVINE_1 | 32K |
| `vanilla_fire_clay_inorganic_path_map.txt` | `df.global.world.raws.inorganics.all[264]` | FIRE_CLAY | 32K |
| `vanilla_granite_inorganic_path_map.txt` | `df.global.world.raws.inorganics.all[172]` | GRANITE | 29K |
| `vanilla_kaolinite_inorganic_path_map.txt` | `df.global.world.raws.inorganics.all[230]` | KAOLINITE | 33K |
| `vanilla_limestone_inorganic_path_map.txt` | `df.global.world.raws.inorganics.all[167]` | LIMESTONE | 29K |
| `vanilla_magnetite_inorganic_path_map.txt` | `df.global.world.raws.inorganics.all[221]` | MAGNETITE | 30K |
| `vanilla_marble_inorganic_path_map.txt` | `df.global.world.raws.inorganics.all[185]` | MARBLE | 29K |
| `vanilla_mythical_remnant_path_map.txt` | `df.global.world.raws.inorganics.all[313]` | MYTHICAL_REMNANT_1 | 31K |
| `vanilla_mythical_substance_path_map.txt` | `df.global.world.raws.inorganics.all[314]` | MYTHICAL_SUBSTANCE_1 | 124K |
| `vanilla_obsidian_inorganic_path_map.txt` | `df.global.world.raws.inorganics.all[179]` | OBSIDIAN | 31K |
| `vanilla_quicklime_inorganic_path_map.txt` | `df.global.world.raws.inorganics.all[32]` | QUICKLIME | 28K |
| `vanilla_sand_tan_inorganic_path_map.txt` | `df.global.world.raws.inorganics.all[255]` | SAND_TAN | 28K |
| `vanilla_tetrahedrite_inorganic_path_map.txt` | `df.global.world.raws.inorganics.all[201]` | TETRAHEDRITE | 30K |

### itemdefs (1)

| File | Subject | Code | Size |
|---|---|---|---|
| `itemdefs_object_map.txt` | `df.global.world.raws.itemdefs` |  | 42K |

### jobs (1)

| File | Subject | Code | Size |
|---|---|---|---|
| `vanilla_job_maybe_fillpond_path_map.txt` | `df.global.world.jobs.list.next` |  | 106K |

### mat_table (6)

| File | Subject | Code | Size |
|---|---|---|---|
| `basic_inorganic_object_path_map.txt` | `df.global.world.raws.mat_table.builtin.INORGANIC` | INORGANIC | 22K |
| `vanilla_ash_builtin_path_map.txt` | `df.global.world.raws.mat_table.builtin.ASH` | ASH | 21K |
| `vanilla_coal_builtin_path_map.txt` | `df.global.world.raws.mat_table.builtin.COAL` | COAL | 20K |
| `vanilla_green_glass_builtin_path_map.txt` | `df.global.world.raws.mat_table.builtin.GLASS_GREEN` | GLASS_GREEN | 22K |
| `vanilla_lye_builtin_path_map.txt` | `df.global.world.raws.mat_table.builtin.LYE` | LYE | 20K |
| `vanilla_water_builtin_path_map.txt` | `df.global.world.raws.mat_table.builtin.WATER` | WATER | 21K |

### material_templates (1)

| File | Subject | Code | Size |
|---|---|---|---|
| `material_template_object_map.txt` | `df.global.world.raws.material_templates.all[0]` | STONE_TEMPLATE | 17K |

### plants (1)

| File | Subject | Code | Size |
|---|---|---|---|
| `plant_object_map.txt` | `df.global.world.raws.plants.all[0]` | SINGLE-GRAIN_WHEAT | 224K |

### reactions (13)

| File | Subject | Code | Size |
|---|---|---|---|
| `make gukil strings instrument piece path map.txt` | `df.global.world.raws.reactions.reactions[525]` | MAKE_ENT306 INS2STRINGS | 23K |
| `make_gadan_instrument_reaction_path_map.txt` | `df.global.world.raws.reactions.reactions[550]` | MAKE_ENT306 INW2 | 23K |
| `make_plaster_powder_reaction_map.txt` | `df.global.world.raws.reactions.reactions[95]` | MAKE_PLASTER_POWDER | 37K |
| `modded_make_cobalt_glass_reaction_path_map.txt` | `df.global.world.raws.reactions.reactions[306]` | MAKE_COBALT_GLASS | 67K |
| `modded_steel_making_reaction_map.txt` | `df.global.world.raws.reactions.reactions[656]` | STEEL_MAKING | 85K |
| `reaction_path_map.txt` | `df.global.world.raws.reactions.reactions[152]` | STEEL_MAKING | 66K |
| `vanilla_brass_making_reaction_path_map.txt` | `df.global.world.raws.reactions.reactions[138]` | BRASS_MAKING | 37K |
| `vanilla_lignite_to_coke_reaction_path_map.txt` | `df.global.world.raws.reactions.reactions[137]` | LIGNITE_TO_COKE | 22K |
| `vanilla_make_clay_bricks_reaction_path_map.txt` | `df.global.world.raws.reactions.reactions[99]` | MAKE_CLAY_BRICKS | 22K |
| `vanilla_make_clay_jug_reaction_path_map.txt` | `df.global.world.raws.reactions.reactions[98]` | MAKE_CLAY_JUG | 22K |
| `vanilla_make_quicklime_reaction_path_map.txt` | `df.global.world.raws.reactions.reactions[116]` | MAKE_QUICKLIME | 37K |
| `vanilla_make_sharp_rock_reaction_path_map.txt` | `df.global.world.raws.reactions.reactions[96]` | MAKE_SHARP_ROCK | 36K |
| `vanilla_make_soap_from_tallow_reaction_path_map.txt` | `df.global.world.raws.reactions.reactions[92]` | MAKE_SOAP_FROM_TALLOW | 51K |

## Object maps (2)

| File | Subject | Code | Size |
|---|---|---|---|
| `reaction_object_map.txt` | `df.global.world.raws.reactions.reactions[138]` | BRASS_MAKING | 18K |
| `inorganic_object_map.txt` | `df.global.world.raws.inorganics.all[0]` | IRON | 9K |

## Dumps, enums and notes (13)

| File | Kind | Lines | Size |
|---|---|---|---|
| `FIELDS ON item_corpsepiecest.txt` | struct field list | 74 | 5K |
| `ITEM_TOOL_LIST.txt` | notes | 463 | 19K |
| `ITEM_TYPE_DUMP.txt` | console dump | 95 | 1K |
| `ITEM_TYPE_DUMP_SORTED.txt` | console dump | 984 | 32K |
| `building_types_and_subtypes_and_skills_numbers.txt` | console dump | 194 | 3K |
| `building_types_and_subtypes_numbers` | console dump | 40 | 565B |
| `building_types_and_subtypes_numbers.txt` | console dump | 40 | 565B |
| `enum_item_type_dump.txt` | console dump | 97 | 1K |
| `jobs sorted.txt` | notes | 272 | 6K |
| `make_gadan_instrument_job_inspect_85.txt` | dump | 669 | 32K |
| `make_gukil_strings_instrument_piece_job_inspect_86.txt` | dump | 669 | 32K |
| `metal panel metal tooltip paths and notes.txt` | notes | 62 | 5K |
| `path map directory.txt` | stale dir listing | 123 | 8K |

## Notes

- `building_types_and_subtypes_numbers` has **no file extension**. Searches filtered on `*.txt` will miss it. Its `.txt` twin is byte-identical.
- `path map directory.txt` is a stale PowerShell directory listing of an old local folder, not an index. It carries timestamps but no descriptions, and may name files no longer present. This INDEX supersedes it.