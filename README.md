
## Files

### 1. `empty_cells`
**Purpose**: Counts the number of empty cells in each column of a semicolon-delimited file.

**Usage**:
```bash
./empty_cells input.txt ";"
```
### 2. `preprocess`
**Purpose**:
- Fills in missing IDs with sequential numbers
- Converts comma-based decimals to dot-based
- Converts semicolon-delimited input to tab-delimited output
- Removes non-ASCII characters

**Usage**:
```bash
./preprocess input.txt > cleaned.tsv
```

### 3. `analysis`
**Purpose**:
- Finds the most popular mechanics and domains
- Calculates correlation between:
  - Year Published and Rating Average
  - Complexity Average and Rating Average

**Usage**:
```bash
./analysis cleaned.tsv
```



## ✅ Example Workflow

```bash
chmod +x empty_cells
  ./empty_cells input.txt ";"
chmod +x preprocess 
  ./preprocess input.txt > cleaned.tsv
chmod +x analysis
  ./analysis cleaned.tsv
```
