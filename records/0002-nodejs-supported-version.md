# Node.js Supported Version

### Current state

As of the date of this PR (March 1st 2024), the only released and maintained version of Express.js is the v4. 
This version was created and published in 2014 and is supporting (working on) all Node.js version between 0.10 and 21.x - with tests run against all of them.

During the conception phase of Express v5 it was discussed to drop the support of all version below Node.js v4 (released in September 2015) - so supporting all versions from Node.js 4.x to Node.js 21.x, representing 18 versions.

### Ecosystem language support

Node.js creates new version every years, with a LTS being stable for ~3 years. 
For example, 20 was created in April 2023, moved to LTS in September 2023 and will be in maintenant mode until October 20224 and will run until April 2026.

Express and the ecosystem should follow versions that are not a security risk and keep being updated and patched as a primary support. 
It is possible to have some breaking changes between major versions but in the past couple years, it was mostly minimal.

> If other version keep to work with that, then this is a good bonus but we should not maintain a compatibility for all Node.js version.

For example

* Latest Springboot release only work with Java 17 and above: released in 2021
* Latest Symfony release only work with PHP8.1 and above: released in 2021
  * Laravel is almost the same as Symfony
* Latest Fastify LTS (released in 2022) supports up to Node.14 - which was the LTS 

### Node.js version supported

As a first point, the Express.js project should only support non-LTS version during their active phase and remove all specific compatibilities when they move out of active status - allowing us to use them as "trial" before the next LTS.

Most of the framework seems to only be compatible with version of the runtime (or language) released ~3 years ago, so something between v14 and v16 if we were to release today.

On the other hand, Node.js v16 is now unsupported for the past 6 months while the v14 is deprecated since one year and in maintenance mode for the past 28 months. 
We can argue that if users are not updating their Node.js version in this timeline they won't update to a new Express.js version.

### Packages and Node.js version

Some packages that we rely on, on their latest major version,are also dropping support of Node.js version that are above Node.js v4. 
Some of them would be part of our direct dependencies like `debug` (Node.js v6) and some other would be dev-dependencies like `mocha` (Node.js v14).

