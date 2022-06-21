# Motivation
- restrictive (corporate) firewall that doesn't allow to access clojars (or maven).
- using `deps.edn` because on Windows it's difficult to provide artifact-coordinates via command-line.

# Introduction
Bundle dependencies on a computer that has access to maven and clojars (PC-A) and bring these over to a computer with limited access (PC-L).

# Requirements
- PC-A: babashka (bb)
  - https://github.com/babashka/babashka#installation

# Instructions
- PC-A: Modify `deps.edn` to contain the dependencies you need.
- PC-A: Call `bb zip <zipname>` to create the ZIP-file, omitting the extension `.zip`.
- Bring the zip over.
- PC-L: unpack into local maven-repository.

