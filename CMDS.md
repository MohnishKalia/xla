bazel build --test_output=all --spawn_strategy=sandboxed //xla/tools:run_hlo_module
bazel build --test_output=all --spawn_strategy=sandboxed //xla/hlo/transforms/simplifiers:algebraic_simplifier
bazel test //xla/hlo/transforms/simplifiers:algebraic_simplifier_test