=========
Changelog
=========

* :release: `10.2.2 <2023-02-28>`
* :bug:`389` Adding unit_as_strings_factory to fix Unit serialization expected as str not dict
* :bug:`389` Fix DispenseColumn serialization prior to constructing Dispense Instruction

* :release: `10.2.1 <2023-02-27>`
* :bug:`387` Fix Instruction::MagneticTransfer invalid volume detection

* :release: `10.2.0 <2023-02-24>`
* :support:`385` Further updates for dataclass compatibility

* :release: `10.1.1 <2023-02-23>`
* :feature: `378` Adjust `96-deep-kf` and `96-v-kf` container types `true_max_vol` to 1.8mL and
                    added validations in `MagBuilders` class such that plates being put onto KF
                    device do not exceed working vol with comb

* :release: `10.1.0 <2023-02-15>`
* :feature: `383` Propagating properties now adds instead of sets for acoustic spread

* :release: `10.0.0 <2023-02-02>`
* :support: `381` Recommit changes to version 10.0.0

* :release:`9.1.1 <2023-02-02>`
* :support: `380` Reverting braking changes that 9.1.0 introduces in order to semantically adjust changes to a major version bump

* :release:`9.1.0 <2023-01-04>`
* :feature:`375` Move typing dataclasses to own module and create unit data type aliases
* :feature:`373` Add restriction on container type to echo compatible plates
* :feature:`369` Update: Autoprotocol python typing

* :release:`9.0.0 <2022-12-20>`
* :feature:`372` Acoustic transfer propagates well properties
* :feature:`371` Added new container type: `384-corning-4512-round-lv`

* :release:`8.0.1 <2022-12-07>`
* :feature:`365` Update autopick method signature to allow for multiple pick groups per instruction

* :release:`8.0.0 <2022-11-16>`
* :feature:`358` Dataclass enhancements to support objects schema-ready and de/serialization
* :support:`360` typing for Protocol.instruction() methods
* :feature:`359` Depriciate Python 3.6

* :release:`7.15.1 <2022-10-27>`
* :feature:`350` update: set pump_override_volume to default to None

* :release:`7.15.0 <2022-10-27>`
* :feature:`354` Added new container type: `96-spl-flat-uv-ps`
* :feature:`353` Added new container type: `384-spl-flat-uv-ps`

* :release:`7.14.4 <2022-09-01>`
* :feature:`347` update: container and well ctx_properties

* :release:`7.14.3 <2022-05-19>`
* :feature:`345` Add new container type: `1536-echo-ldv-beckman-001-6969`

* :release:`7.14.2 <2022-01-11>`
* :feature:`343` Add new container: `384-corning-4513-round-lv`

* :release:`7.14.1 <2021-12-06>`
* :support:`339` Fix Unit handling in `set_compounds` for None, null values

* :release:`7.14.0 <2021-12-04>`
* :feature:`337` Update requirements for tracking concentration on compounds, set defaults

* :release:`7.13.1 <2021-12-02>`
* :feature:`334` Addition of `concentration` and `solubility_flag` keys to compound metadata

* :release:`7.13.0 <2021-11-15>`
* :feature:`332` Extract compound metadata from JSON payload

* :release:`7.12.0 <2021-11-11>`
* :feature:`330` Update allowed step_size in `Dispense`

* :release:`7.11.0 <2021-11-07>`
* :feature:`327` Update container class to have contextual custom properties

* :release:`7.10.1 <2021-10-27>`
* :feature:`323` Add seal ["ultra-clear", "foil"] to FLAT384WHITETC
* :support:`318` Update all pre-commit hooks except pylint to latest versions

* :release:`7.10.0 <2021-10-25>`
* :support:`321` Support `mass=None` assignment
* :feature:`319` Support Python 3.10
* :support:`320` Bump pytest, pytest-cov and coverage versions for python 3.10 support

* :release:`7.9.6 <2021-10-18>`
* :feature:`316` Refactor extracted `mass_mg` -> `mass`

* :release:`7.9.5 <2021-09-30>`
* :feature:`312` Add new container: `96-pcr-fs-clear`
* :feature:`309` Change container short name `384-flat-black-clear-tc` to `384-flatbottom-black-clear-tc`

* :release:`7.9.4 <2021-09-21>`
* :feature:`308` Update `liquid_handle_dispense` instruction to allow for multiple intake hoses in source

* :release:`7.9.3 <2021-09-13>`
* :feature:`306` Add new containers: `384-ubottom-black-clear-tc` and `384-flat-black-clear-tc`
* :feature:`305` Add `cold_196` incubation location

