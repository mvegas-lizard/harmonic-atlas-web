# LAME MP3 encoder

This directory contains the unmodified ES module from `@breezystack/lamejs` 1.2.7, a JavaScript port of LAME by Alex Zhukov, with the ESM packaging fork published by shijinyu. It is licensed under LGPL-3.0, separately from Harmonic Atlas's MIT code.

- LAME project: https://lame.sourceforge.io/
- Upstream repository: https://github.com/gideonstele/lamejs
- Exact upstream source commit: `1fb0ef5fa177413107e2e107d054a9b994e3f79c`
- Corresponding source archive: [source.tar.gz](source.tar.gz)
- Upstream package notice: [LICENSE](LICENSE)
- License texts: [LGPL-3.0](LGPL-3.0.txt), [GPL-3.0](GPL-3.0.txt)
- Unmodified module SHA-256: `1c5f944911ccf2f6e29ab36c2e568363210ab16f50c0d76077060f40ecf91d28`
- Source archive SHA-256: `af8f08f0ff9a13777f2ffff737b48e40019b53a4b21db270dd62e829574e2b83`

The application loads this module separately, on demand, inside its MP3 worker. It is not merged into the application bundle. A recipient can replace this file with a compatible modified version without rebuilding the app. Harmonic Atlas makes no changes to the encoder. The source archive includes the encoder's source and upstream build instructions; the npm package's build configuration is preserved there.
