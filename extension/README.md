# CodeChronicle

AI-powered codebase analysis for VS Code with interactive dependency graphs, blast radius prediction, risk scoring, and natural-language exploration.

## What It Does

- **Dependency Graph**: Visualize files and imports in an interactive graph.
- **Blast Radius**: See direct and transitive impact before editing a file.
- **AI Summaries**: Generate file and relationship summaries using Bedrock.
- **AI Query**: Ask codebase questions in plain English.
- **Risk Map**: View structural + AI risk and export risk reports.
- **Free to Use**: All AI features are free with no credits, payments, or usage limits.

## Getting Started

1. Install CodeChronicle from VS Code Marketplace.
2. Sign in from extension sidebar/auth panel.
3. Open any project folder.
4. Run **CodeChronicle: Scan Workspace**.
5. Open **CodeChronicle: Open Graph View** and use Graph/Blast Radius/AI Query/Risk tabs.

## Commands

| Command | Description |
|---|---|
| `CodeChronicle: Scan Workspace` | Scan workspace and build dependency graph |
| `CodeChronicle: Open Graph View` | Open graph webview |
| `CodeChronicle: Ask AI About Codebase` | Open AI query workflow |
| `CodeChronicle: Predict Blast Radius` | Compute change impact |
| `CodeChronicle: Refresh Analysis` | Re-scan and refresh graph |
| `CodeChronicle: Sign In` | Open auth UI |
| `CodeChronicle: Sign Out` | Log out from extension |

## Extension Settings

| Setting | Description | Default |
|---|---|---|
| `codechronicle.enableCloudAI` | Enable cloud AI features | `true` |
| `codechronicle.awsApiEndpoint` | Backend API Gateway endpoint | `https://usl085fgve.execute-api.us-east-1.amazonaws.com` |
| `codechronicle.awsRegion` | AWS region | `us-east-1` |
| `codechronicle.maxFiles` | Max files to analyze | `10000` |
| `codechronicle.excludePatterns` | Exclusion globs | common build/vendor folders |
| `codechronicle.supportedExtensions` | Supported file extensions | JS/TS/Python/Java/C#/Go/Rust/etc. |

## Privacy

- Graph/metrics/blast-radius analysis runs locally.
- Cloud AI features send bounded context to backend.
- Cached AI outputs are TTL-based, not stored indefinitely.

## License

MIT
