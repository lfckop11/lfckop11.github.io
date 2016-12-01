---
layout: post
title: You're up and running!
---

Next you can update your site name, `cat /etc/isssue`, avatar and other options using the _config.yml file in the root of your repository (shown below).

```shell
alias ll="ls -alF"
alias grep="grep --color=auto"
alias pg="ps aux | head -1; ps aux | grep -v grep | grep"
alias ng="netstat -antup | awk 'NR==2'; netstat -antup | grep"
alias lg="lsof -i -n | head -1; lsof -i -n | grep"
alias extip="curl -s http://whatismyip.akamai.com/"
alias e="exit"
alias yi="yum -y install"
alias mcp="mvn clean package"
alias mcpnt="mvn clean package -DskipTests -Dmaven.test.skip=true"
alias sost="netstat -n | awk '/^tcp/ {s[\$NF]++} END{for(i in s) print i, s[i]}' OFS='\t'"
```

![_config.yml]({{ site.baseurl }}/images/config.png)

The easiest way to make your first post is to edit this one. Go into /_posts/ and update the Hello World markdown file. For more instructions head over to the [Jekyll Now repository](https://github.com/barryclark/jekyll-now) on GitHub.
