### Aman

Staff Engineer. ~12 years on distributed backend systems — event-driven
architecture, Kafka/CDC pipelines, microservices, and the cloud-native
infrastructure they sit on. Day to day I work in a large TypeScript monorepo
and spend most of my time on system design, clean architecture, and developer
tooling.

#### Selected work

**[vitest-dev/vitest#11159](https://github.com/vitest-dev/vitest/pull/11159)** —
Diagnosed a module-resolution bug where a bare `import { PassThrough } from
"stream"` silently resolved to a nonexistent path inside hoisted monorepos,
while `node:stream` worked and the same file passed in a sibling package.
The root cause was a blind `slice` assuming Vitest's `dist` lived under the
project root; *which* builtins broke depended on the character length of your
checkout path, so the same repo failed differently per machine. An equivalent
fix shipped upstream in
[#11196](https://github.com/vitest-dev/vitest/pull/11196).

#### Interests

System design and architecture, developer tooling and test infrastructure,
event-driven systems at scale.
