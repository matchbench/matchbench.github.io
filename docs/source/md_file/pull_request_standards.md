# Pull Comment Standard Documentation

## Brief Introduction

Anyone interested in our work is welcome to use Pull Request(P&R) to participate in. This documentation provides contributors guidelines for Pull Requests and the standard of P&R's Comment.

## Guidelines for Pull Requests

1. **Ask First.** Please ask first Before embarking on any significant pull request(e.g. implementing features, refactoring code...).
2. **Licensing.** By submitting a patch, you agree that your code will be licensed under the same hippie license that YOURLS uses, aka the "Do whatever the hell you want with it" license. 
3. **Quality Requirements.** Make sure your code adhere to [Google Coding Standards](https://google.github.io/styleguide/pyguide.html). Otherwise, there will be unexpected results when generating code documents. <u>Besides, if your P&R is about merging a new model, it is required to **keep the result error within the allowable range(±1.0%)**.</u>

## P&R Comment Standard

When creating a new P&R(follow the [docs](https://docs.github.com/en/pull-requests)), you should follow our P&R Comment Standard.

The Comment should include several parts: Introduction, Results, Reference,... Use Heading level 2 "##" in markdown for these heads.

The contents of these parts are described below.

- **Introduction:** The main description of your work. For example, when merging a model, write down its main features, original papers and referred repository. 
- **Results:(optional)** When merging a model, record your reproduced results and original proposed results.
- **Findings:(optional)** Interesting experimental findings can be shared in this part.
- **Required Packages:(optional)** If your P&R requires extra packages, you should list required packages here and provide codes for install.
- **Other:(optional)** 
- **Reference:** Urls of referred repository, relevant papers,...

## P&R Comment Examples

It is recommended to refer to historical comment: [pull23](https://github.com/ruc-datalab/MatchBench/pull/23), [pull24](https://github.com/ruc-datalab/MatchBench/pull/24)

## Reference

[1] https://github.com/youkpan/YOURLS/wiki/Pull-Request<br>
[2] https://github.com/ruc-datalab/MatchBench/pulls