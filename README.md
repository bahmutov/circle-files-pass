# circle-files-pass [![CircleCI](https://circleci.com/gh/bahmutov/circle-files-pass/tree/master.svg?style=svg)](https://circleci.com/gh/bahmutov/circle-files-pass/tree/master)
> Example passing multiple files from parallel jobs to a single job

Check if the [circle.yml](circle.yml) file is valid with:

```shell
$ circleci config validate circle.yml
```

This CircleCI build (see the last run by clicking on the badge) shows how the second job can run in parallel, each build creates its own file, attaches it to the common workspace, and then the third job runs after - and it receives all files created by the second job.
