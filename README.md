# Platform Team: Kryptos AI Context

Kryptos team-level Copilot instructions for repositories that own secrets infrastructure and cryptographic controls.

## Setup

Load this repository with the platform group instructions:

```bash
export COPILOT_CUSTOM_INSTRUCTIONS_DIRS="\
$HOME/repositories/osinfra-io/platform-group/pt-ai-context,\
$HOME/repositories/osinfra-io/platform-group/kryptos/pt-kryptos-ai-context"
```

The platform layer supplies shared conventions. Kryptos instructions add the ownership boundary between Pneuma-managed cluster runtime and Kryptos-managed OpenBao services.
