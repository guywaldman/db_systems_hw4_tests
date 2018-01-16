# HW4 Wet Tests 🚀

## Caveat

These tests might not be 100% accurate, may contain mistakes and may contain false positives/negatives.
Please use them at your discretion

## Requirements

* MongoDB shell version v3.4.6
* MongoDB server version: 3.4.6

## Usage

### With Node.js

> Make sure that you've moved `script.js` to the root directory, the NPM scripts rely on this.

```bash
$ npm run test
```

### Without Node.js

> Assuming your MongoDB server is running on localhost:27017.
> Otherwise, run instead of the first command, for example:
> ```bash
>   # replace <address:port> as needed
> $ mongo <address:port> test/lib/populate.js
> ```

```bash
  # populate the DB
$ mongo test/lib/populate.js
  # populate the DB
$ mongo script.js
  # run your script
$ mongo test/script.test.js
  # drop the collections
$ mongo test/lib/destroy.js
```

## Output

If you passed, there should be no special output.
Something like this:

<img src="./assets/screenshot_passed.png" alt="screenshot" height="361" width="451"/>

If you failed, there should be indication as to which test you've failed (and sometimes a suggestion as to why you probably failed).

<img src="./assets/screenshot_failed.png" alt="screenshot" height="368" width="451"/>

## Diffing

To see expected output, run:

```bash
$ mongo test/lib/showExpected.js
```