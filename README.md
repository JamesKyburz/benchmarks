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
* __Machine:__ Linux fv-az95 5.3.0-1028-azure #29~18.04.1-Ubuntu SMP Fri Jun 5 14:32:34 UTC 2020 x86_64 x86_64 x86_64 GNU/Linux | 2 vCPUs | 7GB.
* __Method:__ `autocannon -c 100 -d 40 -p 10 localhost:3000` (two rounds; one to warm-up, one to measure).
* __Node:__ `v12.18.1`
* __Run:__ Wed Jul  1 00:51:32 UTC 2020

|                          | Router | Requests/s | Latency | Throughput/Mb |
| :--                      | --:    | :-:        | --:     | --:           |
| bare                     | ✗      | 36789.4    | 2.62    | 5.75          |
| connect-router           | ✓      | 29826.4    | 3.25    | 4.67          |
| connect                  | ✗      | 32705.8    | 2.96    | 5.12          |
| egg.js                   | ✓      | 13393.6    | 7.39    | 4.42          |
| express-route-prefix     | ✓      | 7690.7     | 12.90   | 2.68          |
| express-with-middlewares | ✓      | 6747.6     | 14.68   | 2.44          |
| express                  | ✓      | 7954.9     | 12.41   | 1.24          |
| fastify-big-json         | ✓      | 7802.8     | 12.67   | 89.59         |
| fastify                  | ✓      | 35579.0    | 2.71    | 5.56          |
| foxify                   | ✓      | 33260.8    | 2.91    | 4.73          |
| hapi                     | ✓      | 17628.1    | 5.60    | 2.76          |
| koa-router               | ✓      | 21630.4    | 4.53    | 3.38          |
| koa                      | ✗      | 26518.4    | 3.68    | 4.15          |
| micro-route              | ✓      | 27051.6    | 3.59    | 4.23          |
| micro                    | ✗      | 32748.0    | 2.96    | 5.12          |
| microrouter              | ✓      | 19324.0    | 5.08    | 3.02          |
| polka                    | ✓      | 31840.6    | 3.04    | 4.98          |
| polkadot                 | ✗      | 41205.6    | 2.31    | 6.44          |
| rayo                     | ✓      | 31929.2    | 3.03    | 4.99          |
| restify                  | ✓      | 23564.4    | 4.15    | 3.73          |
| server-base-router       | ✓      | 29867.2    | 3.25    | 4.67          |
| server-base              | ✗      | 29466.4    | 3.29    | 4.61          |
| spirit-router            | ✓      | 29127.2    | 3.05    | 4.56          |
| spirit                   | ✗      | 27749.6    | 3.23    | 4.34          |
| take-five                | ✓      | 0.0        | 0.00    | 0.00          |
| total.js                 | ✓      | 22544.8    | 4.32    | 6.41          |
| trek-engine              | ✗      | 28504.8    | 3.42    | 4.05          |
| trek-router              | ✓      | 26267.2    | 3.71    | 3.73          |
| vapr                     | ✓      | 23510.0    | 4.15    | 3.34          |
| yeps-router              | ✓      | 27350.0    | 3.55    | 4.28          |
| yeps                     | ✗      | 30260.4    | 3.20    | 4.73          |
