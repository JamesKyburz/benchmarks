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
* __Machine:__ Linux fv-az86 5.0.0-1035-azure #37-Ubuntu SMP Wed Mar 18 11:21:35 UTC 2020 x86_64 x86_64 x86_64 GNU/Linux | 2 vCPUs | 7GB.
* __Method:__ `autocannon -c 100 -d 40 -p 10 localhost:3000` (two rounds; one to warm-up, one to measure).
* __Node:__ `v12.16.3`
* __Run:__ Fri May  1 00:45:46 UTC 2020

|                          | Router | Requests/s | Latency | Throughput/Mb |
| :--                      | --:    | :-:        | --:     | --:           |
| bare                     | ✗      | 56618.4    | 1.68    | 8.85          |
| connect-router           | ✓      | 48383.2    | 1.98    | 7.57          |
| connect                  | ✗      | 54113.6    | 1.76    | 8.46          |
| egg.js                   | ✓      | 19397.1    | 5.08    | 6.40          |
| express-route-prefix     | ✓      | 28548.0    | 3.40    | 9.94          |
| express-with-middlewares | ✓      | 21525.6    | 4.53    | 7.78          |
| express                  | ✓      | 26738.0    | 3.64    | 4.18          |
| fastify-big-json         | ✓      | 10519.0    | 9.38    | 120.78        |
| fastify                  | ✓      | 59277.6    | 1.59    | 9.27          |
| foxify                   | ✓      | 55385.6    | 1.71    | 7.87          |
| hapi                     | ✓      | 22692.0    | 4.32    | 3.55          |
| koa-router               | ✓      | 36234.2    | 2.67    | 5.67          |
| koa                      | ✗      | 41154.4    | 2.34    | 6.44          |
| micro-route              | ✓      | 47492.0    | 2.01    | 7.43          |
| micro                    | ✗      | 51519.2    | 1.85    | 8.06          |
| microrouter              | ✓      | 28560.4    | 3.40    | 4.47          |
| polka                    | ✓      | 54657.6    | 1.74    | 8.55          |
| polkadot                 | ✗      | 58621.6    | 1.58    | 9.17          |
| rayo                     | ✓      | 54922.4    | 1.73    | 8.59          |
| restify                  | ✓      | 35381.8    | 2.74    | 5.60          |
| server-base-router       | ✓      | 48193.6    | 1.98    | 7.54          |
| server-base              | ✗      | 49429.6    | 1.93    | 7.73          |
| spirit-router            | ✓      | 37561.6    | 2.11    | 5.87          |
| spirit                   | ✗      | 36094.2    | 2.19    | 5.65          |
| take-five                | ✓      | 0.0        | 0.00    | 0.00          |
| total.js                 | ✓      | 38105.8    | 2.53    | 10.83         |
| trek-engine              | ✗      | 45748.0    | 2.10    | 6.50          |
| trek-router              | ✓      | 45024.0    | 2.14    | 6.40          |
| vapr                     | ✓      | 40140.0    | 2.40    | 5.70          |
| yeps-router              | ✓      | 40432.8    | 2.38    | 6.32          |
| yeps                     | ✗      | 47448.0    | 2.02    | 7.42          |
