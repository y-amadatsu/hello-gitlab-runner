# README

Here is a sample project to check if gitlab runner is runnable specifically on mac.

see) https://qiita.com/y-amadatsu/items/e67fab91e026634cb7fe

```
$ sudo curl --output /usr/local/bin/gitlab-runner https://gitlab-runner-$downloads.s3.amazonaws.com/latest/binaries/gitlab-runner-darwin-amd64
$ sudo chmod +x /usr/local/bin/gitlab-runner
$ git clone https://github.com/y-amadatsu/hello-gitlab-runner.git
$ cd hello-gitlab-runner
$ gitlab-runner exec docker rspec
(snip)
Finished in 0.31912 seconds (files took 1.23 seconds to load)
27 examples, 0 failures, 13 pending

Skipping cache archiving due to empty cache key
Job succeeded
```