# EarthMetrics
**Observation Without Interpretation.**
- HTML Mirror:  [https://roxanneardary.com/earthmetrics-specification/](https://roxanneardary.com/earthmetrics-specification/)

---

EarthMetrics is an open-source specification for a global environmental observation system designed to preserve, organize, verify, and provide access to recorded measurements of Earth's physical systems.

The specification defines a modular architecture for collecting historical and real-time observations from across the planet while preserving the distinction between observation and interpretation.

EarthMetrics records what was measured, where it was measured, when it was measured, how it was measured, and where the record originated.

The system is designed to support environmental records from the earliest available measurement and record-keeping systems through present-day observation networks.

EarthMetrics does not require the core observation layer to assign causes, generate conclusions, or determine what a measurement means.

---

## Core Principle

### Observation Without Interpretation.

EarthMetrics separates recorded observation from analysis.

The core system preserves measurable facts and the metadata necessary to understand those measurements.

EarthMetrics recognizes the following principles:

Observation is not explanation.

Measurement is not conclusion.

Correlation does not equal causation.

A change in a measurement does not independently establish the cause of that change.

Interpretation, modeling, forecasting, and hypothesis testing may use EarthMetrics data through separate systems without altering the original observation record.

## Purpose

The purpose of EarthMetrics is to establish a transparent and durable global record of environmental measurements.

The system is intended to support:

* Historical environmental data preservation
* Real-time environmental observation
* Long-term measurement archives
* Independent scientific analysis
* Public access to environmental records
* Reproducible research
* Data provenance
* Measurement verification
* Historical record digitization
* Distributed data preservation

EarthMetrics is designed as foundational infrastructure rather than as a system for promoting a particular scientific, political, commercial, or policy conclusion.

---

## Core Modules

### Observation Registry

The Observation Registry is the central record system for EarthMetrics.

It stores individual measurements and observations while preserving the original recorded value whenever available.

Each observation should support:

* Unique observation identifier
* Observation type
* Recorded value
* Original unit
* Standardized unit when available
* Observation timestamp
* Geographic location
* Source identifier
* Instrument identifier when available
* Measurement method when available
* Record creation timestamp
* Data provenance reference

The original observation must remain distinguishable from any normalized, converted, corrected, or derived representation.

### Historical Record Module

The Historical Record Module manages the ingestion and preservation of environmental records created before modern automated observation systems.

Supported sources may include:

* Early weather observations
* Historical weather station records
* Ship logs
* Maritime journals
* Scientific notebooks
* Observatory records
* River records
* Geological records
* Printed measurement archives
* Handwritten environmental logs
* Historical survey records

Historical records should preserve references to the original source material whenever possible.

Digitized records should retain information about:

* Original document
* Archive or collection
* Digitization method
* Transcription method
* Date of digitization
* Contributor or system responsible for transcription
* Verification status

### Real-Time Observation Module

The Real-Time Observation Module supports the ingestion of current measurements from compatible observation systems.

Potential sources include:

* Weather stations
* Ocean buoys
* River gauges
* Atmospheric sensors
* Seismic stations
* Satellite systems
* Hydrological sensors
* Public observation networks

Real-time ingestion must preserve the original source timestamp and identify when EarthMetrics received the observation.

### Atmospheric Observation Module

The Atmospheric Observation Module manages measurements relating to the atmosphere.

Supported observations may include:

* Air temperature
* Atmospheric pressure
* Humidity
* Wind speed
* Wind direction
* Precipitation
* Snowfall
* Snow depth
* Cloud observations
* Atmospheric composition
* Upper-air observations
* Jet stream measurements and position records

The module records measurements and associated metadata without assigning causes to atmospheric conditions or changes.

### Ocean Observation Module

The Ocean Observation Module manages measurements relating to oceans and other large bodies of water.

Supported observations may include:

* Sea surface temperature
* Subsurface temperature
* Salinity
* Wave height
* Wave direction
* Ocean currents
* Tide levels
* Water movement
* Water displacement
* Sea level measurements
* Buoy observations

Multiple measurements of the same location or event must remain independently identifiable.

### Hydrology Module

The Hydrology Module manages observations relating to freshwater systems and water movement.

Supported observations may include:

* River discharge
* River height
* Stream flow
* Groundwater measurements
* Reservoir levels
* Lake levels
* Flood measurements
* Watershed observations
* Precipitation accumulation

The module should preserve both continuous measurements and historical observations where available.

### Cryosphere Module

The Cryosphere Module manages measurements relating to frozen water systems.

Supported observations may include:

* Glacier measurements
* Ice sheet measurements
* Ice thickness
* Sea ice extent
* Snowpack depth
* Snow coverage
* Ice mass measurements when directly measured or provided as a documented dataset

Derived values must remain distinguishable from original measurements.

### Geological Observation Module

The Geological Observation Module manages recorded physical changes and events relating to Earth's geology.

Supported observations may include:

* Earthquakes
* Seismic measurements
* Volcanic activity
* Tectonic movement
* Land uplift
* Land subsidence
* Landslides
* Ground displacement

The module records the event or measurement without requiring the core record to establish why it occurred.

### Instrument Registry

The Instrument Registry provides a structured record of instruments and measurement systems associated with EarthMetrics observations.

An instrument record may include:

* Instrument identifier
* Instrument type
* Manufacturer
* Model
* Measurement method
* Accuracy specification
* Operating range
* Installation date
* Retirement date
* Sensor location
* Calibration history reference

Historical instruments may contain incomplete metadata.

Missing metadata should be recorded as unavailable rather than inferred.

### Calibration Module

The Calibration Module records available information about instrument testing, calibration, adjustment, maintenance, and replacement.

A calibration record may include:

* Instrument identifier
* Calibration date
* Calibration method
* Reference standard
* Reported accuracy
* Calibration organization
* Supporting documentation

Calibration records must not overwrite the original observation.

### Provenance Module

The Provenance Module tracks the origin and history of every dataset and observation.

A provenance record should support:

* Original source
* Source organization or archive
* Source record identifier
* Acquisition method
* Import date
* Transformation history
* Dataset version
* Verification references
* Original document or file reference when available

EarthMetrics should make the path from an observation back to its source as transparent as possible.

### Data Lineage Module

The Data Lineage Module records how data moved through the EarthMetrics system.

Lineage may include:

* Original source
* Original record
* Import process
* Validation process
* Unit conversion
* Normalization
* Dataset release
* Derived dataset relationship

Lineage information should allow users to distinguish an original observation from later processing.

### Raw Data Preservation Module

The Raw Data Preservation Module protects original observations from silent modification.

The module supports:

* Append-only records
* Historical version preservation
* Change logging
* Source retention
* Original value preservation
* Original unit preservation
* Original timestamp preservation when available

Corrections or later information should be stored as additional records or documented revisions rather than silently replacing the historical record.

### Raw and Adjusted Data Module

The Raw and Adjusted Data Module separates original observations from adjusted, corrected, normalized, or otherwise modified values.

When an adjusted dataset is included, EarthMetrics should preserve:

* Original value when available
* Adjusted value
* Adjustment method
* Adjustment source
* Dataset version
* Documentation reference

Adjusted values must not be presented as the original measurement.

### Parallel Observation Module

The Parallel Observation Module preserves independent measurements from multiple sources.

When multiple instruments or systems measure the same or similar conditions, the observations should remain individually accessible.

The module does not require:

* Automatic averaging
* Forced consensus values
* Replacement of conflicting observations
* Selection of a single authoritative measurement

Differences between observations may be documented as metadata without requiring EarthMetrics to determine which measurement is correct.

### Measurement Quality Module

The Measurement Quality Module stores factual information about the quality and condition of recorded observations.

Supported information may include:

* Instrument accuracy
* Resolution
* Calibration status
* Completeness
* Missing fields
* Known transmission errors
* Source quality indicators
* Verification status

Quality metadata must remain separate from conclusions about environmental causes or outcomes.

### Unit Preservation and Normalization Module

The Unit Preservation and Normalization Module stores the unit used in the original record and may generate standardized representations for querying and comparison.

The module must preserve:

* Original value
* Original unit
* Standardized value
* Standardized unit
* Conversion method

Unit conversion must not remove access to the original measurement.

### Dataset Versioning Module

The Dataset Versioning Module preserves the history of imported and published datasets.

Each dataset release should support:

* Dataset identifier
* Version identifier
* Source version
* Import date
* Publication date
* Change description
* Source reference

Older versions should remain identifiable and accessible when legally and technically possible.

### Integrity Module

The Integrity Module provides mechanisms for detecting unauthorized or undocumented changes.

Supported mechanisms may include:

* Cryptographic hashes
* Record checksums
* Signed dataset manifests
* Append-only logs
* Version history
* Independent verification

Integrity mechanisms should verify the state and history of data without changing the underlying observation.

### Coverage and Data Gap Module

The Coverage and Data Gap Module identifies where observations are unavailable, sparse, incomplete, or missing.

The system should support analysis of:

* Geographic coverage
* Temporal coverage
* Measurement density
* Missing periods
* Incomplete metadata
* Instrument availability

Data gaps are part of the factual record and should remain visible.

### Event Indexing Module

The Event Indexing Module organizes observations associated with identifiable environmental or geological events.

Supported event categories may include:

* Hurricanes
* Storms
* Floods
* Droughts
* Earthquakes
* Tsunamis
* Volcanic events
* Extreme temperature events

Event indexing should describe the observed event and its associated measurements.

The core module must not require a causal explanation for the event.

### Historical Replay Module

The Historical Replay Module allows users to explore observations associated with a selected time and location.

The module may provide access to:

* Recorded weather conditions
* Ocean observations
* Hydrological observations
* Geological activity
* Seismic activity
* Available historical measurements

Missing data must remain visible rather than being silently replaced with estimated values.

### Query Module

The Query Module provides access to EarthMetrics observations across time, geography, measurement type, source, and instrument.

Queries may support:

* Date ranges
* Geographic regions
* Geographic radius
* Measurement types
* Instrument identifiers
* Source datasets
* Observation categories
* Dataset versions

The query system should make raw and adjusted data distinguishable.

### Public API Module

The Public API Module provides programmatic access to EarthMetrics data and metadata.

The API should support access to:

* Observations
* Datasets
* Instruments
* Calibration records
* Provenance records
* Data lineage
* Historical archives
* Coverage information

API responses should provide enough metadata to identify the origin and status of returned records.

### Data Export Module

The Data Export Module enables users to retrieve EarthMetrics data for independent storage and analysis.

Supported export formats may include:

* CSV
* JSON
* Parquet
* NetCDF
* Other documented open formats

Exports should preserve provenance and dataset version information where technically practical.

### Historical Document Archive Module

The Historical Document Archive Module associates structured observations with original records.

Supported materials may include:

* Scanned documents
* Handwritten logs
* Printed tables
* Ship journals
* Historical charts
* Scientific notebooks

The original source material should remain distinguishable from transcribed or structured data.

### Citizen Observation Module

The Citizen Observation Module supports contributions from individuals and independent sensor networks.

Citizen observations should support classification such as:

* Unverified
* Source documented
* Instrument identified
* Calibration documented
* Independently verified

Classification describes the status of the record and does not determine whether an environmental conclusion is true.

### Distributed Mirror Module

The Distributed Mirror Module supports independent copies of EarthMetrics datasets.

Mirrors may be operated by:

* Universities
* Research institutions
* Independent organizations
* Public archives
* Individual operators

Mirror systems should preserve dataset version and integrity information.

### Offline Archive Module

The Offline Archive Module supports long-term preservation through downloadable and independently hosted dataset packages.

Archive packages may include:

* Data files
* Metadata
* Dataset manifests
* Integrity hashes
* Documentation
* Provenance records

The goal is to reduce dependence on a single service or organization.

### Visualization Module

The Visualization Module provides interfaces for exploring observations without modifying the underlying data.

Supported visualizations may include:

* Maps
* Time series
* Geographic coverage
* Historical comparisons
* Measurement timelines
* Event views
* Data availability views

Visualizations should clearly distinguish measured observations from derived or optional analytical outputs.

### Planetary Dashboard Module

The Planetary Dashboard Module provides a public interface for viewing current and historical observations.

The dashboard may display:

* Temperature measurements
* Atmospheric pressure
* Wind observations
* Precipitation
* Ocean conditions
* Water movement
* River measurements
* Seismic activity
* Ice observations

Displayed information should identify its source and measurement status.

---

## Optional Plugin Modules

Optional plugin modules extend EarthMetrics without changing the core principle of preserving observations separately from interpretation.

Plugins may access EarthMetrics data through documented interfaces while maintaining clear boundaries between core records and plugin-generated results.

### Analysis Plugin

The Analysis Plugin provides statistical and computational tools for examining EarthMetrics data.

Possible capabilities include:

* Trend analysis
* Statistical comparison
* Correlation analysis
* Distribution analysis
* Time series analysis

Results generated by the plugin must remain separate from the core observation record.

### Modeling Plugin

The Modeling Plugin supports the use of EarthMetrics data in external or integrated models.

Possible capabilities include:

* Environmental models
* Atmospheric models
* Hydrological models
* Ocean models

Model outputs must be identified as derived results rather than recorded observations.

### Forecasting Plugin

The Forecasting Plugin supports predictive systems that use EarthMetrics data as an input.

Forecasts must remain separate from historical and real-time observation records.

### Hypothesis Testing Plugin

The Hypothesis Testing Plugin supports structured research and scientific investigation.

The plugin may document:

* Research questions
* Methods
* Selected datasets
* Statistical procedures
* Results

Research outputs must not alter the original observation layer.

### External Dataset Connector Plugin

The External Dataset Connector Plugin provides reusable connectors for importing compatible datasets.

Each connector should document:

* Data source
* Access method
* Source license
* Import method
* Field mapping
* Dataset version behavior

### OCR and Transcription Plugin

The OCR and Transcription Plugin assists with the digitization of historical records.

Capabilities may include:

* Optical character recognition
* Handwriting transcription
* Structured table extraction
* Human review workflows

The plugin should preserve the original document and distinguish machine-generated transcription from verified transcription.

### Satellite Processing Plugin

The Satellite Processing Plugin supports ingestion and processing of satellite observation products.

Derived products must remain distinguishable from source observations and source datasets.

### Sensor Integration Plugin

The Sensor Integration Plugin provides connectors for compatible hardware and independent observation networks.

The plugin may support:

* Automated data submission
* Instrument registration
* Calibration reporting
* Measurement transmission

### Community Verification Plugin

The Community Verification Plugin supports public review of historical documents, transcriptions, metadata, and data provenance.

Verification activity should be recorded transparently and should not erase the original submitted record.

### Advanced Visualization Plugin

The Advanced Visualization Plugin may provide specialized interfaces including:

* Three-dimensional globe views
* Historical environmental replay
* Measurement animation
* Comparative data views
* Geographic exploration tools

### Research Workspace Plugin

The Research Workspace Plugin provides tools for creating reproducible research projects based on EarthMetrics data.

A workspace may record:

* Dataset versions
* Queries
* Analysis methods
* Generated results

Research workspaces remain separate from the core observation database.

### Mirror Node Plugin

The Mirror Node Plugin provides software and configuration support for independent EarthMetrics mirrors.

Capabilities may include:

* Dataset synchronization
* Integrity verification
* Version management
* Public discovery

### Alerting Plugin

The Alerting Plugin may notify users when selected measurements or observation conditions meet user-defined criteria.

Alerts must be identified as automated notifications and must not modify historical observations.

---

## Data Principles

EarthMetrics follows these principles:

* Preserve original measurements whenever available.
* Preserve original units.
* Preserve original timestamps whenever available.
* Preserve source references.
* Preserve dataset versions.
* Document transformations.
* Keep raw and adjusted data separate.
* Preserve parallel observations.
* Make data gaps visible.
* Maintain traceable provenance.
* Record corrections transparently.
* Keep analysis separate from observation.
* Keep forecasts separate from recorded conditions.
* Keep models separate from measured records.
* Keep causal claims outside the core observation layer.

## Transparency Requirements

EarthMetrics implementations should provide transparent access to information necessary to understand a record.

Where available, this includes:

* Data source
* Source identifier
* Measurement method
* Instrument information
* Timestamp
* Location
* Original unit
* Dataset version
* Transformation history
* Calibration information
* Verification status

Missing information should be identified as unavailable rather than silently inferred.

## Vision

EarthMetrics aims to establish a permanent, transparent, and independently verifiable record of Earth's environmental measurements.

The specification is designed to preserve the distinction between what was observed and what people conclude from those observations.

EarthMetrics does not exist to determine a single explanation for Earth's physical systems.

It exists to preserve the record.

---

## Specification Branding License (SBL)
### Standard
- Fully AGPL-3.0+ compliant system
- Copyleft enforced for network deployments
- Required attribution:
  - Roxanne Ardary
  - https://www.roxanneardary.com/

### Optional

- **Specification Branding License (SBL)**
  - Attribution-free commercial deployment
  - Pricing based on scale, usage, and deployment scope
  - [https://roxanneardary.com/earthmetrics/](https://roxanneardary.com/earthmetrics/)

---

## 📜 License & Notice Requirements

EarthMetrics is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.  
By contributing to this project, you agree that your contributions will also be released under this license.

Please note the following:

- All contributions must comply with the **AGPL-3.0+** terms.  
- Under **Section 7** of the license, all redistributions, forks, and derivative works must preserve attribution to:  
  **Roxanne Ardary** and **[roxanneardary.com](https://www.roxanneardary.com/)**
- EarthMetrics specifications are free to use with attribution. A Specification Branding License can be negotiated upon request.
- The project's **notice.md** file tracks attribution requirements and contributor acknowledgments.  
  Any update that adds new contributors or modifies attribution should also update `notice.md`. 
- When submitting a pull request, ensure that any new files maintain the attribution headers where applicable.
- Network-deployed versions of this software must also remain fully AGPL-3.0+ compliant, including exposure of source code modifications when applicable under the license.

For full legal details, please refer to the AGPL-3.0+ license and the project's `notice.md` file.
