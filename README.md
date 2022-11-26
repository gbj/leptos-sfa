# PLEASE NOTE

**Do not use this.** This was a scratch-pad for how to simplify our build systems. The examples in the [Leptos repo](https://github.com/gbj/leptos) now use a tweaked version of this format. You should check out [cargo-leptos](https://github.com/akesson/cargo-leptos) as a build tool.


# leptos-sfa
Experimenting with a single-folder app

This packs the `app`, `client`, and `server` crates into a single crate/directory. See [this issue](https://github.com/gbj/leptos/issues/68).

You should be able to launch the client app with a simple `trunk serve --open`. 

To launch the server you can run `cargo run --no-default-features --features=ssr`.

To compile Wasm for hydrating that server-generated HTML you can `wasm-pack build --target=web --no-default-features --features=hydrate`
