## 2.0.5

**In-node QwenVL prompt enhance** — the director can rewrite each segment's
prompt with a local GGUF chat model (llama-cpp) before relay, no external
service needed. The enhancer model and preset are catalog dropdowns: GGUF
files are listed from disk and missing ones auto-download from Hugging Face.

**Enhancer output hardened** — thinking blocks (`</think>`) are stripped from
GGUF replies, `/no_think` is sent up front, the model's part count is regrouped
back to the segment count when it over-splits, and prompts are read from the
main-track segments so stale caches cannot leak in.

**Widget order preserved** — enhance inputs moved to the end of the node so
workflows saved before the feature keep their widget values.

## 2.0.4

Reference Sheet/Ingredients IC-LoRA support, optimizations, bug fixes and
improvements.
