# Trendy Cucumber
Cucumber Reporting Tool that Generates a Summary Table from Test Results.

## Example Usage
```
trendy-cucumber ./test/feature-test-results.json
```

## Example Output
```
┌───────────┬────────┬──────────┬────────┬──────────┬───────┐
│           │ Passed │ % Passed │ Failed │ % Failed │ Total │
├───────────┼────────┼──────────┼────────┼──────────┼───────┤
│ Features  │ 4      │ 80.00%   │ 1      │ 20.00%   │ 5     │
├───────────┼────────┼──────────┼────────┼──────────┼───────┤
│ Scenarios │ 18     │ 85.71%   │ 3      │ 14.29%   │ 21    │
└───────────┴────────┴──────────┴────────┴──────────┴───────┘
┌───────────────────────────┬──────────────────┬────────────────────┬──────────────────┬────────────────────┬─────────┐
│ Feature Name              │ Scenarios Passed │ % Scenarios Passed │ Scenarios Failed │ % Scenarios Failed │ % Total │
├───────────────────────────┼──────────────────┼────────────────────┼──────────────────┼────────────────────┼─────────┤
│ User Registration         │ 5                │ 23.81%             │ 3                │ 14.29%             │ 38.10%  │
├───────────────────────────┼──────────────────┼────────────────────┼──────────────────┼────────────────────┼─────────┤
│ User Login                │ 5                │ 23.81%             │ 0                │ 0.00%              │ 23.81%  │
├───────────────────────────┼──────────────────┼────────────────────┼──────────────────┼────────────────────┼─────────┤
│ Admin Login               │ 2                │ 9.52%              │ 0                │ 0.00%              │ 9.52%   │
├───────────────────────────┼──────────────────┼────────────────────┼──────────────────┼────────────────────┼─────────┤
│ Admin Dashboard           │ 4                │ 19.05%             │ 0                │ 0.00%              │ 19.05%  │
├───────────────────────────┼──────────────────┼────────────────────┼──────────────────┼────────────────────┼─────────┤
│ Admin User Creation       │ 2                │ 9.52%              │ 0                │ 0.00%              │ 9.52%   │
├───────────────────────────┼──────────────────┼────────────────────┼──────────────────┼────────────────────┼─────────┤
│                           │ 21               │ 85.71%             │ 3                │ 14.29%             │ 100%    │
└───────────────────────────┴──────────────────┴────────────────────┴──────────────────┴────────────────────┴─────────┘


```


## Generating JSON for Tests

Trendy Cucumber accepts json input. You can generate json output specify the `--format` parameter 

```
cucumber --format json:./test/feature-test-results.json
```


