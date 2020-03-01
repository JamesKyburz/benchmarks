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
* __Machine:__ Linux fv-az89 5.0.0-1032-azure #34-Ubuntu SMP Mon Feb 10 19:37:25 UTC 2020 x86_64 x86_64 x86_64 GNU/Linux | 2 vCPUs | 7GB.
* __Method:__ `autocannon -c 100 -d 40 -p 10 localhost:3000` (two rounds; one to warm-up, one to measure).
* __Node:__ `v12.16.1`
* __Run:__ Sun Mar  1 00:46:32 UTC 2020

|                          | Router | Requests/s | Latency | Throughput/Mb |
| :--                      | --:    | :-:        | --:     | --:           |
| bare                     | ✗      | 60504.0    | 1.56    | 9.46          |
| connect-router           | ✓      | 51077.6    | 1.87    | 7.99          |
| connect                  | ✗      | 55340.8    | 1.72    | 8.66          |
| egg.js                   | ✓      | 18850.0    | 5.23    | 6.22          |
| express-route-prefix     | ✓      | 31507.8    | 3.07    | 10.97         |
| express-with-middlewares | ✓      | 23220.0    | 4.20    | 8.39          |
| express                  | ✓      | 29454.4    | 3.30    | 4.61          |
| fastify-big-json         | ✓      | 11119.0    | 8.87    | 127.67        |
| fastify                  | ✓      | 62958.0    | 1.49    | 9.85          |
| foxify                   | ✓      | 60130.8    | 1.57    | 8.54          |
| hapi                     | ✓      | 24054.4    | 4.07    | 3.76          |
| koa-router               | ✓      | 37594.4    | 2.58    | 5.88          |
| koa                      | ✗      | 42668.8    | 2.26    | 6.67          |
| micro-route              | ✓      | 53324.0    | 1.78    | 8.34          |
| micro                    | ✗      | 59086.4    | 1.60    | 9.24          |
| microrouter              | ✓      | 29340.4    | 3.31    | 4.59          |
| polka                    | ✓      | 62942.8    | 1.50    | 9.84          |
| polkadot                 | ✗      | 63178.0    | 1.45    | 9.88          |
| rayo                     | ✓      | 57778.4    | 1.64    | 9.04          |
| restify                  | ✓      | 38119.4    | 2.54    | 6.03          |
| server-base-router       | ✓      | 58188.0    | 1.63    | 9.10          |
| server-base              | ✗      | 55324.8    | 1.72    | 8.65          |
| spirit-router            | ✓      | 41905.6    | 1.94    | 6.55          |
| spirit                   | ✗      | 46152.8    | 1.76    | 7.22          |
| take-five                | ✓      | 0.0        | 0.00    | 0.00          |
| total.js                 | ✓      | 43516.0    | 2.20    | 11.37         |
| trek-engine              | ✗      | 51776.0    | 1.85    | 7.36          |
| trek-router              | ✓      | 50843.2    | 1.88    | 7.22          |
| vapr                     | ✓      | 44734.4    | 2.14    | 6.36          |
| yeps-router              | ✓      | 45446.4    | 2.11    | 7.11          |
| yeps                     | ✗      | 55309.6    | 1.72    | 8.65          |
