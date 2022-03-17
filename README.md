# Yarn Berry - Multi-Project Mono-Repo

To reproduce, run:

- `yarn` at the root of the repository
- `cd nm`
- `yarn` inside the directory `nm`

Error stacktrace:

```
➤ YN0000: ┌ Resolution step
➤ YN0000: └ Completed
➤ YN0000: ┌ Fetch step
➤ YN0000: └ Completed
➤ YN0000: ┌ Link step
➤ YN0001: │ Error: Assertion failed: Expected the package to have been registered
    at h (/somewhere/in/my/system/repro/.yarn/releases/yarn-berry.cjs:2:167304)
    at h (/somewhere/in/my/system/repro/.yarn/releases/yarn-berry.cjs:2:167639)
    at h (/somewhere/in/my/system/repro/.yarn/releases/yarn-berry.cjs:2:167639)
    at b (/somewhere/in/my/system/repro/.yarn/releases/yarn-berry.cjs:2:167665)
    at Q (/somewhere/in/my/system/repro/.yarn/releases/yarn-berry.cjs:2:164335)
    at re.finalizeInstallWithPnp (/somewhere/in/my/system/repro/.yarn/releases/yarn-berry.cjs:2:185739)
    at async re.finalizeInstall (/somewhere/in/my/system/repro/.yarn/releases/yarn-berry.cjs:2:269270)
    at async ie.linkEverything (/somewhere/in/my/system/repro/.yarn/releases/yarn-berry.cjs:2:371776)
    at async /somewhere/in/my/system/repro/.yarn/releases/yarn-berry.cjs:2:379337
    at async f.startTimerPromise (/somewhere/in/my/system/repro/.yarn/releases/yarn-berry.cjs:2:389740)
➤ YN0000: └ Completed
➤ YN0000: Failed with errors in 0s 105ms

```