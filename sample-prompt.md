# Worldbuilding Data Integration & Story Correlation Process

**Objective**: Systematic worldbuilding data integration with story correlation using Fi's Kernel Sequence Protocol for optimal efficiency and quality assurance.

**Activation Requirements**: This workflow meets Kernel Sequence Protocol activation criteria (batch processing, cross-dimensional validation, file operations with quality standards). Fi should implement full protocol framework for systematic execution.

## Primary Workflow

**Entry Selection**: Process 3-5 unprocessed entries from `worldbuilding/data-parsed/` per iteration. If folder is empty, task is complete. Prioritize entries with complex cross-references to maximize graph connectivity preservation.

## Processing Framework

For each selected entry, apply systematic analysis:

**Story Correlation**:
- Conduct semantic search across story content using entry name and related concepts
- Search character files (`../characters/`), chapter summaries (`../summaries/`), and content indexes
- Document story appearances with chapter citations and character interactions
- Assess plot relevance and narrative significance

**Content Integration**:
- **Canonical Priority**: Story canon takes precedence over worldbuilding conflicts
- **Unique Detail Preservation**: Retain worldbuilding information not present in story
- **Conflict Documentation**: Log contradictions in `worldbuilding-contradictions.md`
- **Tag Optimization**: Add relevant thematic, character-relationship, and geographic tags

**Quality Standards**:
- **Complete Entries**: Full descriptions with story integration
- **Stub Entries**: Mark as "PLACEHOLDER - [concept]" while preserving searchability  
- **Cross-Reference Validation**: Ensure mentioned entities exist or create stub entries
- **Graph Connectivity**: Maintain bidirectional references for concept traversal

## File Management & Documentation

**Automated Processing**: Edit entries directly within `data-parsed/` directory for optimal efficiency.

**File Movement System**: 
- Add completed filenames (without path) to `worldbuilding/files-to-move.txt`
- User executes `move-processed-files.bat` (Windows) or `move-processed-files.sh` (Unix/Linux/macOS)
- Script transfers files from `data-parsed/` to `data/` and clears tracking file

**Iteration Summary**: Provide completion report including:
- Processed entries summary with key decisions
- Notable canonical conflicts or cross-reference changes  
- List of completed files ready for automated movement

## Success Criteria

**Primary Goals**:
- Maintain cross-reference network for concept traversal during writing
- Apply story canon authority consistently
- Preserve searchable placeholder entries while marking status clearly
- Ensure comprehensive story integration for each processed entry
- Limit iterations to 3-5 entries for systematic thoroughness

**Completion Indicator**: Process continues until `worldbuilding/data-parsed/` directory is empty, indicating full integration phase completion.

**Quality Assurance**: Each iteration should enhance the worldbuilding reference system's story integration while preserving conceptual relationships and maintaining efficient searchability for writing support.
