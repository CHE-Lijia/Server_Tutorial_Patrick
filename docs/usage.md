## Environment Usage Guide

Environments are stored at `/hdd1/shared_env/username/` 

Databases are stored at `/hdd1/shared_db/username/`

Software without environment requirement are stored at `/hdd1/shared_software/username/` 

### 1. Activating Environments

If you use aliases starting with [`act_`](./software_list.md#3-shell-configuration-recommended) for each environment. You can simply type the corresponding alias in your terminal to activate the environment.

**Examples:**

```bash
# Activate the assembly environment
act_asm

# Activate the taxonomic classification environment
act_gtdbtk
```

*Note: To deactivate the current environment, use the standard command: `conda deactivate`.*

### 2. Activating Environments

### 2. Using Databases

To manage large bioinformatics databases efficiently, we should use database on server instead of downloading multiple copies. If you defined all database paths as [environment variables](./software_list.md#3-shell-configuration-recommended). You are allowed to reference database locations directly in your commands without typing long, absolute paths.

**Database Variable List:**

| Variable Name | Path |
| :--- | :--- |
| `$ANTISMASH_DB` | `/hdd1/shared_db/chelijia/antismash_db` |
| `$BAKTA_DB` | `/hdd1/shared_db/chelijia/bakta_db` |
| `$CHECKM_DB` | `/hdd1/shared_db/chelijia/checkm_db` |
| `$CHECKM2_DB` | `/hdd1/shared_db/chelijia/checkm2_db` |
| `$EGGNOG_DB` | `/hdd1/shared_db/chelijia/eggnog_db` |
| `$GTDBTK_DB` | `/hdd1/shared_db/chelijia/gtdbtd_db` |
| `$IPHOP_DB` | `/hdd1/shared_db/chelijia/iphop_db` |
| `$KRAKEN2_DB` | `/hdd1/shared_db/chelijia/kraken2_db` |
| `$MOB_SUITE_DB` | `/hdd1/shared_db/chelijia/mob_suite_db` |
| `$VIRSORTER_DB` | `/hdd1/shared_db/chelijia/virsorter_db` |

When running analysis tools, you can use these variables directly as parameter input.

### 3. Applying Changes

If you modify your `~/.bashrc` file (e.g., by adding new aliases or database paths), you must run the following command to make the changes take effect in your current terminal session:

```bash
source ~/.bashrc
```

### 4. Contributing New Resources

This server is a collaborative environment. If you need a database or software that is not currently available, you can add it yourself and share it with others by following these steps:

**Adding New Databases**

If you need a database, please download it to the `/hdd1/shared_db/your_username/` directory. Once downloaded, send the path and your preferred variable name to *@chelijia*, and it will be added to the official database list.

*Example:*
```bash
export NEW_DB_NAME="/shared_db/your_username/new_db_name"
```

**Adding New Conda Environments**

If you need software that requires a Conda environment, please create it in the shared directory using the `--prefix` flag:

```bash
conda create --prefix /hdd1/shared_envs/your_username/env_name [packages...]
```

After creating the environment, set an alias for it (e.g., `alias act_new='conda activate /hdd1/shared_envs/your_username/env_name'`) and send it to *@chelijia* so it can be added to the environment list for everyone to access.

**Adding Standalone Software**

For software that does not require Conda or has no complex dependencies, please install it in:
`/hdd1/shared_software/your_username/softwarename/`

Once installed, send the details to *@chelijia* to have it added to the shared software list, making it available for others to use.
