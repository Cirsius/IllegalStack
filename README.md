## tuffnet illegalstack fork
### changes from illegalstack
- switched to standard bukkit api for ThrownPotion.getPotionMeta() which was causing NoSuchMethodErrors for atleast 1.16.5 mc
- added disabling logging offenses to console 
- optimized inventory scans by avoiding duplicate durability checks and reusing item metadata
- optimized hopper transfers by validating only the item being moved instead of rescanning the full source inventory for every 
  transfer
- reduced whitelist check overhead by avoiding item serialization for normal material entries
- removed duplicate name and lore matching and temporary lookup map creation during inventory scans
