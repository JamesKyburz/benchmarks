<div align="center">
<img src="https://github.com/fastify/graphics/raw/master/full-logo.png" width="650" height="auto"/>
</div>

<div align="center">

[![Build Status](https://travis-ci.org/fastify/fastify.svg?branch=master)](https://travis-ci.org/fastify/fastify)
[![Coverage Status](https://coveralls.io/repos/github/fastify/fastify/badge.svg?branch=master)](https://coveralls.io/github/fastify/fastify?branch=master)
[![js-standard-style](https://img.shields.io/badge/code%20style-standard-brightgreen.svg?style=flat)](http://standardjs.com/)
[![NPM version](https://img.shields.io/npm/v/fastify.svg?style=flat)](https://www.npmjs.com/package/fastify)
[![NPM downloads](https://img.shields.io/npm/dm/fastify.svg?style=flat)](https://www.npmjs.com/package/fastify) [![Gitter](https://badges.gitter.im/gitterHQ/gitter.svg)](https://gitter.im/fastify)
</div>
<br />

# TL;DR

* [Fastify](https://github.com/fastify/fastify) is, fast and low overhead web framework for Node.js
* This package shows how fast it is comparatively.

# Installing

```
npm i -g fastify-benchmarks
```

# Usage

```
benchmark [arguments (optional)]
```

#### Arguments

* `-h`: Help on how to use the tool.
* `compare`: Get comparative data for your benchmarks.

> You may also compare all test results, at once, in a single table; `benchmark compare -t`

> You can also extend the comparison table with percentage values based on fastest result; `benchmark compare -p`
# Benchmarks
* __Machine:__ Linux fv-az98 5.3.0-1032-azure #33~18.04.1-Ubuntu SMP Fri Jun 26 15:01:15 UTC 2020 x86_64 x86_64 x86_64 GNU/Linux | 2 vCPUs | 7GB.
* __Method:__ `autocannon -c 100 -d 40 -p 10 localhost:3000` (two rounds; one to warm-up, one to measure).
* __Node:__ `v12.18.3`
* __Run:__ Sat Aug  1 00:53:27 UTC 2020

|                          | Router | Requests/s | Latency | Throughput/Mb |
| :--                      | --:    | :-:        | --:     | --:           |
| bare                     | ✗      | 36211.0    | 2.67    | 5.66          |
| connect-router           | ✓      | 30656.6    | 3.16    | 4.79          |
| connect                  | ✗      | 33967.2    | 2.85    | 5.31          |
| egg.js                   | ✓      | 13567.6    | 7.29    | 4.48          |
| express-route-prefix     | ✓      | 7355.2     | 13.50   | 2.56          |
| express-with-middlewares | ✓      | 6941.2     | 14.25   | 2.51          |
| express                  | ✓      | 7771.4     | 12.71   | 1.22          |
| fastify-big-json         | ✓      | 7880.9     | 12.54   | 90.49         |
| fastify                  | ✓      | 33584.6    | 2.88    | 5.25          |
| foxify                   | ✓      | 35943.8    | 2.69    | 5.11          |
| hapi                     | ✓      | 18043.7    | 5.47    | 2.82          |
| koa-router               | ✓      | 23397.2    | 4.18    | 3.66          |
| koa                      | ✗      | 26538.4    | 3.67    | 4.15          |
| micro-route              | ✓      | 30991.8    | 3.13    | 4.85          |
| micro                    | ✗      | 36434.6    | 2.65    | 5.70          |
| microrouter              | ✓      | 19470.4    | 5.04    | 3.05          |
| polka                    | ✓      | 34129.8    | 2.83    | 5.34          |
| polkadot                 | ✗      | 43744.8    | 2.14    | 6.84          |
| rayo                     | ✓      | 33512.0    | 2.89    | 5.24          |
| restify                  | ✓      | 25844.0    | 3.77    | 4.09          |
| server-base-router       | ✓      | 30141.2    | 3.22    | 4.71          |
| server-base              | ✗      | 32175.8    | 3.01    | 5.03          |
| spirit-router            | ✓      | 29999.6    | 2.94    | 4.69          |
| spirit                   | ✗      | 31213.4    | 2.82    | 4.88          |
| take-five                | ✓      | 0.0        | 0.00    | 0.00          |
| total.js                 | ✓      | 22315.2    | 4.37    | 6.34          |
| trek-engine              | ✗      | 28213.2    | 3.45    | 4.01          |
| trek-router              | ✓      | 27641.6    | 3.53    | 3.93          |
| vapr                     | ✓      | 24775.6    | 3.93    | 3.52          |
| yeps-router              | ✓      | 27801.6    | 3.50    | 4.35          |
| yeps                     | ✗      | 33319.6    | 2.90    | 5.21          |
