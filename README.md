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
* __Machine:__ Linux fv-az59 5.0.0-1032-azure #34-Ubuntu SMP Mon Feb 10 19:37:25 UTC 2020 x86_64 x86_64 x86_64 GNU/Linux | 2 vCPUs | 7GB.
* __Method:__ `autocannon -c 100 -d 40 -p 10 localhost:3000` (two rounds; one to warm-up, one to measure).
* __Node:__ `v12.16.1`
* __Run:__ Wed Apr  1 00:45:47 UTC 2020

|                          | Router | Requests/s | Latency | Throughput/Mb |
| :--                      | --:    | :-:        | --:     | --:           |
| bare                     | ✗      | 42800.8    | 2.23    | 6.69          |
| connect-router           | ✓      | 34594.0    | 2.79    | 5.41          |
| connect                  | ✗      | 35891.0    | 2.69    | 5.61          |
| egg.js                   | ✓      | 14613.8    | 6.77    | 4.82          |
| express-route-prefix     | ✓      | 20804.5    | 4.69    | 7.24          |
| express-with-middlewares | ✓      | 16465.2    | 5.97    | 5.95          |
| express                  | ✓      | 18967.2    | 5.16    | 2.97          |
| fastify-big-json         | ✓      | 8185.8     | 12.07   | 93.99         |
| fastify                  | ✓      | 43055.2    | 2.22    | 6.73          |
| foxify                   | ✓      | 37839.8    | 2.55    | 5.38          |
| hapi                     | ✓      | 19086.9    | 5.17    | 2.99          |
| koa-router               | ✓      | 25200.4    | 3.88    | 3.94          |
| koa                      | ✗      | 28236.8    | 3.45    | 4.42          |
| micro-route              | ✓      | 33031.4    | 2.93    | 5.17          |
| micro                    | ✗      | 37923.2    | 2.54    | 5.93          |
| microrouter              | ✓      | 19144.4    | 5.11    | 2.99          |
| polka                    | ✓      | 40908.0    | 2.35    | 6.40          |
| polkadot                 | ✗      | 43364.0    | 2.19    | 6.78          |
| rayo                     | ✓      | 36337.4    | 2.65    | 5.68          |
| restify                  | ✓      | 28068.8    | 3.47    | 4.44          |
| server-base-router       | ✓      | 34718.2    | 2.78    | 5.43          |
| server-base              | ✗      | 33128.2    | 2.92    | 5.18          |
| spirit-router            | ✓      | 34451.6    | 2.52    | 5.39          |
| spirit                   | ✗      | 29820.2    | 2.97    | 4.66          |
| take-five                | ✓      | 0.0        | 0.00    | 0.00          |
| total.js                 | ✓      | 27154.4    | 3.58    | 7.72          |
| trek-engine              | ✗      | 31043.0    | 3.13    | 4.41          |
| trek-router              | ✓      | 29873.2    | 3.26    | 4.25          |
| vapr                     | ✓      | 29525.6    | 3.29    | 4.20          |
| yeps-router              | ✓      | 29528.8    | 3.29    | 4.62          |
| yeps                     | ✗      | 37538.0    | 2.57    | 5.87          |
