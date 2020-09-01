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
* __Machine:__ Linux fv-az59 5.3.0-1034-azure #35~18.04.1-Ubuntu SMP Mon Jul 13 12:54:45 UTC 2020 x86_64 x86_64 x86_64 GNU/Linux | 2 vCPUs | 7GB.
* __Method:__ `autocannon -c 100 -d 40 -p 10 localhost:3000` (two rounds; one to warm-up, one to measure).
* __Node:__ `v12.18.3`
* __Run:__ Tue Sep  1 00:55:51 UTC 2020

|                          | Router | Requests/s | Latency | Throughput/Mb |
| :--                      | --:    | :-:        | --:     | --:           |
| bare                     | ✗      | 47676.0    | 2.01    | 7.46          |
| connect-router           | ✓      | 42160.0    | 2.28    | 6.59          |
| connect                  | ✗      | 47173.6    | 2.03    | 7.38          |
| egg.js                   | ✓      | 17877.7    | 5.52    | 5.90          |
| express-route-prefix     | ✓      | 9249.8     | 10.72   | 3.22          |
| express-with-middlewares | ✓      | 9040.5     | 10.91   | 3.27          |
| express                  | ✓      | 10195.9    | 9.68    | 1.59          |
| fastify-big-json         | ✓      | 8853.1     | 11.15   | 101.66        |
| fastify                  | ✓      | 48090.4    | 1.99    | 7.52          |
| foxify                   | ✓      | 48035.2    | 2.00    | 6.83          |
| hapi                     | ✓      | 21345.6    | 4.60    | 3.34          |
| koa-router               | ✓      | 32570.6    | 2.99    | 5.09          |
| koa                      | ✗      | 35945.4    | 2.70    | 5.62          |
| micro-route              | ✓      | 41900.0    | 2.30    | 6.55          |
| micro                    | ✗      | 46905.6    | 2.05    | 7.34          |
| microrouter              | ✓      | 25331.2    | 3.85    | 3.96          |
| polka                    | ✓      | 47488.8    | 2.02    | 7.43          |
| polkadot                 | ✗      | 55628.0    | 1.68    | 8.70          |
| rayo                     | ✓      | 46473.6    | 2.07    | 7.27          |
| restify                  | ✓      | 32256.8    | 3.01    | 5.11          |
| server-base-router       | ✓      | 42693.6    | 2.26    | 6.68          |
| server-base              | ✗      | 44572.8    | 2.16    | 6.97          |
| spirit-router            | ✓      | 35887.2    | 2.20    | 5.61          |
| spirit                   | ✗      | 36592.2    | 2.13    | 5.72          |
| take-five                | ✓      | 0.0        | 0.00    | 0.00          |
| total.js                 | ✓      | 35251.4    | 2.75    | 10.02         |
| trek-engine              | ✗      | 40349.0    | 2.40    | 5.73          |
| trek-router              | ✓      | 41715.2    | 2.32    | 5.93          |
| vapr                     | ✓      | 37991.2    | 2.54    | 5.40          |
| yeps-router              | ✓      | 37724.0    | 2.57    | 5.90          |
| yeps                     | ✗      | 45434.4    | 2.11    | 7.11          |
