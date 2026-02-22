# Homebrew Tap for TidyFiles

AI-powered file organizer using rules + Claude Haiku.

## Installation

```bash
brew tap ayhid/tidyfiles
brew install tidyfiles
```

## Usage

```bash
# Dry-run scan
tidyfiles scan ~/Downloads

# Interactive TUI
tidyfiles tui ~/Downloads

# Organize with confirmation
tidyfiles organize ~/Downloads

# Undo last operation
tidyfiles undo
```

## Configuration

Set your Anthropic API key for AI classification of ambiguous files:

```bash
export ANTHROPIC_API_KEY="sk-ant-..."
```

Without the key, ambiguous files default to the "Other" category.
Extension-based classification (~85% of files) works without an API key.
