# reddit-submision-limiter (RSL)
Limits the number of submissions per user to a subreddit in a given timeframe. Uses PRAW and Redis.

### Requirements
- A reddit user and accompanying script app with scopes for reporting and removing posts. See the [PRAW documentation](https://praw.readthedocs.io/en/latest/index.html) for details on this.
- A local [Redis](https://redis.io/) server. Support is not provided for password-protected instances.
- Python 3 and [Pipenv](https://pipenv.pypa.io/en/latest/)

### Configuring and Running RSL
1. Copy `config.example.py` to `config.py`
2. Fill in **all** config values. Subreddit should just be the sub's name (i.e. `AskReddit`, not `/r/AskReddit`)
3. Run `pipenv install`
4. Run `pipenv run python -m main`
