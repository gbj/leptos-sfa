# leptos-sfa
Experimenting with a single-folder app

This packs the `app`, `client`, and `server` crates into a single crate/directory. See [this issue](https://github.com/gbj/leptos/issues/68).

You should be able to launch the client app with a simple `trunk serve --open`. 

To launch the server you can run `cargo run --no-default-features --features=ssr`.

To compile Wasm for hydrating that server-generated HTML you can `wasm-pack build --target=web --no-default-features --features=hydrate`