* :release:`7.9.2 <2021-06-22>`
* :support:`304` remove standard cover type attribute from container type: 96-ubottom-clear-tc

* :release:`7.9.1 <2021-06-08>`
* :support:`302` Remove volume from wells that are on a container that is evaporated

* :release:`7.9.0 <2021-05-25>`
* :feature:`300` Allow reservoir stamping for plates with shape SBS384 provided that container has capability: `sbs384_compatible`. Capability added to container RESSW384LP.
* :support:`300` Add tests in util to check if container type is a compatible reservoir

* :release:`7.8.0 <2021-05-18>`
* :feature:`301` Add liquid_handle_dispense method, include protein buffer liquid class and volume resolution in `LiquidHandleBuilders`. Add helper function for building device level mode_params in LiquidHandleBuilders for tempest.
* :support:`301` Add tests for liquid_handle_dispense method
* :support:`301` Update authors

* :release:`7.7.0 <2021-03-18>`
* :feature:`297` Add support for SMILES to Compound class
* :bug:`296 major` Remove low-evaporation cover type from FALCON96UBOTTOM

* :release:`7.6.1 <2021-03-04>`
* :bug:`294` Fix output of AttachCompounds wells

* :release:`7.6.0 <2021-03-02>`
* :feature:`292` Add informatics param to p.transfer
* :support:`291` Update copyright and authors
* :feature:`290` Add informatics attribute to Instruction

* :release:`7.5.0 <2021-01-31>`
* :feature:`288` Add "Compound" to derived types
* :support:`284` add isort for automatic import sorting
* :support:`286` CodeCov action for GitHub actions
* :support:`285` use readme.rst for long description
* :feature:`283` Support Python 3.9
* :support:`282` migrate CI from travis to GitHub actions
* :support:`281` Add downloads badge to track package usage

* :release:`7.4.1 <2020-11-19>`
* :bug:`277` Fix travis.yml deployment syntax

* :release:`7.4.0 <2020-10-28>`
* :feature:`276` Add 96-flat-white-dc container type
* :bug:`275 major` Fix acoustic transfer `one_source` bug to take dead volume into account.
* :bug:`274 major` Container.wells_with(prop, val) not returning wells with val due to `is` operator instead of `==`

* :release:`7.3.0 <2020-10-01>`
* :feature:`272` Add 96-ubottom-clear-tc container type
* :bug:`266 major` FlowCytometry excitation field should be optional and support specification of multiple lasers
* :bug:`270 major` 0 uL acoustic transfer raises an error instead of creating empty 'groups' field
* :support:`269` Update travis.yml to trigger deployment only once

* :release:`7.2.0 <2020-09-15>`
* :feature:`265` Add support for mass_concentration, amount_concentration and volume_concentration, as specified in ASC-51
* :support:`267` Pin black version to reduce CI/local inconsistencies. Pin to 20.8b1

* :release:`7.1.1 <2020-07-21>`
* :bug:`261` Revert empty Protocol assertion check in `as_dict()`

* :release:`7.1.0 <2020-06-29>`
* :feature:`259` Add humanize and robotize support for 1536w
* :feature:`258` Add time_constraints value to the Protocol attributes
* :feature:`254` Add support for provisioning of resources by mass

* :release:`7.0.1 <2020-06-02>`
* :bug:`255` Update desired_mode method in LiquidHandle to allow for cases where mode_param is empty

* :release:`7.0.0 <2020-05-28>`
* :bug:`253 major` Provision instruction for multiple wells is not including all wells in the request
* :support:`252` Switch to using .readthedocs.yml for docs build config
* :support:`251` Add code coverage badge
* :support:`250` Bump test dependencies, notably pytest to >=5.4, pylint to 2.5.2 and tox >=3.15
* :support:`249` Update documentation dependencies, notably Sphinx to >=2.4
* :feature:`248` Bump Pint version to 0.9
* :support:`247` Add `black` as auto-formatter to pre-commit workflow
* :support:`245` Add expected propagate_properties behavior tests
* :bug:`244 major` Revert Protocol.propagate_properties to use Well.add_properties
* :feature:`239` Add `absorbance` and `fluorescence` capabilities to 96-well-v-bottom container type
* :support:`243` Update docs with environment setup and testing
* :support:`243` Restructure travis.yml jobs structure to separate out each stage
* :support:`243` Add basic pre-commit infrastructure, shift pylint inside pre-commit
* :support:`241` Deprecate support for Python 3.5, add support for Python 3.8
* :feature:`238` Add 96-well-v-bottom container type

