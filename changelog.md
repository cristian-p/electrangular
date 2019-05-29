# Changelog
All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](http://keepachangelog.com/)
and this project adheres to [Semantic Versioning](http://semver.org/).

# Scope
This changelog applies to the following scripts:
- ExecSequenceDatastage_<<acronym>>_TOOL_TWS_RADAR.sh
- ExecSequenceDatastage_<<acronym>>_TOOL_RADAR.sh
- ExecSequence_common_RADAR.sh

## [0.8] - 29/05/2019

### Added

### Changed


## [0.7] - 07/01/2019

### Added
- Handling FLG_OUTPUT_MODE (new field in the U7B2_OWN.TR_BD_TWS_DSJOB table)
- Handling FILE_OUTPUT_WS
- Check -z ${NOM_JOB_DATASTAGE} 
- RESET command before launching job

### Changed
- dsjob command inside $COMMAND variable
- Launch dsjob with 2>&1


## [0.6] - 08/12/2018

### Added
- ExecSequence_common_RADAR.cleanLogsAndCFG that handles the following activities:
    - gzips files with last modified date between 31 and 62 days 
    - deletes logs and gzipped logs older than 62 days;
    - deletes ITT/in/tmp_cfg/<<UUID>>.cfg files older than 8 days;
- Datastage output (runInfo) is now redirected to log

### Changed
- The file <<UUID>>.cfg is no longer deleted and the end of the process

### Fixed
- Fixed spelling for some parameter names and log outputs

## [0.1] to [0.5] - 26/07/2018
### Added
- Initial implementation
### Changed
-
### Removed
-
### Fixed
-
### Security
-
### Deprecated
-


## [Unreleased]
### Added
- 
### Changed
-
### Removed
-
### Fixed
-
### Security
-
### Deprecated
-