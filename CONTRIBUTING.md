# Contributing to LLM Stats

Thank you for your interest in contributing. This guide outlines the process for updating and adding information to the LLM Stats database.

## Table of Contents

- [Overview](#overview)
- [Data Structure](#data-structure)
- [General Guidelines](#general-guidelines)
- [Organizations](#organizations)
- [Models](#models)
- [Benchmark Results](#benchmark-results)
- [Benchmarks](#benchmarks)
- [Providers](#providers)
- [Licenses](#licenses)
- [Validation](#validation)
- [Submitting Your Contribution](#submitting-your-contribution)

## Overview

All data is organized in the `data/data/` directory with a hierarchical structure. Each entity type has its own JSON schema definition in `schemas/` that validates the data structure.

## Data Structure

```
data/
├── data/
│   ├── organizations/
│   │   └── [organization_id]/
│   │       ├── organization.json
│   │       └── models/
│   │           └── [model_id]/
│   │               ├── model.json
│   │               └── benchmarks.json
│   ├── providers/
│   │   └── [provider_id]/
│   │       ├── provider.json
│   │       └── models.json
│   ├── licenses/
│   │   └── [license_id].json
│   └── benchmarks/
│       └── [benchmark_id].json
└── schemas/
    ├── organization.schema.json
    ├── model.schema.json
    ├── benchmark-results.schema.json
    ├── benchmark.schema.json
    ├── provider.schema.json
    ├── provider-models.schema.json
    └── license.schema.json
```

## General Guidelines

1. **Accuracy First**: Ensure all data is accurate and sourced from authoritative references
2. **Follow Structure**: Adhere to the existing file structure and naming conventions
3. **Consistent Formatting**: Use consistent JSON formatting with 2-space indentation
4. **One Change per PR**: Submit one pull request per logical change (e.g., one model, one provider)
5. **Schema Validation**: All data files must validate against their respective JSON schemas
6. **Required Fields**: Pay attention to required vs optional fields in schemas
7. **Timestamps**: Use ISO 8601 format for dates (YYYY-MM-DD or full timestamp)

## Organizations

Organizations represent the entities that create and release models (e.g., OpenAI, Anthropic, Meta).

### Location

`data/data/organizations/[organization_id]/organization.json`

### Adding a New Organization

1. Create a new directory: `data/data/organizations/[organization_id]/`
2. Create `organization.json` with the following structure:

```json
{
  "organization_id": "organization-name",
  "name": "Organization Display Name",
  "website": "https://organization.com",
  "description": "Brief description of the organization",
  "country": "US",
  "created_at": "2025-10-02T00:00:00.000000+00:00",
  "updated_at": "2025-10-02T00:00:00.000000+00:00"
}
```

3. Validate against `schemas/organization.schema.json`
4. Create a `models/` subdirectory for future models

### Updating an Existing Organization

1. Navigate to `data/data/organizations/[organization_id]/organization.json`
2. Update the relevant fields
3. Update the `updated_at` timestamp
4. Validate against the schema

## Models

Models are stored within their respective organization directories.

### Location

`data/data/organizations/[organization_id]/models/[model_id]/`

### Adding a New Model

1. Ensure the organization exists in `data/data/organizations/`
2. Ensure the license exists in `data/data/licenses/`
3. Create a new directory: `data/data/organizations/[organization_id]/models/[model_id]/`
4. Create two files in this directory:

#### `model.json`

```json
{
  "model_id": "model-name-version",
  "name": "Model Display Name",
  "organization_id": "organization-name",
  "fine_tuned_from_model_id": null,
  "description": "Detailed description of the model's capabilities",
  "release_date": "2024-10-22",
  "announcement_date": "2024-10-22",
  "license_id": "proprietary",
  "multimodal": false,
  "knowledge_cutoff": "2024-04-01",
  "param_count": 7000000000,
  "training_tokens": 15000000000000,
  "available_in_zeroeval": true,
  "source_api_ref": "https://...",
  "source_playground": "https://...",
  "source_paper": "https://...",
  "source_scorecard_blog_link": "https://...",
  "source_repo_link": "https://github.com/...",
  "source_weights_link": "https://huggingface.co/...",
  "created_at": "2025-10-02T00:00:00.000000+00:00",
  "updated_at": "2025-10-02T00:00:00.000000+00:00",
  "model_family_id": null
}
```

**Required Fields**: `model_id`, `name`, `organization_id`, `release_date`, `license_id`, `multimodal`

**Optional Fields**: Set to `null` if not applicable

#### `benchmarks.json`

Start with an empty array if no benchmark results are available yet:

```json
[]
```

5. Validate both files against their respective schemas

### Updating an Existing Model

1. Navigate to `data/data/organizations/[organization_id]/models/[model_id]/model.json`
2. Update the relevant fields
3. Update the `updated_at` timestamp
4. Validate against `schemas/model.schema.json`

## Benchmark Results

Benchmark results are stored in the `benchmarks.json` file within each model directory.

### Location

`data/data/organizations/[organization_id]/models/[model_id]/benchmarks.json`

### Adding Benchmark Results

1. Ensure the benchmark exists in `data/data/benchmarks/`
2. Ensure the model exists
3. Add a new entry to the `benchmarks.json` array:

```json
[
  {
    "benchmark_id": "mmlu",
    "score": 85.5,
    "score_unit": "percentage",
    "source_link": "https://example.com/results",
    "created_at": "2025-10-02T00:00:00.000000+00:00",
    "updated_at": "2025-10-02T00:00:00.000000+00:00"
  }
]
```

4. Validate against `schemas/benchmark-results.schema.json`

### Updating Benchmark Results

1. Locate the specific result in the array
2. Update the `score` and/or `source_link`
3. Update the `updated_at` timestamp
4. Ensure the `source_link` is reliable and authoritative

## Benchmarks

Benchmarks define the evaluation tests used to measure model performance.

### Location

`data/data/benchmarks/[benchmark_id].json`

### Adding a New Benchmark

1. Create a new file: `data/data/benchmarks/[benchmark_id].json`
2. Follow this structure:

```json
{
  "benchmark_id": "benchmark-name",
  "name": "Benchmark Display Name",
  "description": "Description of what this benchmark measures",
  "category": "reasoning",
  "source_link": "https://...",
  "created_at": "2025-10-02T00:00:00.000000+00:00",
  "updated_at": "2025-10-02T00:00:00.000000+00:00"
}
```

3. Validate against `schemas/benchmark.schema.json`

## Providers

Providers are services that offer access to models (e.g., OpenAI API, AWS Bedrock, Google Vertex AI).

### Location

`data/data/providers/[provider_id]/`

### Adding a New Provider

1. Create a new directory: `data/data/providers/[provider_id]/`
2. Create two files:

#### `provider.json`

```json
{
  "provider_id": "provider-name",
  "name": "Provider Display Name",
  "website": "https://provider.com",
  "created_at": "2025-10-02T00:00:00.000000+00:00",
  "updated_at": "2025-10-02T00:00:00.000000+00:00"
}
```

#### `models.json`

Start with an empty array:

```json
[]
```

3. Validate both files against their respective schemas

### Updating Provider Information

1. Navigate to `data/data/providers/[provider_id]/provider.json`
2. Update the relevant fields
3. Update the `updated_at` timestamp

### Adding Provider Models

Provider models specify pricing and availability of models through specific providers.

1. Open `data/data/providers/[provider_id]/models.json`
2. Add a new entry to the array:

```json
[
  {
    "provider_model_id": "provider-specific-id",
    "model_id": "actual-model-id",
    "provider_id": "provider-name",
    "input_price_per_million": 3.0,
    "output_price_per_million": 15.0,
    "context_window": 200000,
    "max_output_tokens": 4096,
    "available": true,
    "created_at": "2025-10-02T00:00:00.000000+00:00",
    "updated_at": "2025-10-02T00:00:00.000000+00:00"
  }
]
```

3. Ensure the model exists in `data/data/organizations/[org]/models/[model_id]/`
4. Validate against `schemas/provider-models.schema.json`

## Licenses

Licenses define the terms under which models can be used.

### Location

`data/data/licenses/[license_id].json`

### Adding a New License

1. Create a new file: `data/data/licenses/[license_id].json`
2. Follow this structure:

```json
{
  "license_id": "license-name",
  "name": "License Display Name",
  "url": "https://...",
  "commercial_use": true,
  "created_at": "2025-10-02T00:00:00.000000+00:00",
  "updated_at": "2025-10-02T00:00:00.000000+00:00"
}
```

3. Validate against `schemas/license.schema.json`

## Validation

Before submitting your contribution:

### Manual Validation

Run the validator script from the `data/` directory:

```bash
cd data
node schemas/validator.js
```

This will check all JSON files against their respective schemas.

### What the Validator Checks

- JSON syntax correctness
- Required fields are present
- Field types match schema definitions
- ID references exist (e.g., organization_id, license_id)
- Date formats are valid
- URLs are properly formatted

### Common Validation Errors

1. **Missing Required Fields**: Ensure all required fields are present
2. **Invalid Date Format**: Use ISO 8601 format (YYYY-MM-DD or full timestamp)
3. **Invalid References**: Ensure referenced IDs exist (organization_id, license_id, etc.)
4. **Type Mismatch**: Ensure numbers are numbers, strings are strings, etc.
5. **Trailing Commas**: Remove trailing commas in JSON arrays/objects

## Submitting Your Contribution

1. **Fork the Repository**: Create your own fork of the project
2. **Create a Branch**: Use a descriptive branch name (e.g., `add-gpt5-model`, `update-claude-pricing`)
3. **Make Changes**: Follow the guidelines above
4. **Validate Locally**: Run `node schemas/validator.js` to ensure your changes are valid
5. **Commit Changes**: Write clear, descriptive commit messages
6. **Submit a Pull Request**:
   - Provide a clear title and description
   - List what was added or changed
   - Include links to authoritative sources
   - Reference any related issues

### Pull Request Template

```markdown
## Description

Brief description of what this PR adds or changes

## Changes

- Added/Updated model: [Model Name]
- Added/Updated organization: [Organization Name]
- Added benchmark results for: [Benchmark Name]

## Sources

- [Source 1]: https://...
- [Source 2]: https://...

## Validation

- [ ] Ran `node schemas/validator.js` successfully
- [ ] All files follow the correct structure
- [ ] All references (organization_id, license_id) are valid
```

### Example Pull Request

For reference, see this [example pull request](https://github.com/JonathanChavezTamales/llm-leaderboard/pull/1).

## Questions?

If you have questions or need clarification, please:

1. Check the schema files in `schemas/` for detailed field definitions
2. Look at existing data files as examples
3. Open an issue on GitHub

Thank you for contributing to LLM Stats!