* :release:`6.2.0 <2020-05-13>`
* :support:`236` Support auto-deploy from travis
* :feature:`235` Add support for specifying different Protocol subclasses in harness.run
* :support:`232` Update various date, emails and copyright references
* :support:`232` Move and update license, authors, contributing to top-level
* :bug:`233 major` Change Protocol.propagate_properties to use Well.set_properties
* :bug:`231 major` Fix LiquidHandleBuilders method desired_mode docstring preventing Travis build
* :feature:`229` Update LiquidHandle instruction with 'density' parameter and 'positive_displacement' mode
* :support:`228` Remove Phabricator references

* :release:`6.1.2 <2020-02-18>`
* :bug:`226` Don't unnecessarily sanitize inputs in z position builder

* :release:`6.1.1 <2020-01-27>`
* :bug:`223` Fix `well_from_shape` logic for 384 well plates
* :feature:`221` Add `warm_35` incubation location
* :bug:`220` Fix Image autoprotocol parameter

* :release:`6.1.0 <2019-10-14>`
* :feature:`217` Add `concentration(molar)` to valid input-types in harness
* :feature:`217` Add `concentration(mass)` to valid input-types in harness
* :bug:`216 major` Fix pytest-cov package dependency

* :release:`6.0.1 <2019-09-11>`
* :bug:`213` Fix SPE autoprotocol instruction key
* :bug:`212` Fix Agitate parameter order
* :bug:`209` Fix Sonicate `bath` mode default frequency
* :bug:`210` Fix `semantic-version` dependency, pin to 2.6.0 for docs to build

* :release:`6.0.0 <2019-08-21>`
* :support:`206` Deprecate support for Python 2, migrate to support only Python >=3.5
* :support:`205` Fix changelog formatting

* :release:`5.6.0 <2019-08-18>`
* :feature:`203` Add `image` instruction
* :feature:`202` Add `SPE` instruction
* :feature:`201` Add `evaporate` instruction
* :feature:`200` Add `sonicate` instruction
* :feature:`199` Add `agitate` instruction

* :release:`5.5.0 <2019-07-17>`
* :feature:`196` Add get_protocol_preview in harness

* :release:`5.4.1 <2019-05-06>`
* :bug:`194` Add support for seal capabilities to 384-flat
* :bug:`193` Add support for well properties with non-string values in `wells_with`

