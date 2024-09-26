# Transaction Subgraph
This is a subgraph implementing parsing of transaction entities on multiversx chain according to [eStandard Digital Tokens specification](https://github.com/multiversx/mx-specs/blob/main/ESDT-specs.md)

# Running
1. Clone the [firehose-multiversx](https://github.com/multiversx/firehose-multiversx) repository
2. Edit [substreams.yaml](./substreams.yaml) and change [line 18](./substreams.yaml#L18) to point at the `proto` folder from the cloned firehose-multiversx repository
3. Edit [package.json](./package.json) to set `--node` and `--ipfs` to point at the graphnode
4. Build the spkg
    ```shell
    pnpm run build
    ```
5. Create the subgraph
    ```shell
    pnpm run create
    ```
6. Deploy the subgraph
    ```shell
    pnpm run deploy
    ```
