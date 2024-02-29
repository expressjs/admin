# Supported versions

## Long Term Support

Express Long Term Support (LTS) version is provided as per defined in this document - and also include all the packages part of the Express.js Organization (express, pillarjs and jshttp).

1. Express follows a semantic versioning A.B.C (also know as semver), where the major version is represented by "A". Major version are supported for a minimal time of a year (as seen as 365 days). 

2. After the time that a LTS version (that can exceed one year) is maintained, the version will move to a maintenance mode during which only security patches will be released. This maintenance mode will be supported for at least one year. 

> In specific case, a version in maintenance mode may require a breaking change to fix a security risk. If this happen, then it will be released as a minor version change but outlined in the release message

3. Major version will be tested against all the LTS versions that were active during the time of the major version. This doesn't mean that the package won't support previous versions, but no tests will be run against them.

> As per the date of this PR (March, 1st 2024), Node.js LTS versions are 18 (maintenance) and 20 (active) meaning that if a new major version was released today we would support Node.js 18, Node.js 20 and at minimal Node.js 22 when it will become a stable LTS (without dropping Node.js 18 when it would be move out of maintenance mode).

## Express Releases

| Express version  	| Release  	| Maintenance  	| End of Life  	| Supported Node.js version  	|
|---	|---	|---	|---	|g---	|
|  v1 	| Nov 17, 2010  	|  ? 	| ?  	| ?  	|
|  v2 	| Mar 18, 2011  	|  ? 	| ?  	| ?  	|
|  v3 	| on Nov 2, 2012  	|  ? 	| ?  	| ?  	|
|  v4 	| Apr 9, 2014  	| ?  	|  ? 	| 0.10 to 20.x  	|
|  v5 	|  ? 	| ?  	|   ?	|  ? 	|