* :release:`5.4.0 <2019-03-06>`
* :feature:`191` Add initial cover state to ref opts (ASC-042)
* :feature:`190` Make Well.add_properties extend the original instead of replacing it if both values are lists
* :release:`5.3.0 <2019-02-21>`
* :feature:`188` Add `Protocol` flag to propagate aliquot properties when liquid handling
* :feature:`188` Add `Container` utils for selecting wells
* :feature:`188` Add support for non-string aliquot property values as long as they're JSON-serializable
* :support:`187` Remove Phabricator URI from .arcconfig
* :release:`5.2.1 <2019-01-08>`
* :bug:`186` Fix well volume math when liquid handling in python2 and add missing seal capability for `384-flat-white-clear`
* :feature:`185` Allow `384-flat-white-clear` containers to be sealed with `ultra-clear` seals
* :bug:`183` fix `ThermocycleBuilders.dyes` to reference ints instead of Wells
* :support:`184` Improve CI pipeline and fix lint warnings for new versions of pylint
* :bug:`182` fix `WellGroup` missing equality method
* :release:`5.2.0 <2018-12-11>`
* :feature:`180` add support for `read_position` and `position_z` to `spectrophotometry` (ASC-041)
* :release:`5.1.0 <2018-9-28>`
* :bug:`178 major` fixed passing through of store_lid field in `p.uncover`
* :feature:`177` update `Incubate` instruction and corresponding protocol method `co2` parameter docstrings and add type check
* :release:`5.0.2 <2018-08-28>`
* :bug:`176` increment version
* :release:`5.0.1 <2018-08-28>`
* :bug:`175` fix transfer failing to assign `tip_type` with calibrated transfers that require splitting
* :release:`5.0.0 <2018-08-24>`
* :feature:`172` add new `FlowCytometry` instruction and corresponding protocol method
* :feature:`174` use more sensible default z positions for pre_buffer and blowout in `LiquidHandleMethod`
* :bug:`174 major` fix broken PreMixBlowoutTransfer that used outdated logic
* :feature:`170` protect liquid_handle-related utils until they can be made more general-purpose
* :feature:`170` deprecate unused utils including `euclidean_distance`, `quad_ind_to_num`, and `quad_num_to_ind`
* :feature:`170` port existing checkers to builders format
* :support:`169` add CONTRIBUTING.rst, cleaned up README.md, and ported it to rst
* :feature:`165` add __repr__ methods to Autoprotocol Python objects
* :feature:`165` update instruction serialization to use a new _as_AST method as op is no longer included in Instruction data
* :feature:`165` deprecate `Instruction.json` method for now as most instructions contain non-JSON-serializable objects
* :bug:`167 major` properly handle `transfer` with tip_type and no volume calibration
* :feature:`166` add 384-well flat-bottom polystyrene plate containerType
* :feature:`168` improved pruning of empty data structures from 'Instruction.data' field
* :support:`164` update `docs/requirements.txt` for rtd to build properly
* :feature:`163` add liquid_handle instruction (ASC-032)
* :feature:`163` add LiquidHandleMethods and corresponding protocol methods to represent generic liquid handling abstractions
* :feature:`163` replaced `p.stamp` & `p.transfer` with a new implementation of `p.transfer` that generates a liquid_handle instruction
* :feature:`163` replaced the internals of `p.spread` with a new implementation that generates a liquid_handle instruction
* :feature:`163` deprecated the `p.consolidate` and `p.distribute` protocol methods
* :feature:`163` deprecated Pipette, Stamp, Consolidate, Distribute, and Spread instructions
* :support:`162` fix and update docstrings so that sphinx can be executed with no warnings
* :feature:`161` deprecate support for `p.append` in favor of `p._append_and_return`
* :feature:`161` deprecate support for generating multiple GelSeparate instructions using `p.gel_separate`
* :feature:`161` deprecate `newpick` in `p.autopick`
* :feature:`161` deprecate `util.make_dottable_dict` and `util.deep_merge_params`
* :feature:`161` converted all Unit internals to use Decimals in place of other Numbers
* :support:`161` cleaned up references of `Unit.fromstring` and `Unit._magnitude`
* :feature:`161` added builtin support for `ceil` and `floor` and changed py2 compatibility `Unit.floor` and `Unit.ceil` methods to use them
* :feature:`161` add `spectrophotometry` instruction (ASC-038)
* :feature:`161` add `count_cells` instruction (ASC-033)
* :feature:`161` change `measure_mass` instruction to take in a single container instead (ASC-030)
* :feature:`161` add `store_lid` to `p.uncover` (ASC-040)
* :feature:`161` add `retrieve_lid` to `p.cover` (ASC-040)
* :feature:`161` add parameters to `p.seal`, including `mode`, `temperature`, `duration` (ASC-034)
* :feature:`161` add parameters to `p.luminescence`, including `settle_time`, `integration_time` (ASC-026)
* :feature:`161` add parameters to `p.fluorescence`, including `detection_mode`, `position_z`, `settle_time`, `lag_time`, `integration_time` (ASC-026)
* :feature:`161` add `settle_time` to `p.absorbance` (ASC-026)
* :feature:`161` add `lid_temperature` to `p.thermocycle` (ASC-035)
* :feature:`161` add parameters to `p.dispense`, including `flowrate`, `nozzle_position`, `step_size`, `reagent_source`, `dispense_speed`, `pre_dispense`, `shape`, `shake_after` options (ASC-027, ASC-029, ASC-036, ASC-039)
* :feature:`161` all protocol methods now return the Instruction
* :feature:`161` add `util.check_unit`, a helper for checking the units in bounds
* :feature:`161` add `util.parse_unit`, a helper for parsing and checking an unit input
* :feature:`161` modify `acoustic_transfer` to no longer proactively group consecutive instructions. Please use `WellGroup` explicitly instead
* :feature:`161` add `batch_containers`, for controlling containers entering/exiting together
* :feature:`161` add ideal time constraints which can be specified by `add_time_constraint` (ASC-037)
* :feature:`161` shift `op` as an official attribute of Instruction
* :support:`160` change default linter to pylint and update tox

