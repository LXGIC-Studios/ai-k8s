# ai-k8s

[![npm version](https://img.shields.io/npm/v/ai-k8s.svg)](https://www.npmjs.com/package/ai-k8s)
[![npm downloads](https://img.shields.io/npm/dm/ai-k8s.svg)](https://www.npmjs.com/package/ai-k8s)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![GitHub stars](https://img.shields.io/github/stars/lxgic-studios/ai-k8s)](https://github.com/lxgic-studios/ai-k8s/stargazers)
[![TypeScript](https://img.shields.io/badge/TypeScript-5.0+-blue)](https://www.typescriptlang.org/)



Got a docker-compose file and need to move to Kubernetes? Don't spend hours translating YAML by hand. Just feed it in and get proper K8s manifests back.

## Install

```bash
npm install -g ai-k8s
```

## Usage

```bash
# From a docker-compose file
npx ai-k8s docker-compose.yml --namespace production

# From a description
npx ai-k8s "3 replicas of a node app with redis and postgres"

# Save output
npx ai-k8s docker-compose.yml -o k8s-manifests.yml
```

## Setup

```bash
export OPENAI_API_KEY=your-key-here
```

## Options

- `-n, --namespace <ns>` - Target namespace (defaults to "default")
- `-o, --output <file>` - Write to a file

## License

MIT
