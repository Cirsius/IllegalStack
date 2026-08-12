## tuffnet illegalstack fork
### changes from illegalstack
- switched to standard bukkit api for ThrownPotion.getPotionMeta() which was causing NoSuchMethodErrors for atleast 1.16.5 mc
- added disabling logging offenses to console 
- optimized inventory scans by avoiding duplicate durability checks and reusing item metadata
