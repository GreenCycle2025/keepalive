# keep-alive

Tiny scheduled GitHub Action that pings the Render free-tier backend every ~12 minutes
so it doesn't sleep — preventing cold-start `503`s on **shoresh.1bigfam.com** (and
bagrut.1bigfam.com), which share `bagrut-math-api-img.onrender.com`.

Public repo on purpose: public repos get unlimited free Actions minutes.
No secrets, no app code — just a `curl` to `/health`.
