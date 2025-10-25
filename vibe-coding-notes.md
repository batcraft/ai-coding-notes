# What I am learning from vibe coding a giant enterprise app :)

## LLM codegen is a  *buddy cop movie*

* Your new partner has unconventional methods. They are brilliant but insane
* You are the weathered, long-time veteran that has seen it all
* Your partner is going to push you out of your comfort zone and introduce you to new ways of doing your job
* You have to rein them in, teach them how the system works, and make sure they get the job done "by the book"

## And I cannot emphasize this enough, Tests

* Write tests as soon as you write code
  * (That is, tell the LLM to write them)
* Make sure your tests are strong and representative
  * We started with unit tests and e2e tests
  * We test against a live database using the same migrations (not mocks)
* You'll have to pay attention to test performance, because you are writing a lot and executing them often  

## Why Greenfield is Easier

* We live in a world of frameworks and mature patterns
  * database: golang-migrate
  * ORM: gorm
  * Frontend: vue.js, tailwind, pinia
  * Frontend Components: PrimeVue
  * Logging: slog  
* LLMs are good at doing things when the pattern is established already
* A lot of the start of an app is boilerplate and setup
* I think my best day was ~15,000 lines of code. And Miles has surely beaten that
  
## LLM Codegen doesn't have to be your stereotype of "vibe coding"

* You, and tests, and the LLM itself, can tend to this code and make sure it's not slop
* You need to proactively guide the LLM toward what it's building. You have to be good at prompting.
  * Really, good prompting is just good communication

## Fun "tail-eating" moments

* Have Copilot on github.com review your PR
  * (They really need to stop calling *everything* Copilot)
* Your IDE agent calls `gh pr view <PR_NUMBER> --comments`
* Your IDE robot addresses the comments from the github.com robot
* Lather, rinse, repeat the virtuous cycle
