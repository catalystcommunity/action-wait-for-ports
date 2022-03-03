<!-- start title -->

# GitHub Action:Hello World

<!-- end title -->
<!-- start description -->

Greet someone and record the time

<!-- end description -->
<!-- start contents -->
<!-- end contents -->
<!-- start usage -->

```yaml
- uses: catalystsquad/action-javascript-action-template@undefined
  with:
    # Who to greet
    # Default: World
    who-to-greet: ""
```

<!-- end usage -->
<!-- start inputs -->

| **Input**          | **Description** | **Default** | **Required** |
| :----------------- | :-------------- | :---------: | :----------: |
| **`who-to-greet`** | Who to greet    |   `World`   |   **true**   |

<!-- end inputs -->
<!-- start outputs -->

| **Output** | **Description**         | **Default** | **Required** |
| :--------- | :---------------------- | ----------- | ------------ |
| `time`     | The time we greeted you |             |              |

<!-- end outputs -->
<!-- start examples -->

### Example usage

```yaml
on: [push]

jobs:
  wait-for-ports:
    runs-on: ubuntu-latest
    name: Wait for ports to be available
    steps:
      - name: Wait for ports
        uses: catalystsquad/action-wait-for-ports@v1
        with:
          ports: 4000
          max-wait: 300000
          check-interval: 5000
```

<!-- end examples -->
<!-- start [.github/ghdocs/examples/] -->
<!-- end [.github/ghdocs/examples/] -->
