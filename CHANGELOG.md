# 0.1.0 (2026-04-03)


### Bug Fixes

* add emptyDir volume for postgres socket directory to resolve permission error ([4295399](https://github.com/ravibagri5/crossview/commit/4295399562b36b372b7bac7ee38396042506f31a))
* add engines field to package.json for Node.js version compatibility ([26a203d](https://github.com/ravibagri5/crossview/commit/26a203dda60bdd55487355636d2e4d1b77867b6d))
* add Helm registry login for OCI push authentication ([386219b](https://github.com/ravibagri5/crossview/commit/386219be38ad6c7f8059e14a1c0763cfcfc3001c))
* add SSL properties to Helm values schema ([889723f](https://github.com/ravibagri5/crossview/commit/889723ff846ca3f0f30bdd73e021681690e446ea))
* build only for amd64 to avoid QEMU ARM64 emulation issues ([4b4fb9e](https://github.com/ravibagri5/crossview/commit/4b4fb9e6999f5faa9b11f34518ee64a7d302aec9))
* check SARIF file exists before upload and upgrade to CodeQL v4 ([2170bc7](https://github.com/ravibagri5/crossview/commit/2170bc74585aaeaa8c9df7e3efa9da92d10d5d00))
* create PR for version bumps instead of pushing to protected main branch ([8805ec8](https://github.com/ravibagri5/crossview/commit/8805ec85af299ccbdfa81286246adb397caeee37))
* enable search functionality with server-side pagination and improve Providers page spacing ([f26fc88](https://github.com/ravibagri5/crossview/commit/f26fc88c0faeb6237f8ae4174f955a6de3431a7c))
* ensure rollup platform dependencies are installed in CI ([e8f9029](https://github.com/ravibagri5/crossview/commit/e8f9029b24dd6126481568917915063e23207e97))
* **helm:** validate release version against existing GitHub releases ([f417565](https://github.com/ravibagri5/crossview/commit/f417565b25c646faaf59264e3e9dc606c8345392))
* htlm ingress service reference ([f2e8202](https://github.com/ravibagri5/crossview/commit/f2e8202b83b8f80100d2444944749debbb5d0b81))
* improve logging, security contexts, OIDC callbacks, and in-cluster mode ([4191318](https://github.com/ravibagri5/crossview/commit/4191318f13aa0cfd68dd1d8ec5c1ec307c9ae379))
* **kubernetes:** defer RUnlock after conditional re-lock in GetContexts ([9174265](https://github.com/ravibagri5/crossview/commit/9174265ddc2f5a6ed0be3c91431902aa1a499d8f)), closes [#172](https://github.com/ravibagri5/crossview/issues/172)
* optimize composite resources loading and prevent unnecessary reloads ([da4b48f](https://github.com/ravibagri5/crossview/commit/da4b48fb7788b6f4e16ebe7884fc8ca737edfb2c))
* regenerate package-lock.json to resolve yaml version conflict ([29eface](https://github.com/ravibagri5/crossview/commit/29eface55b3d35e30611e108c2d341693ec1ff8d))
* regenerate package-lock.json to sync with package.json ([42d4537](https://github.com/ravibagri5/crossview/commit/42d4537299ec06986e4fe205e42fdc44dea735d8))
* remove context sidebar completely in in-cluster mode and fix service targetPort ([b316143](https://github.com/ravibagri5/crossview/commit/b316143127c1d6b656eabf2995170dafed11c13a))
* switch Dockerfile from Alpine to Debian for better multi-arch support ([95ee161](https://github.com/ravibagri5/crossview/commit/95ee1612a78ab190c8c1208e6da7d80d295fc7d6))
* update Helm chart to use dynamic DB_HOST and v-prefixed image tags ([cb2c588](https://github.com/ravibagri5/crossview/commit/cb2c58810949387de47b1ab3be9d49376f04dc19))
* update ORAS to 1.3.0 and add Helm config layer for 3.18+ compatibility ([9784a51](https://github.com/ravibagri5/crossview/commit/9784a51698ac725af456fe94fae7a41a60272ee3))
* use explicit docker.io registry URL and add retry for OCI push ([82d3dc7](https://github.com/ravibagri5/crossview/commit/82d3dc70420eff20cc5ab6e9282c3b0a04cb163a))
* use template value for postgres health check instead of env var expansion ([61f61fe](https://github.com/ravibagri5/crossview/commit/61f61fe77a328004f03f16d3e7a0b00c4d385f96))
* use unique branch name with run_id to avoid branch conflicts ([2ca2406](https://github.com/ravibagri5/crossview/commit/2ca24066984caf38864fbd066ba749b89e2e8bc5))


### Features

* add ManagedResourceDefinitions and ManagedResourceActivationPolicies support ([640f715](https://github.com/ravibagri5/crossview/commit/640f715549ebea4ea100aaf71dc641c40962d444))
* add OCI registry support for Helm charts ([9b9abcd](https://github.com/ravibagri5/crossview/commit/9b9abcd9f92a0705478c6461a7d5d518a3faddee))
* add PostgreSQL SSL/TLS connection support ([a2f040c](https://github.com/ravibagri5/crossview/commit/a2f040c3604919c938a28005e6a5df827b70a6cf))
* add syntax highlighting and independent widget loading ([1a0cdc7](https://github.com/ravibagri5/crossview/commit/1a0cdc7c8d8d8c145e7faedd3b7355ffcab665ad))
* change service type from LoadBalancer to ClusterIP ([533ec29](https://github.com/ravibagri5/crossview/commit/533ec292ef3a0f93d86d93ba714f53322d0bdb37))
* enhance MRD/MRAP error handling with Crossplane 2.0 upgrade messaging ([dcd5a05](https://github.com/ravibagri5/crossview/commit/dcd5a05ec073f672c07d7e8237c7786f0bd2aad3))
* Helm chart improvements and ARM64 support ([5847ace](https://github.com/ravibagri5/crossview/commit/5847ace61ca677b4eb503ff3f6b767303604231e))
* implement pagination throughout the application ([eac39b4](https://github.com/ravibagri5/crossview/commit/eac39b4f73c8474ca42f3134ea8fdb2f3b074cbe))
* implement real-time Kubernetes resource watching with event-driven updates ([e8d3150](https://github.com/ravibagri5/crossview/commit/e8d315019e415dbba4cbd1a4a5018a355c24de86))
* UI improvements, performance optimizations, and bug fixes ([78d9560](https://github.com/ravibagri5/crossview/commit/78d9560f5f29f22ce6f9de368c5c05d5772de7ff))
* unified API design and managed resources caching ([fe4c068](https://github.com/ravibagri5/crossview/commit/fe4c06852854de4b3707bdf6dcdd119c34f97bc4))


### Performance Improvements

* optimize data fetching for faster loading across all pages ([9879b5b](https://github.com/ravibagri5/crossview/commit/9879b5bd1543accf78e3a5667815a1cee90bf989))


### Reverts

* Revert "Add database connection retry logic with exponential backoff" ([6d9f2c7](https://github.com/ravibagri5/crossview/commit/6d9f2c71ee43433406cd48bf7d7465b705322d91))
* Revert "Fix Helm OCI push authentication by copying Docker credentials to Helm registry config" ([076e6b6](https://github.com/ravibagri5/crossview/commit/076e6b6d34084f6a350ae4d09640e99b21dbc341))
* remove PR creation and version commit step ([8deaf1e](https://github.com/ravibagri5/crossview/commit/8deaf1ef608ae5b7420fa20fa675e417647a9306))
# Changelog

# v3.8.0 (April 2026)

## Features & Enhancements

- **Handle missing Kubernetes API resources gracefully**  
  - Add `IsMissingKubernetesResourceError` helper to classify missing-resource cases, including the “the server could not find the requested resource” message.
  - Use that helper in Kubernetes resource listing so unsupported APIs return an empty result instead of bubbling up as an error.
  - Update the Kubernetes controller to treat those missing-resource errors as `200 OK` with empty `items`, avoiding the 500 path.
  - Add tests for the new helper and for the controller behavior when `Function` APIs are unavailable.

- **Add support for Managed Resource Definitions (MRD) and Managed Resource Activation Policies (MRAP)**  
  - Introduce dedicated pages for MRDs and MRAPs following the existing XRDs pattern.
  - MRDs page includes columns for NAME, STATE, ESTABLISHED, AGE with multi-filter support and status badges.
  - MRAPs page provides a clean view with NAME and AGE.
  - Both pages include ResourceDetails slideout and improved error handling with messaging for Crossplane 2.0 upgrades.

- **PostgreSQL SSL/TLS connection support**  
  - Add configurable SSL/TLS options for PostgreSQL connections via new environment variables: `DB_SSL_MODE`, `DB_SSL_ROOT_CERT`, `DB_SSL_CERT`, and `DB_SSL_KEY`.
  - Dynamically build the DSN with `sslmode`, `sslrootcert`, `sslcert`, and `sslkey` parameters (supports `disable`, `require`, `verify-ca`, `verify-full`, etc.).
  - Update configuration (`config.yaml`, `loader.js`), Helm chart values, ConfigMap, and deployment templates to support a nested `ssl` object.
  - Default to `sslmode=disable` for backward compatibility.
  - Remove password from connection failure logs for improved security.

- **Automate changelog, release notes, and PR title linting**  
  - Introduce automation using Conventional Commits and `changelog-cli` to generate `CHANGELOG.md` and `RELEASE_NOTES.md` during releases.
  - Add GitHub release integration (attach release notes and use them as description).
  - Enforce consistent PR titles via `lint-pr-title.yml` workflow.
  - Update `docs/CONTRIBUTING.md` with guidelines for PR titles, commits, and release notes.
  - Add local development support (scripts and `changelog-cli` dependency).

## Bug Fixes & Improvements

- **Fix server-side table search to filter full dataset**  
  - Apply search filtering to the complete dataset before pagination (instead of only the current page) in server-side mode.
  - Ensure search terms and searchable fields are properly passed to fetch callbacks.
  - Update filtering logic for Managed Resources, Claims, Composite Resources, Compositions, MRDs, and MRAPs.
  - Use continue tokens for Composite resource retrieval to support full-dataset filtering.
  - Total count now reflects the size of the filtered dataset.

- **Add SSL properties to Helm values schema**  
  - Fix missing SSL configuration properties in the Helm values JSON schema (follow-up to PostgreSQL SSL support).

- **Validate Helm release version against existing GitHub releases**  
  - Add version validation job in the Helm release workflow to prevent publishing arbitrary or mismatched versions.
  - Make test and release jobs dependent on successful validation.
  - Improve error messaging to show already-released versions when validation fails.

- **Updated readme**  
  - Fix `Helm Repository` address in the README (was pointing to the old organization).

- **Provided default values for admin username and password in `helm/crossview/values.yaml`**  
```yaml
secrets:
  adminUsername: "admin"
  adminPassword: "password"
```

- **Improve documentation for production SSO deployments**  
  - Document `server.cors.origin` (`CORS_ORIGIN`) as a required field for any non-local deployment using SSO. When unset, the post-login redirect goes to `http://localhost:5173` instead of the actual host.
  - Add a dedicated "Required: Set `server.cors.origin` for Production" section to `docs/SSO_SETUP.md` with config file, env var, and Helm examples.
  - Update `callbackURL` examples throughout `docs/SSO_SETUP.md` to use a real host (`https://crossview.example.com/api/auth/oidc/callback`) instead of localhost.
  - Add `CORS_ORIGIN` to `docs/CONFIGURATION.md` server settings and SSO troubleshooting section.
  - Add inline warning comment on `config.server.cors.origin` in `helm/crossview/values.yaml`.

- **Document default admin credentials for session auth mode**  
  - Add a "Default Admin Credentials" subsection to `docs/CONFIGURATION.md` noting that the default username/password is `admin`/`password` and documenting how to override them via Helm values or environment variables.
  - Add default credentials as the top item in the Security Best Practices section.

## Contributors

A big thank you to all the contributors who helped make this release possible!

- **conclusionlogic** – for gracefully handling missing Kubernetes API resources
- **ravibagri5** – for adding support for Managed Resource Definitions (MRD) and Managed Resource Activation Policies (MRAP)
- **MoeidHeidari** – for PostgreSQL SSL/TLS connection support and Helm schema fixes
- **Berk-Unsal** – for fixing server-side table search to work on the full dataset
- **erfanmo** – for automating changelog generation, release notes, PR title linting, and Helm version validation

Thank you for your valuable contributions! 🙏