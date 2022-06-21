# Requirements
- babashka (bb)
  - https://github.com/babashka/babashka#installation

# Instructions
- Modify `deps.edn` to contain the dependencies you need.
- Call `bb zip <zipname>` to create the ZIP-file, omitting the extension `.zip`.
- Bring the zip over.

# Motivation
- restrictive (corporate) firewall that doesn't allow to access clojars (or maven).
- using `deps.edn` because on Windows it's difficult to provide artifact-coordinates via command-line.

