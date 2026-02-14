# Bazel workshop lab (Codespaces-friendly)

This repo contains small hands-on labs that you can run in GitHub Codespaces.

## Lab 01: select() + platforms

Broken version:
  labs/lab01_select_platform/broken

Solution (one possible fix):
  labs/lab01_select_platform/solution

Run from repo root:

Broken, linux (succeeds):
  bazel build //labs/lab01_select_platform/broken:report --platforms=//platforms:linux

Broken, mac (fails):
  bazel build //labs/lab01_select_platform/broken:report --platforms=//platforms:mac

After you fix the broken lab, both commands should succeed.

Compare with the provided solution:
  bazel build //labs/lab01_select_platform/solution:report --platforms=//platforms:mac
