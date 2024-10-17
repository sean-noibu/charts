# Charts

A repository for my custom Helm charts. You're welcome to use them too, and PRs/Issues are welcome.

* Briefer ([README](charts/briefer/README.md))- A chart for deploying [Briefer](https://briefer.cloud/).

## Usage

[Helm](https://helm.sh) must be installed to use the charts. Please refer to Helm's [documentation](https://helm.sh/docs) 
to get started.

Once Helm has been set up correctly, add the repo as follows:

```bash
helm repo add pseudomuto https://pseudomuto.github.io/charts
```

If you had already added this repo earlier, run `helm repo update` to retrieve
the latest versions of the packages.  You can then run `helm search repo
pseudomuto` to see the charts.

To install the <chart-name> chart:

```bash
helm install my-<chart-name> pseudomuto/<chart-name>
```

To uninstall the chart:

```bash
    helm delete my-<chart-name>
```

> Note: See the README for the particular chart for more installation details.

## Contributing

You'll need the [task] binary installed. I don't like installing global binaries (which is why you'll notice the helm,
k3d, helm-docs, etc. are all installed in `./bin` here). If you'd like to do the same for [task], you can run the
following which will put it in `./bin/task`.

```bash
sh -c "$(curl --location https://taskfile.dev/install.sh)" -- -d v3.39.2
```

After that, you can run `bin/task -a` to see a list of available tasks.

[task]: https://taskfile.dev/
