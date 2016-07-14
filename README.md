# Mix.Compiler.Core

Compiles Core Erlang files

## Installation

If [available in Hex](https://hex.pm/docs/publish), the package can be installed as:

  1. Add `mix_core_compiler` to your list of dependencies in `mix.exs`:

    ```elixir
    def deps do
      [{:mix_core_compiler, "~> 0.1.0"}]
    end
    ```

  2. Ensure `mix_core_compiler` is started before your application:

    ```elixir
    def application do
      [applications: [:mix_core_compiler]]
    end
    ```

  2. Ensure `:core` is added to your project's compilers:

    ```elixir
    def project do
      #...
      compilers: [:core | Mix.compilers],
      #...
    end
    ```

## Usage

Identical to the `Mix.Tasks.Compile.Erlang` and `Mix.Compiler.Erlang` modules. By default looks in `src` for `.core` files.
