# CHANGELOG - http_check

## 8.0.1 / 2022-05-23

* [Fixed] Clarify no cert service check message. See [#12064](https://github.com/DataDog/integrations-core/pull/12064).

## 8.0.0 / 2022-05-15

* [Fixed] Don't pin urllib3. See [#11944](https://github.com/DataDog/integrations-core/pull/11944).
* [Removed] Delete unused `weakciphers` option path. See [#11926](https://github.com/DataDog/integrations-core/pull/11926).

## 7.1.1 / 2022-04-11 / Agent 7.36.0

* [Fixed] Improve service check message when cert is not found. See [#11793](https://github.com/DataDog/integrations-core/pull/11793).

## 7.1.0 / 2022-04-05

* [Added] Upgrade dependencies. See [#11726](https://github.com/DataDog/integrations-core/pull/11726).
* [Added] Add metric_patterns options to filter all metric submission by a list of regexes. See [#11695](https://github.com/DataDog/integrations-core/pull/11695).
* [Fixed] Document TLS options. See [#11714](https://github.com/DataDog/integrations-core/pull/11714).
* [Fixed] Remap `check_hostname` to `tls_validate_hostname` . See [#11706](https://github.com/DataDog/integrations-core/pull/11706).
* [Fixed] Fail more gracefully. See [#11615](https://github.com/DataDog/integrations-core/pull/11615).

## 7.0.1 / 2022-03-02

* [Fixed] Avoid reading response content unless necessary. See [#11590](https://github.com/DataDog/integrations-core/pull/11590).
* [Fixed] Remove outdated warning in the description for the `tls_ignore_warning` option. See [#11591](https://github.com/DataDog/integrations-core/pull/11591).

## 7.0.0 / 2022-03-02 / Agent 7.35.0

* [Added] Add `pyproject.toml` file. See [#11365](https://github.com/DataDog/integrations-core/pull/11365).
* [Fixed] Fix namespace packaging on Python 2. See [#11532](https://github.com/DataDog/integrations-core/pull/11532).
* [Changed] Add tls_protocols_allowed option documentation. See [#11251](https://github.com/DataDog/integrations-core/pull/11251).

## 6.1.2 / 2022-01-08 / Agent 7.33.0

* [Fixed] Add urllib3 as dependency. See [#11069](https://github.com/DataDog/integrations-core/pull/11069).
* [Fixed] Fix urllib3 import statement. See [#11065](https://github.com/DataDog/integrations-core/pull/11065).
* [Fixed] Add comment to autogenerated model files. See [#10945](https://github.com/DataDog/integrations-core/pull/10945).

## 6.1.1 / 2021-10-18

* [Fixed] Avoid resetting auth token on headers. See [#10388](https://github.com/DataDog/integrations-core/pull/10388).

## 6.1.0 / 2021-10-04 / Agent 7.32.0

* [Added] Update dependencies. See [#10228](https://github.com/DataDog/integrations-core/pull/10228).
* [Added] Add HTTP option to control the size of streaming responses. See [#10183](https://github.com/DataDog/integrations-core/pull/10183).
* [Added] Add allow_redirect option. See [#10160](https://github.com/DataDog/integrations-core/pull/10160).
* [Added] Disable generic tags. See [#10027](https://github.com/DataDog/integrations-core/pull/10027).
* [Fixed] Bump base package dependency. See [#10218](https://github.com/DataDog/integrations-core/pull/10218).
* [Fixed] Fix the description of the `allow_redirects` HTTP option. See [#10195](https://github.com/DataDog/integrations-core/pull/10195).

## 6.0.0 / 2021-08-22 / Agent 7.31.0

* [Changed] Remove messages for integrations for OK service checks. See [#9888](https://github.com/DataDog/integrations-core/pull/9888).

## 5.3.2 / 2021-06-07 / Agent 7.29.0

* [Fixed] Fix data configuration type. See [#9482](https://github.com/DataDog/integrations-core/pull/9482).

## 5.3.1 / 2021-04-20 / Agent 7.28.0

* [Fixed] Restore correct default value of tls_verify. See [#9197](https://github.com/DataDog/integrations-core/pull/9197).

## 5.3.0 / 2021-04-19

* [Added] Upgrade cryptography to 3.4.6 on Python 3. See [#8764](https://github.com/DataDog/integrations-core/pull/8764).
* [Added] Add runtime configuration validation. See [#8932](https://github.com/DataDog/integrations-core/pull/8932).

## 5.2.0 / 2021-03-07 / Agent 7.27.0

* [Fixed] Bump minimum base package version. See [#8443](https://github.com/DataDog/integrations-core/pull/8443).
* [Security] Upgrade cryptography python package. See [#8611](https://github.com/DataDog/integrations-core/pull/8611).

## 5.1.0 / 2021-01-28 / Agent 7.26.0

* [Security] Upgrade cryptography python package. See [#8476](https://github.com/DataDog/integrations-core/pull/8476).

## 5.0.0 / 2021-01-21

* [Added] Support combined client cert files. See [#8298](https://github.com/DataDog/integrations-core/pull/8298).
* [Fixed] Fix misleading debug message. See [#8379](https://github.com/DataDog/integrations-core/pull/8379).
* [Changed] Update http_check to use TLS context wrapper. See [#8268](https://github.com/DataDog/integrations-core/pull/8268).
* [Changed] Only send ssl metrics if a connection succeeded. See [#8102](https://github.com/DataDog/integrations-core/pull/8102).

## 4.12.0 / 2020-10-31 / Agent 7.24.0

* [Added] Add support for OPTIONS method. See [#7894](https://github.com/DataDog/integrations-core/pull/7894).
* [Added] Add ability to dynamically get authentication information. See [#7660](https://github.com/DataDog/integrations-core/pull/7660).
* [Security] Upgrade `cryptography` dependency. See [#7869](https://github.com/DataDog/integrations-core/pull/7869).

## 4.11.0 / 2020-09-21 / Agent 7.23.0

* [Added] Add RequestsWrapper option to support UTF-8 for basic auth. See [#7441](https://github.com/DataDog/integrations-core/pull/7441).
* [Fixed] Do not render null defaults for config spec example consumer. See [#7503](https://github.com/DataDog/integrations-core/pull/7503).
* [Fixed] Update proxy section in conf.yaml. See [#7336](https://github.com/DataDog/integrations-core/pull/7336).

## 4.10.0 / 2020-08-10 / Agent 7.22.0

* [Added] Add config specs to http check. See [#7245](https://github.com/DataDog/integrations-core/pull/7245).
* [Fixed] Update ntlm_domain example. See [#7118](https://github.com/DataDog/integrations-core/pull/7118).

## 4.9.1 / 2020-07-09

* [Fixed] Raise http service check message limit. See [#7008](https://github.com/DataDog/integrations-core/pull/7008).

## 4.9.0 / 2020-06-29 / Agent 7.21.0

* [Added] Add note about warning concurrency. See [#6967](https://github.com/DataDog/integrations-core/pull/6967).

## 4.8.0 / 2020-05-17 / Agent 7.20.0

* [Added] Allow optional dependency installation for all checks. See [#6589](https://github.com/DataDog/integrations-core/pull/6589).

## 4.7.1 / 2020-04-09 / Agent 7.19.0

* [Fixed] Fix new option name in config sample. See [#6296](https://github.com/DataDog/integrations-core/pull/6296).

## 4.7.0 / 2020-04-04

* [Added] Add option to set SNI hostname via the `Host` header for RequestsWrapper. See [#5833](https://github.com/DataDog/integrations-core/pull/5833).
* [Fixed] Update deprecated imports. See [#6088](https://github.com/DataDog/integrations-core/pull/6088).
* [Fixed] Update reference to `disable_ssl_validation`. See [#5945](https://github.com/DataDog/integrations-core/pull/5945).

## 4.6.4 / 2020-02-22 / Agent 7.18.0

* [Fixed] Apply strptime thread-safety fix only on Python 2. See [#5618](https://github.com/DataDog/integrations-core/pull/5618).

## 4.6.3 / 2020-01-24 / Agent 7.17.0

* [Fixed] Document that tls_verify is False by default. See [#5547](https://github.com/DataDog/integrations-core/pull/5547).

## 4.6.2 / 2020-01-21

* [Fixed] Properly enable TLS/SSL verification when `tls_verify` is true. See [#5507](https://github.com/DataDog/integrations-core/pull/5507).

## 4.6.1 / 2020-01-17

* [Fixed] Avoid cross instance data sharing. See [#5499](https://github.com/DataDog/integrations-core/pull/5499).

## 4.6.0 / 2020-01-13

* [Added] Use lazy logging format. See [#5377](https://github.com/DataDog/integrations-core/pull/5377).

## 4.5.0 / 2019-12-02 / Agent 7.16.0

* [Added] Upgrade cryptography to 2.8. See [#5047](https://github.com/DataDog/integrations-core/pull/5047).

## 4.4.0 / 2019-11-15

* [Fixed] Update response_time metric source. See [#5025](https://github.com/DataDog/integrations-core/pull/5025).
* [Added] Add auth type to RequestsWrapper. See [#4708](https://github.com/DataDog/integrations-core/pull/4708).
* [Fixed] Improve config constructor syntax. See [#4841](https://github.com/DataDog/integrations-core/pull/4841).

## 4.3.1 / 2019-10-18 / Agent 6.15.0

* [Fixed] Ensure the correct tls_ca_cert value is used. See [#4819](https://github.com/DataDog/integrations-core/pull/4819).

## 4.3.0 / 2019-10-11

* [Added] Add option to override KRB5CCNAME env var. See [#4578](https://github.com/DataDog/integrations-core/pull/4578).

## 4.2.0 / 2019-08-24 / Agent 6.14.0

* [Added] Add request wrapper to http_check. See [#4363](https://github.com/DataDog/integrations-core/pull/4363).

## 4.1.1 / 2019-07-22 / Agent 6.13.0

* [Fixed] Fix detection of the embedded Agent directory. See [#4158](https://github.com/DataDog/integrations-core/pull/4158).

## 4.1.0 / 2019-07-04

* [Added] Update cryptography version. See [#4000](https://github.com/DataDog/integrations-core/pull/4000).

## 4.0.0 / 2019-05-14 / Agent 6.12.0

* [Changed] Remove every default header except `User-Agent`. See [#3644](https://github.com/DataDog/integrations-core/pull/3644).
* [Added] Adhere to code style. See [#3516](https://github.com/DataDog/integrations-core/pull/3516).

## 3.2.1 / 2019-03-29 / Agent 6.11.0

* [Fixed] Fix Python 3.7 support. See [#3293](https://github.com/DataDog/integrations-core/pull/3293).
* [Fixed] ensure_unicode with normalize for py3 compatibility. See [#3218](https://github.com/DataDog/integrations-core/pull/3218).

## 3.2.0 / 2019-02-18 / Agent 6.10.0

* [Added] Add url as tag. See [#3080](https://github.com/DataDog/integrations-core/pull/3080).
* [Added] [http_check] adds instance tag to metrics. See [#3065](https://github.com/DataDog/integrations-core/pull/3065).

## 3.1.1 / 2018-12-07 / Agent 6.8.0

* [Fixed] Fix unicode handling of log messages. See [#2700](https://github.com/DataDog/integrations-core/pull/2700).

## 3.1.0 / 2018-11-30

* [Added] Add option to set `stream` parameter on requests. See [#2658](https://github.com/DataDog/integrations-core/pull/2658). Thanks [syskill](https://github.com/syskill).
* [Added] Upgrade cryptography. See [#2659](https://github.com/DataDog/integrations-core/pull/2659).
* [Added] Upgrade requests. See [#2481](https://github.com/DataDog/integrations-core/pull/2481).
* [Fixed] Use raw string literals when \ is present. See [#2465](https://github.com/DataDog/integrations-core/pull/2465).
* [Added] Fix unicode handling on A6. See [#2435](https://github.com/DataDog/integrations-core/pull/2435).
* [Added] Validate that the url starts with the scheme. See [#2393](https://github.com/DataDog/integrations-core/pull/2393).

## 3.0.0 / 2018-10-12 / Agent 6.6.0

* [Added] Handle SSL exception and send a DOWN service check status. See [#2332](https://github.com/DataDog/integrations-core/pull/2332).
* [Changed] Refactoring: isolate config parsing. See [#2321](https://github.com/DataDog/integrations-core/pull/2321).

## 2.4.0 / 2018-10-01

* [Fixed] Fix fetching ca_certs from init_config. See [#2318](https://github.com/DataDog/integrations-core/pull/2318).
* [Added] Allow configuring cert expiration time in seconds. See [#2290](https://github.com/DataDog/integrations-core/pull/2290).

## 2.3.0 / 2018-09-04 / Agent 6.5.0

* [Fixed] Update cryptography to 2.3. See [#1927](https://github.com/DataDog/integrations-core/pull/1927).
* [Fixed] fix link in config option description. See [#1865](https://github.com/DataDog/integrations-core/pull/1865).
* [Added] support NTLM auth. See [#1812](https://github.com/DataDog/integrations-core/pull/1812).
* [Fixed] Add data files to the wheel package. See [#1727](https://github.com/DataDog/integrations-core/pull/1727).

## 2.2.0 / 2018-06-20 / Agent 6.3.1

* [Fixed] Add support client auth for http check cert expiration.. See [#1754](https://github.com/DataDog/integrations-core/pull/1754).
* [Fixed] Check will now send data with PUT, DELETE, and PATCH methods--not just POST. See [#1718](https://github.com/DataDog/integrations-core/pull/1718).

## 2.1.0 / 2018-06-06

* [Fixed] fixes AttributeError when running on 6.2.1. See [#1617](https://github.com/DataDog/integrations-core/pull/1617).
* [Fixed] Suppress InsecureRequestWarning for urllib3 for http_check. See [#1574](https://github.com/DataDog/integrations-core/pull/1574).
* [Added] Allow users to disable matching hostnames verification in ssl cert verification. See [#1519](https://github.com/DataDog/integrations-core/pull/1519).
* [Changed] Emit a warning if disable_ssl_validation is unset. See [#1517](https://github.com/DataDog/integrations-core/pull/1517).

## 2.0.1 / 2018-05-11

* [BUGFIX] Properly detect default certificate file for all supported Platforms. See [#1340](https://github.com/DataDog/integrations-core/pull/1340)

## 2.0.0 / 2018-03-23

* [BUGFIX] Make import of default certificate file relative rather than absolute
  Fixes loading problem on Windows, and/or allows check to be installed in other
  location
* [DEPRECATION] Remove the `skip_event` option from the check. See [#1054](https://github.com/DataDog/integrations-core/pull/1054)

## 1.4.0 / 2018-02-13

* [IMPROVEMENT] begin deprecation of `no_proxy` config flag in favor of `skip_proxy`. See [#1057](https://github.com/DataDog/integrations-core/pull/1057).

## 1.3.1 / 2018-01-17

* [BUGFIX] Use lowercase in an `if statement` for a user defined HTTP method.

## 1.3.0 / 2018-01-10

* [FEATURE] Report http connect status as metrics. See #659.
* [BUGFIX] User-defined "url" tag replaces default "url" tag. See[#301](https://github.com/DataDog/integrations-core/pull/301). (Thanks [@colinmollenhour](https://github.com/colinmollenhour))
* [FEATURE] Add configurable ssl server name for cert expiration check. See[#905](https://github.com/DataDog/integrations-core/pull/905).

## 1.2.0 / 2017-10-10

* [FEATURE] Add support for client side certificate. See[#688](https://github.com/DataDog/integrations-core/issues/688). (Thanks [@xkrt](https://github.com/xkrt))
* [IMPROVEMENT] Make tornado optional. See [#758](https://github.com/DataDog/integrations-core/issues/758).

## 1.1.2 / 2017-08-28

* [IMPROVEMENT] Improved logging. See [#652](https://github.com/DataDog/integrations-core/issues/652).

## 1.1.1 / 2017-07-18

* [BUGFIX] Fix response tuple arity in SSL certificate check. See[#461](https://github.com/DataDog/integrations-core/issues/461).

## 1.1.0 / 2017-06-05

* [FEATURE] Add support for SOAP requests. See [#328](https://github.com/DataDog/integrations-core/issues/328).
* [FEATURE] Add gauge metric for ssl days left. See [#249](https://github.com/DataDog/integrations-core/issues/249).

## 1.0.0 / 2017-03-22

* [FEATURE] adds http_check integration.
