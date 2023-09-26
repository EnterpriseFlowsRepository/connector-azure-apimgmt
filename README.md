# Introduction

This projet contains a connector to EFR from Azure API Management.

# Installation

1. Add a fragment EFRTrace
content is src/Fragment.xml

2. Add Named Values:

|Name|Value|Description|
|||||||
|environment|production|name of this environment|

# Usage

In your policy, add variables to describe your mediation:

```xml

```

Call EFR in your policy:

```xml

```

# Configuration into Enterprise Flows Repository

1. Add a Flow:
- name: APIM <API name>

2. Add a mediation for each API operation to supervize:
- name: APIM<API name><API version>-<operation name>
- RegEx: <API name><API version>-<operation name>.*

2. Complete list of mediations into Flow:
- select mediation created.
