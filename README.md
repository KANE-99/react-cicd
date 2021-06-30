### Run below command to run watchtower
`
docker run \
    -d \
    --name watchtower \
    -e REPO_USER=kane-99 -e REPO_PASS=Kirtesh@1661 \
    -v /var/run/docker.sock:/var/run/docker.sock containrrr/watchtower \
    --debug \
    --label-enable \
    --cleanup \
    --notifications slack --notification-slack-hook-url \ https://hooks.slack.com/services/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
`
