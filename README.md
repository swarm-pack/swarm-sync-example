# Swarm-sync Example Config Repo

An example configuration repository for [swarm-sync](https://github.com/kevb/swarm-sync).

See also: [swarm-pack](https://github.com/vudknguyen/swarm-pack).

# Bump

Bumpable number to trigger change: 2

## Notes

### Stacks

A stack is a namespace containing a set of releases. The use-cases for stack include separating different environments (prod, staging, etc) or different swarms (e.g. we have a 'tools' swarm on separate infra).

Multiple stacks can live in the same repo, and an instance of swarm-sync can target one or more stacks in a repo.

Stacks are defined in directories `stacks/[stack-name]`.

### Releases

A release describes a single swarm-pack deployed within a stack. Releases are defined in individual `stacks/[stack-name]/[release-name].yml` files.

At it's most basic, a release consists of `release_name` and `pack`.