* :release:`4.0.0 <2017-11-22>`
* :feature:`-` add `ceil` and `floor` methods to `Unit`
* :feature:`-` add shaking capabilities to :meth:`protocol.incubate`
* :feature:`-` add `step_size` to dispense and dispense_full_plate methods
* :feature:`-` add ability to specify a well as reagent source for dispense and dispense_full_plate methods
* :feature:`-` add ability to specify `x_cassette` for dispense and dispense_full_plate methods
* :feature:`-` add support for `more_than` in `add_time_constraint`
* :feature:`-` add PerkinElmer 384-well optiplate to container_type (cat# 6007299), `container-type-384-flat-white-white-optiplate`
* :feature:`-` allow breathable seals on 96-deep and 24-deep
* :feature:`-` add prioritize_seal_or_cover allow priority selection
* :support:`-` docstring cleanup, linting
* :bug:`- major` remove cover prior to mag steps where applicable
* :support:`-` convert test suite to py.test
* :feature:`-` add new containers, true_max_vol_ul in _CONTAINER_TYPES
* :support:`-` fix documentation typos

* :release:`3.10.1 <2017-05-25>`
* :bug:`-` update pint requirements, update error handling on UnitError
* :bug:`-` update default lid types for `container-type-384-echo`, `container-type-96-flat`, `container-type-96-flat-uv`, and `container-type-96-flat-clear-clear-tc`

* :release:`3.10.0 <2016-10-25>`
* :support:`-` add functions and tests to enable use of `--dye_test` flag
* :support:`-` more descriptive error message in ref protocol
* :bug:`- major` fix name of `container-type-384-round-clear-clear`
* :feature:`-` new plate types `container-type-384-v-clear-clear`, `container-type-384-round-clear-clear`,`384-flat-white-white-nbs`
* :bug:`- major` fix Well.set_properties() so that it completely overwrites the existing properties dict
* :bug:`- major` respect incubate conditions where uncovered=True
* :bug:`- major` prevent invalid incubate parameters in `protocol-absorbance`
* :bug:`- major` allow incubation of containers at ambient without covers

* :release:`3.9.0 <2016-08-10>`
* :feature:`-` new plate type `container-type-96-flat-clear-clear-tc`
* :feature:`-` Container method: `container-tube`
* :support:`-` update documention for `harness-seal-on-store`
* :bug:`- major` Unit validations from str in `protocol-flow-analyze` instruction

* :release:`3.8.0 <2016-07-26>`
* :bug:`- major` unit conversion to microliters in `protocol-dispense` instruction
* :support:`-` using release for changelog and integration into readthedocs documentation

* :release:`3.7.6 <2016-07-25>`
* :bug:`-` dispense_speed and distribute_target in `protocol-distribute` instruction
* :bug:`127` convert pipette operations to microliters
* :bug:`128` cover_types on `container-type-96-deep-kf` and `container-type-96-deep`
* :bug:`-` convert pipette operations to microliters

* :release:`3.7.5 <2016-07-08>`
* :feature:`- backported` plate type `container-type-6-flat-tc` to ContainerType

* :release:`3.7.4 <2016-07-07>`
* :bug:`-` auto-uncover before `protocol-provision` instructions

* :release:`3.7.3 <2016-07-06>`
* :feature:`- backported` `is_resource_id` added to `protocol-dispense` and `protocol-dispense-full-plate` instructions
* :support:`-` `protocol-dispense` instruction tests
* :feature:`- backported` autocover before `protocol-incubate`
* :feature:`- backported` assertions and tests for `protocol-flow-analyze`
* :feature:`- backported` WellGroup methods: `wellgroup-group-name`, `wellgroup-pop`, `wellgroup-insert`, `wellgroup-wells-with`
* :support:`- backported` documentation
* :feature:`- backported` WellGroup.extend(wells) can now take in a list of wells
* :bug:`-` `protocol-dispense` instruction json outputs
* :bug:`-` removed capability 'cover' from `container-type-96-pcr` and `container-type-384-pcr` plates
* :bug:`-` `protocol-spin` auto-cover
* :bug:`-` compatibility with py3 in `protocol-flow-analyze`

* :release:`3.7.2 <2016-06-24>`
* :feature:`- backported` validations before implicit cover or seal
* :feature:`- backported` new plate types `container-type-384-flat-clear-clear`, `container-type-384-flat-white-white-lv`, `container-type-384-flat-white-white-tc`

* :release:`3.7.1 <2016-06-17>`
* :feature:`- backported` validations of input types before cover check
* :feature:`- backported` cover_types and seal_types to _CONTAINER_TYPES
* :bug:`-` string input types for source, destination wells for Instructions `protocol-consolidate`, `protocol-autopick`, `protocol-mix`

* :release:`3.7.0 <2016-06-14>`
* :feature:`-` track plate cover status - Container objects now have a `cover` attribute, implicit plate unsealing or uncovering prior to steps that require the plate to be uncovered.
* :bug:`- major` `protocol-stamp` separates row stamps with more than 2 containers

* :release:`3.6.0 <2016-06-07>`
* :feature:`-` `protocol-add-time-constraint` added
* :feature:`-` `protocol-illuminaseq` allows cycle specification

* :release:`3.5.3 <2016-05-16>`
* :bug:`-` harness.py returns proper boolean for thermocycle types

* :release:`3.5.2 <2016-05-13>`
* :feature:`- backported` `unit-unit` specific error handling
* :bug:`-` thermocycle gradient steps in harness.py

* :release:`3.5.1 <2016-05-12>`
* :feature:`- backported` `protocol-mix` allows one_tip=True
* :bug:`-` `protocol-acoustic-transfer` handling of droplet size

* :release:`3.5.0 <2016-05-06>`
* :feature:`-` `protocol-measure-mass` instruction
* :feature:`-` `protocol-measure-volume` instruction
* :feature:`-` `protocol-illuminaseq` instruction
* :feature:`-` `protocol-gel-purify` parameters improved
* :feature:`-` `protocol-spin` instruction takes directional parameters
* :bug:`- major` WellGroup checks that all elements are wells
* :bug:`- major` Concatenation of Well to WellGroup no longer returns None
* :support:`-` gel string in documentation
* :bug:`- major` fix harness to be python3 compatible
* :bug:`- major` Compatibility of Unit for acceleration

* :release:`3.4.0 <2016-04-22>`
* :feature:`-` :ref:container-discard` and and `container-set-storage` methods for containers
* :feature:`-` `protocol-gel-purify` instruction to instruction.py and protocol.py
* :feature:`-` support for list input type for humanize and robotize (container and container_type)

* :release:`3.3.0 <2016-04-13>`
* :feature:`-` csv-table input type to harness.py

* :release:`3.2.0 <2016-04-07>`
* :feature:`-` additional parameter, `gain`, to `protocol-fluorescence`
* :feature:`-` checking for valid plate read incubate parameters
* :feature:`-` Unit(Unit(...)) now returns a Unit
* :feature:`-` disclaimer to README.md on unit support
* :feature:`-` Unit support for `molar`
* :support:`-` adding magnetic transfer functions to documentation
* :feature:`-` magnetic transfer instructions to now pass relevant inputs through units
* :support:`-` documentation for magnetic transfer instructions correctly uses hertz

* :release:`3.1.0 <2016-03-24>`
* :feature:`-` additional parameters to spectrophotometry instructions (`protocol-absorbance`, `protocol-luminescence`, `protocol-fluorescence`) to instruction.py and protocol.py
* :feature:`-` helper function in util.py to create incubation dictionaries
* :feature:`-` support for a new instruction for `protocol-measure-concentration`
* :bug:`- major` Updated handling of multiplication and division of Units of the same dimension to automatically resolve when possible
* :bug:`- major` Updated maximum tip capacity for a transfer operation to 900uL instead of 750uL
* :bug:`- major` Updated Unit package to default to `Autoprotocol` format representation for temperature and speed units

* :release:`3.0.0 <2016-03-17>`
* :feature:`-` `container+` input type to harness.py
* :feature:`-` `magnetic_transfer` instruction to instruction.py and protocol.py
* :feature:`-` kf container types `container-type-96-v-kf` and `container-type-96-deep-kf` in container_type.py
* :feature:`-` release versioning has been removed in favor of protocol versioniong in harness.py
* :feature:`-` update `container-type-6-flat` well volumes
* :feature:`-` `unit-unit` now uses Pint's Quantity as a base class
* :bug:`- major` default versioning in manifest_test.json
* :bug:`- major` Update container_test.py and container_type_test.py to include safe_min_volume_ul

* :release:`2.7.0 <2016-02-18>`
* :feature:`-` safe_min_volume_ul in _CONTAINER_TYPES
* :feature:`-` updated dead_volume_ul values in _CONTAINER_TYPES
* :bug:`- major` `protocol-stamp` smartly calculates max_tip_volume using residual volumes

* :release:`2.6.0 <2015-02-02>`
* :feature:`-` Include well properties in outs
* :feature:`-` `wellgroup-extend` method to WellGroup
* :feature:`-` Allow single Well reading for Absorbance, Fluorescence and Luminescence
* :feature:`-` `protocol-autopick` now conforms to updated ASC (**not backwards compatible**)
* :support:`-` Protocol.plate_to_magblock() and Protocol.plate_from_magblock()
* :bug:`- major` Protocol.stamp() allows one_tip=True when steps use a `mix_vol` greater than "31:microliter" even if transferred volumes are not all greater than "31:microliter"
* :bug:`- major` `protocol-transfer` respects when `mix_after` or `mix_before` is explicitly False

* :release:`2.5.0 <2015-10-12>`
* :feature:`-` `protocol-stamp` has been reformatted to take groups of transfers. This allows for one_tip=True, one_source=True, and WellGroup source and destinations

* :release:`2.4.1 <2015-10-12>`
* :bug:`-` volume tracking for `protocol-stamp` ing to/from 384-well plates
* :bug:`-` one_tip = True transfers > 750:microliter are transferred with single tip

* :release:`2.4.0 <2015-09-28>`
* :feature:`-` UserError exception class for returning custom errors from within protocol scripts
* :feature:`-` functionality to harness.py for naming aliquots
* :support:`-` `protocol-stamp` transfers are not combinable if they use different tip volume types
* :support:`-` Transfers with one_source true does not keep track of the value of volume less than 10^-12
* :bug:`- major` Small bug for transfer with one_source=true fixed
* :bug:`- major` Better handling of default append=true behavior for `protocol-stamp`
* :bug:`- major` more recursion in `make_dottable_dict`, a completely unnecessary function you shouldn't use

* :release:`2.3.0 <2015-08-31>`
* :feature:`-` `protocol-stamp` now support selective (row-wise and column-wise) stamping (see docstring for details)

* :release:`2.2.2 <2015-08-28>`
* :feature:`- backported` Storage attribute on Container
* :feature:`- backported` Protocol.store()
* :feature:`- backported` manually change storage condition destiny of a Container
* :feature:`- backported` Test for more complicated `transfer`ing with `one_source=True`
* :feature:`- backported` Better error handling in harness.py and accompanying tests
* :feature:`- backported` Arguments to `protocol-transfer` for `mix_before` and `mix_after` are now part of **mix_kwargs** to allow for specifying separate parameters for mix_before and mix_after
* :bug:`-` Error with `transfer`ing with `one_source=True`

* :release:`2.2.1 <2015-08-20>`
* :feature:`- backported` volume tracking to `protocol-stamp` and associated helper functions in autoprotocol.util
* :support:`- backported` semantic versioning fail
* :feature:`- backported` name property on Well
* :feature:`- backported` "outs" section of protocol.  Use `well-set-name` to name an aliquot
* :feature:`- backported` unit conversion from milliliters or nanoliters to microliters in `Well.set_volume()`, `protocol-provision`, `protocol-transfer`, and `protocol-distribute`
* :bug:`-` Error with `protocol-provision` ing to multiple wells of the same container
* :bug:`-` Error when `protocol-transfer` ing over 750uL
* :bug:`-` Unit scalar multiplication

* :release:`2.2.0 <2015-07-21>`
* :feature:`-` `Stamp` class in autoprotocol.instruction
* :feature:`-` volume tracking to destination wells when using Protocol.dispense()
* :feature:`-` `__repr__` override for Unit class
* :feature:`-` `protocol-stamp` now utilizes the new Autoprotocol `stamp` instruction instead of `protocol-transfer`
* :bug:`- major` fixed indentation
* :bug:`- major` refactored Protocol methods: `protocol-ref`, `protocol-consolidate`, `protocol-transfer`, `protocol-distribute`
* :bug:`- major` better error handling for `protocol-transfer` and `protocol-distribute`

* :release:`2.1.0 <2015-06-10>`
* :feature:`-` `protocol-flash-freeze` Protocol method and Instruction
* :feature:`-` `criteria` and `dataref` fields to `protocol-autopick`
* :feature:`-` `protocol-sangerseq` now accepts a sequencing `type` of `"rca"` or `"standard"` (defaults to "standard")
* :feature:`-` collapse `protocol-provision` instructions if they're acting on the same container
* :support:`-` Protocol.thermocycle_ramp()
* :support:`-` Protocol.serial_dilute_rowwise()
* :bug:`- major` type check in Container.wells
* :bug:`- major` `protocol-ref` behavior when specifying the `id` of an existing container

* :release:`2.0.5 <2015-06-04>`
* :support:`- backported` Added folder for sublime text snippets
* :feature:`- backported` volume adjustment when `protocol-spread` ing
* :feature:`- backported` `ImagePlate()` class and `protocol-image-plate` Protocol method for taking images of containers
* :feature:`- backported` add `protocol-consolidate` Protocol method and accompanying tests
* :feature:`- backported` support for container names with slashes in them in `harness.py`
* :feature:`- backported` `container-type-1-flat` plate type to `_CONTAINER_TYPES`
* :feature:`- backported` brought back recursively transferring volumes over 900 microliters
* :feature:`- backported` allow transfer from multiple sources to one destination
* :feature:`- backported` support for `choice` input type in `harness.py`
* :feature:`- backported` `protocol-provision` Protocol method
* :feature:`- backported` Additional type-checks in various functions
* :feature:`- backported` More Python3 Compatibility
* :support:`- backported` check that a well already exists in a WellGroup
* :bug:`-` typo in `protocol-sangerseq` instruction
* :support:`- backported` documentation punctuation and grammar

* :release:`2.0.4 <2015-05-05>`
* :feature:`- backported` More Python3 Compatibility
* :feature:`- backported` specify `Wells` on a container using `container.wells(1,2,3)`or `container.wells([1,2,3])`
* :feature:`- backported` Thermocycle input type in `harness.py`
* :feature:`- backported` `new_group` keyword parameter on `protocol-transfer` and `protocol-distribute` to manually break up `Pipette()` Instructions
* :support:`- backported` documentation for `plate_to_mag_adapter` and `plate_from_mag_adapter` **subject to change in near future**
* :feature:`- backported` tox for testing with multiple versions of python
* :feature:`- backported` `protocol-gel-separate` generates instructions taking wells and matrix type passed
* :feature:`- backported` `protocol-stamp` ing to or from multiple containers now requires that the source or dest variable be passed as a list of `[{"container": <container>, "quadrant": <quadrant>}, ...]`
* :bug:`-` references to specific reagents for `protocol-dispense`
* :bug:`-` Transfering liquid from `one_source` actually works now

* :release:`2.0.3 <2015-04-17>`
* :feature:`- backported` At least some Python3 compatibility
* :feature:`- backported` Well.properties is an empty hash by default
* :feature:`- backported` `well-add-properties`
* :feature:`- backported` `container-quadrant` returns a WellGroup of the 96 wells representing the quadrant passed
* :feature:`- backported` `96-flat-uv` container type in `_CONTAINER_TYPES`
* :feature:`- backported` `6-flat` container type in `_CONTAINER_TYPES`
* :feature:`- backported` co2 parameter in `protocol-incubate`
* :feature:`- backported` `protocol-flow-analyze` Instruction
* :feature:`- backported` `protocol-spread` Instruction
* :feature:`- backported` `protocol-autopick` Instruction
* :feature:`- backported` `protocol-oligosynthesize` Instruction
* :feature:`- backported` Additional keyword arguments for `protocol-transfer` and `protocol-distribute` to customize pipetting
* :feature:`- backported` Added `pipette_tools` module containing helper methods for the extra pipetting parameters
* :feature:`- backported` `protocol-stamp` Protocol method for using the 96-channel liquid handler
* :feature:`- backported` more tests
* :feature:`- backported` seal takes a "type" parameter that defaults to ultra-clear
* :feature:`- backported` `protocol-sangerseq` Instruction and method
* :feature:`- backported` `Protocol.pipette()` is now a private method `_pipette()`
* :bug:`-` refactoring of type checks in `unit-unit`
* :support:`- backported` improved documentation tree
* :bug:`-` references to specific matrices and ladders in `protocol-gel-separate`
* :bug:`-` recursion to deal with transferring over 900uL of liquid
* :bug:`-` `protocol-gel-separate` generates number of instructions needed for number of wells passed

* :release:`2.0.2 <2015-03-06>`
* :support:`- backported` autoprotocol and JSON output examples for almost everything in docs
* :support:`- backported` link to library documentation at readthedocs.org to README
* :feature:`- backported` default input value and group and group+ input types in `harness.py`
* :feature:`- backported` melting keyword variables and changes to conditionals in Thermocycle
* :support:`- backported` a wild test appeared!

* :release:`2.0.1 <2015-02-06>`
* :feature:`- backported` properties attribute to `Well`, along with `well-set-properties` method
* :feature:`- backported` aliquot++, integer, boolean input types to harness.py
* :feature:`- backported` `protocol-dispense` Instruction and accompanying Protocol method for using a reagent dispenser
* :feature:`- backported` `protocol-dispense-full-plate`
* :feature:`- backported` warnings for `_mul_` and `_div_` scalar Unit operations
* :support:`- backported` README.rst
* :bug:`-` "speed" parameter in `protocol-spin` to "acceleration"
* :bug:`-` `well_type` from `_CONTAINER_TYPES`
* :bug:`-` spelling of luminescence :(

* :release:`2.0.0 <2014-01-24>`
* :feature:`-` harness.py for parameter conversion
* :support:`-` NumPy style docstrings for most methods
* :feature:`-` `container-inner-wells` method to exclude edges
* :feature:`-` 3-clause BSD license, contributor info
* :feature:`-` `wellGroup-indices` returns a list of string well indices
* :feature:`-` dead_volume_ul in _CONTAINER_TYPES
* :feature:`-` volume tracking upon `protocol-transfer` and `protocol-distribute`
* :feature:`-` "one_tip" option on `protocol-transfer`
* :support:`-` static methods `Pipette.transfers()` and `Pipette._transferGroup()`

* :release:`1.0.0 <2014-01-22>`
* :feature:`-` initializing ap-py
