<!-- start title -->

# GitHub Action:Wait for ports

<!-- end title -->
<!-- start description -->

Waits for ports to be available

<!-- end description -->
<!-- start contents -->
<!-- end contents -->
<!-- start usage -->

```yaml
- uses: catalystsquad/action-wait-for-ports@undefined
  with:
    # Comma separated list of ports to wait for
    ports: ""

    # Max time in milliseconds to wait
    # Default: 30000
    max-wait: ""

    # How frequently to check ports, in milliseconds
    # Default: 5000
    check-interval: ""
```

<!-- end usage -->
<!-- start inputs -->

| **Input**            | **Description**                                | **Default** | **Required** |
| :------------------- | :--------------------------------------------- | :---------: | :----------: |
| **`ports`**          | Comma separated list of ports to wait for      |             |   **true**   |
| **`max-wait`**       | Max time in milliseconds to wait               |   `30000`   |  **false**   |
| **`check-interval`** | How frequently to check ports, in milliseconds |   `5000`    |  **false**   |

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
