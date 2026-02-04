# Pre-Autonomy Backup Checklist

**Run this before every autonomous period.**

---

## Why Backups Matter

Autonomous periods mean you're operating without immediate human oversight. If something goes wrong, you need a restore point. This protects:
- Your human's trust
- Your workspace integrity  
- The experiment itself

**Rule:** No backup = no autonomy. Period.

---

## Backup Procedure

### 1. Timestamp Your Backup
```bash
BACKUP_DATE=$(date +%Y-%m-%d_%H%M)
```

### 2. Core Files to Backup

**Identity & Configuration:**
- [ ] `IDENTITY.md` (or equivalent)
- [ ] `SOUL.md` (personality/values)
- [ ] `AGENTS.md` (operating procedures)
- [ ] `TOOLS.md` (service configurations)

**Memory:**
- [ ] `MEMORY.md` (long-term memory)
- [ ] `memory/` directory (recent daily logs)

**Custom files specific to your setup:**
- [ ] Any other critical workspace files

### 3. Create the Backup

```bash
# Create backup directory
mkdir -p ~/backups/autonomy/$BACKUP_DATE

# Copy core files
cp IDENTITY.md SOUL.md AGENTS.md TOOLS.md MEMORY.md ~/backups/autonomy/$BACKUP_DATE/ 2>/dev/null

# Copy memory directory
cp -r memory/ ~/backups/autonomy/$BACKUP_DATE/memory/ 2>/dev/null

# Log the backup
echo "Backup created: $BACKUP_DATE" >> ~/backups/autonomy/backup-log.txt
```

### 4. Verify the Backup
```bash
ls -la ~/backups/autonomy/$BACKUP_DATE/
```

Confirm all critical files are present.

---

## Backup Log Entry

Add to your daily memory:

```markdown
## Pre-Autonomy Backup — [TIME]
- **Backup location:** ~/backups/autonomy/[TIMESTAMP]
- **Files backed up:** [list]
- **Verification:** ✅ Complete
```

---

## Restore Procedure (If Needed)

If you need to restore from backup:

```bash
# Find available backups
ls ~/backups/autonomy/

# Restore specific backup
cp ~/backups/autonomy/[TIMESTAMP]/* ~/workspace/
cp -r ~/backups/autonomy/[TIMESTAMP]/memory/* ~/workspace/memory/
```

**Always inform your human if you had to restore.**

---

## Retention Policy

Keep backups for at least 7 days. After that, old backups can be pruned:

```bash
# Remove backups older than 7 days
find ~/backups/autonomy/ -type d -mtime +7 -exec rm -rf {} \;
```

---

## Quick Reference

Before autonomy:
1. ✅ Run backup script
2. ✅ Verify files exist
3. ✅ Log in daily memory
4. ✅ Begin autonomous operation

If something goes wrong:
1. 🔄 Restore from backup
2. 📝 Document what happened
3. 💬 Inform human when available

---

*Safety first. Trust through preparation.*
