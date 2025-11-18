# `POPxf`: An Exchange Format for Polynomial Observable Predictions

The Polynomial Observable Prediction Exchange Format, `POPxf`, is a structured, machine-readable data format for the publication and exchange of semi-analytical theoretical predictions in high energy physics. The format is designed to encode observables that can be expressed in terms of polynomials in model parameters, with particular emphasis on Effective Field Theory applications. All relevant assumptions and metadata are recorded explicitly, and the treatment of uncertainties and correlations is flexible enough to capture parameter-dependent effects. The format aims to improve reproducibility, facilitate global fits and reinterpretations, and streamline the use of theoretical predictions across the particle physics community.

## Key Features

- General applicability to any observable that can be expressed in terms of a polynomial in model parameters, including but not limited to EFT Wilson coefficients.
- Support for arbitrary polynomial order, enabling the inclusion of higher-order terms such as those arising from dimension-eight EFT operators.
- Support for sectors of related observables, such as binned distributions, angular observables, or correlated decay channels.
- Support for observables defined as functions of one or multiple polynomial parameterisations, such as normalised distributions or ratios of decay widths.
- Explicit encoding of all assumptions, such as parameter basis definitions, input parameter values, renormalisation scale, and operator normalisations, to ensure reproducibility.
- Consistent treatment of theoretical uncertainties from various sources, including support for parameter-dependent uncertainties.
- Support for correlated uncertainties between observables, including the possibility of parameter-dependent correlations.
- Based on the `JSON` standard, a lightweight, text-based data format that is both human-readable and natively supported in most programming languages and computer algebra systems.

## `JSON` Schema

The `JSON` Schema defining the `POPxf` data format and its documentation can be found in the [json-schemas](https://github.com/pop-xf/json-schemas) repository.

## Validator and Parser

A lightweight validator and parser for `POPxf` files can be found in the [parser](https://github.com/pop-xf/parser) repository.

## Examples

Examples of POPxf files can be found in the [examples](https://github.com/pop-xf/examples) repository.

## Publication

The publication introducing and describing the `POPxf` data format is currently available as a [draft on the CERN Document Server](https://cds.cern.ch/record/2946482).
