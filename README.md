# Actions
Actions-Repo

# schedule:
  #  - cron: "0/5 * * * *"
  #  - cron: "0/6 * * * *"
  # push:


Post-Request zum Dispatchen:
curl -X POST -H "Accept: application/vnd.github.v3+json" -H "Content-Type: application/json" -H "Authorization: token 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" https://api.github.com/repos/Chubaker/Actions/dispatches -d '{"event_type": "build"}'

Mit payload:
$ curl -X POST -H "Accept: application/vnd.github.v3+json" -H "Content-Type: application/json" -H "Authorization: token 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" https://api.github.com/repos/Chubaker/Actions/dispatches -d '{"event_type": "build", "client_payload": { "env": "production" } }'
