# mlx-swift-lm — afm pre-patched fork

This is a **pre-patched fork** of [ml-explore/mlx-swift-lm](https://github.com/ml-explore/mlx-swift-lm),
maintained as the SwiftPM dependency for **afm** ([scouzi1966/maclocal-api](https://github.com/scouzi1966/maclocal-api)).

The tree is the upstream submodule with `maclocal-api/Scripts/patches/` already applied
(new model architectures, batch KV cache, sampler/tool-call/tokenizer changes) and
`Package.swift` pinned to `mlx-swift` exact `0.30.3`. It exists so afm can be consumed by
`.package(url:)` **without git submodules** (a plain `git clone` + `swift build` works).

**Do not edit this fork directly.** It is regenerated from upstream + the patch set by
`maclocal-api/Scripts/build-mlx-swift-lm-fork.sh`. Upstream license (MIT) is retained.
