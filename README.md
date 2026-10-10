# Tax Calculator DevOps — Tekton

This repository contains the Tekton manifests for the tax-calculator coursework.

- `tasks.yaml`: npm install and Jasmine test tasks
- `pipeline.yaml`: source clone, dependencies, Jasmine tests, Kaniko container build and push
- `run.yaml`: PipelineRun configured for this repository

**Before running:** Add the actual tax-calculator application files (Dockerfile, package.json, sources and tests), replace the placeholder IBM Container Registry namespace in run.yaml, install Tekton's git-clone Task, and create the Kubernetes secret `icr-docker-config` with valid registry credentials. These manifests alone do not prove a completed pipeline run.
